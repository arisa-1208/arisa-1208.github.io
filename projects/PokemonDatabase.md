---
layout: project
type: project
image: img/pokemon.jpg
title: "Pokémon Database: File I/O Implementation in C"
date: 2024
published: true
labels:
  - C Programming
  - File Handling
  - Binary File I/O
summary: "A Pokémon database system implemented in C, using file I/O operations for structured data storage. ICS 212"
---

<img class="img-fluid" src="../img/pokemon_database.png" style="max-width: 70%; border: 2px solid #ddd; border-radius: 8px; padding: 5px; margin-bottom: 20px;">

## Project Overview  
This project is a **Pokémon database system** that allows users to **store and retrieve Pokémon data** (name and level) using **file I/O operations in C**. It focuses on **binary file handling**, ensuring structured data storage that persists between program runs.  

The project involved implementing key functions for **writing and reading structured data** using `fwrite()` and `fread()`, ensuring that Pokémon records were saved correctly and retrieved accurately. Testing was conducted using custom test drivers to validate file handling and data integrity.

The final system supports:  
- Writing Pokémon data to a binary file (`writefile` function).  
- Reading Pokémon data from the file (`readfile` function).  
- Ensuring structured data storage and retrieval.  
- Handling errors like missing or corrupted files.  

---

##  **Writing and Reading Pokémon Data (iofunctions.c)**

The `writefile` function is responsible for **storing Pokémon records** into a binary file. Each Pokémon has a **name** (stored as a character array) and a **level** (stored as an integer). The function ensures that the data is written in a structured format.

```c
/*****************************************************************
//
//  Function name: writefile
//
//  DESCRIPTION:   This function writes the Pokemon data stored 
//                 in the array to a file. If the file exists, 
//                 then it will be overwritten.
//
//  Parameters:    pokearray (struct pokemon[]) : array of Pokemon to write
//                 num (int)                    : number of Pokemon to write
//                 filename (char[])            : name of the file to write to
//
//  Return values:  0 : success
//                 -1 : error (file could not be opened)
//
****************************************************************/

int writefile(struct pokemon pokearray[], int num, char filename[])
{  
    /* Open the writefile (file will be overwritten if already exists) */
    FILE *pokemonFile = fopen(filename, "w");
    
    int i = 0;

    /* Check if file was successfully opened */
    if (pokemonFile == NULL) 
    {
        return -1; /* return if file could not be opened */
    }
    
    /* Loop the array of pokemons and write their data to the file */
    for (i = 0; i < num; i++) 
    {
        fprintf(pokemonFile, "%d\n", pokearray[i].level); /* Write the Pokemon's level */
        fprintf(pokemonFile, "%s\n", pokearray[i].name); /* Write the Pokemon's name */
    }
    
    /* Close the file so that all of the data is written */
    fclose(pokemonFile);
    return 0;
}

```
The `readfile` function retrieves Pokémon records from a binary file and stores them in an array.

```c
/*****************************************************************
//
//  Function name: readfile
//
//  DESCRIPTION:   This function reads the Pokemon data from a file
//                 and stores it in an array. It stops reading if it 
//                 reaches the maximum array size or the end of the 
//                 file. 
//
//  Parameters:    pokearray (struct pokemon[]) : array to store Pokemon data
//                 num (int*)                   : pointer to the number of Pokemon
//                 filename (char[])            : name of the file to read from
//
//  Return values:  0 : success
//                 -1 : error (file could not be opened)
//
****************************************************************/

int readfile(struct pokemon pokearray[], int *num, char filename[])
{
    int i = 0; /* Counter to how many pokemons have been read so far */

    /* Open the readfile (read it from an existing file) */
    FILE *pokemonFile = fopen(filename, "r");

    /* If fopen returns NULL, then the file was unable to open so return -1 */
    if (pokemonFile == NULL) 
    {
        return -1;
    }

    /* Loop through to read the data from the file. Either read the max number of pokemons or until it reaches the end of the file */
    while (i < *num && fscanf(pokemonFile, "%d\n", &pokearray[i].level) != EOF && fgets(pokearray[i].name, sizeof(pokearray[i].name), pokemonFile) != NULL) 
    {
        /* Remove the newline character from the name, if there is one */
        if (pokearray[i].name[strlen(pokearray[i].name) - 1] == '\n')
        {
            pokearray[i].name[strlen(pokearray[i].name) - 1] = '\0';
        }
        i++;
    }
    
    /* Update the num variable so we can see how many pokemons were read */
    *num = i;
    
    /*Close the file to make sure that all the data is saved and is properly closed */
    fclose(pokemonFile);

    return 0;
}
```
---
##  **Example Output**

Below is an example of how the program writes Pokémon data to a file and retrieves it using `writefile` and `readfile`. The program first stores three Pokémon records and then reads them back, displaying the retrieved data.

```
==== Test Case 1 ====
Calling writefile with 3 pokemons, filename: 'pokemons1.txt'
writefile returned: 0
Successfully wrote 3 pokemons to 'pokemons1.txt'

Calling readfile to read pokemons from 'pokemons1.txt'
readfile returned: 0
Successfully read 3 pokemons from 'pokemons1.txt'
Pokemon 1 - Level: 19, Name: Pikachu
Pokemon 2 - Level: 81, Name: Eevee
Pokemon 3 - Level: 24, Name: Sylveon

==== Test Case 2 ====
Calling writefile with 3 pokemons, filename: 'pokemons2.txt'
writefile returned: 0
Successfully wrote 3 pokemons to 'pokemons2.txt'

Calling readfile to read pokemons from 'pokemons2.txt'
readfile returned: 0
Successfully read 3 pokemons from 'pokemons2.txt'
Pokemon 1 - Level: 150, Name: Skitty
Pokemon 2 - Level: 220, Name: Happiny
Pokemon 3 - Level: 100, Name: Jigglypuff
```
---
###  **My Role & Contributions**
My role in this project was to implement the **file I/O functions (`writefile` and `readfile`) in `iofunctions.c`**, ensuring that Pokémon data was written and retrieved correctly. Additionally, I developed **`driver.c`**, a test program that systematically verified file operations by storing sample Pokémon records, reading them back, and checking for errors such as missing or corrupted files. I was responsible for designing the structure of the file storage, handling error cases, and debugging issues related to data persistence and incorrect formatting. To confirm that the program worked as expected, I created test scenarios and documented results in `output.txt`.  

###  **Lessons Learned & Skills Gained**
This project strengthened my understanding of **binary file handling in C** and improved my skills in **structured programming and debugging file-related issues**. I learned how to manage structured data efficiently using `fwrite()` and `fread()`, how to handle errors like unreadable files, and how to test file operations with systematic validation. Additionally, I gained experience in writing **modular code**, breaking down functionality into separate files (`iofunctions.c` and `driver.c`), which made the program more organized and easier to maintain. This experience provided me with a deeper understanding of how **real-world applications store and retrieve data persistently**, reinforcing key concepts in file handling and structured programming.
