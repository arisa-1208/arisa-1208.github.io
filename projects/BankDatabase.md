---
layout: project
type: project
image: img/bank-database/bank-database-square.png
title: "Bank Database System"
date: 2024
published: true
labels:
  - C Programming
  - Data Structures
  - File Management
summary: "A C-based bank record management system implementing linked lists for dynamic record storage."
---

<img class="img-fluid" src="../img/bank-database/bank-database-header.png">

## Project Overview  
This project is a **C-based bank record management system** that allows users to **add, search, modify, and delete bank records** stored in a linked list. The system ensures efficient memory usage and provides a user-friendly interface for handling records dynamically. The program operates through a menu-driven interface, allowing users to interact with the database easily.  

The project focused on fundamental concepts such as **linked lists, dynamic memory allocation, and structured programming**. It also required careful implementation of **input validation and error handling** to ensure smooth execution and data integrity. Debugging was an essential part of development, and special attention was given to identifying memory leaks and handling segmentation faults.  

The final system supports:  
- Adding a new bank record with an account number, name, and address.  
- Searching for a record by account number.  
- Modifying existing records.  
- Deleting a record from the database.  
- Printing all stored records.  

---

## Data Structures & Implementation  
The system is built using **linked lists** to manage bank records dynamically. Each record is stored in a **struct** containing the following fields:  

- `accountno` – Unique integer identifier for each bank account.  
- `name` – Character array to store the account holder’s name.  
- `address` – Multi-line address stored as a character array.  
- `next` – Pointer to the next record in the linked list.  

## Code Implementation  
### Adding a New Record  
```c
void addRecord(struct record **start, int accountno, char name[], char address[]) {
    struct record *newRecord = malloc(sizeof(struct record));
    if (newRecord != NULL) {
        newRecord->accountno = accountno;
        strcpy(newRecord->name, name);
        strcpy(newRecord->address, address);
        newRecord->next = *start;
        *start = newRecord;
    }
}
