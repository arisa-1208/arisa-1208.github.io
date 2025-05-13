---
layout: essay
type: essay
title: "Reflecting On The Use of AI in ICS 314"
# All dates must be YYYY-MM-DD format!
date: 2025-05-12
published: true
labels:
  - Software Development
  - ChatGPT
  - AI Usage
---

<img width="200px" class="rounded float-start pe-4" src="../img/IMG_5643.jpg">

&nbsp; 

## I. Introduction

Artificial Intelligence (AI) has become a transformative tool in education, especially in fields like Software Engineering where problem-solving, creativity, and technical precision are essential. Instead of replacing learning, AI has started to reshape how we learn—giving students new ways to understand concepts, write better code, and overcome technical challenges. In ICS 314, AI tools like ChatGPT, Claude, and GitHub Copilot played an influential role in my coding workflow and learning process. I found myself using these tools for everything from debugging and writing functions, to explaining concepts I didn’t fully understand the first time in class.

These tools provided on-demand explanations, code examples, and real-time help, which allowed me to work more efficiently and gain a deeper understanding of key software engineering principles. Whether I was working on a timed WOD, writing an essay about coding standards, or trying to fix a broken API route in our final project, AI became a constant resource. At the same time, using AI also taught me the importance of reviewing its responses carefully and learning how to ask better, more specific questions. This essay reflects on how AI has impacted my experience in ICS 314—both the challenges and the benefits—and how it shaped the way I now approach software engineering.

## II. Personal Experience with AI

### 1. Experience WODs (e.g., E18)
For most of the Experience WODs, I have used ChatGPT to help me understand what the assignment was asking for and how I should efficiently code my solution. For E18, Functional Programming, I asked: "Without using a for or a while loop, can you help me implement the functions using the Array functional methods?" This helped me to understand how functional programming worked and how I needed to code this so that I can get the output that I want.

### 2. In-class Practice WODs
I used Chat GPT for the In-Class Practice WODs, for example the recreation of the Murphy's React Mockup using Next.js. I have asked AI (ChatGPT and Claude) specific questions such as "Can you help me recreate the navbar so that it looks just like the one seen in the photo?" For the most part, AI was able to help me recreate there were times where I was having a hard time trying to explain exactly what I wanted which as a result, I was given a completely different navbar than what I was hoping to see. 

### 3. In-class WODs
I can say that I used AI for all of the In-class WODs that we had. Through my experience, there were times throughout the WOD where I was having a hard time figuring out how to explain what I wanted AI to give me. An example would be the WOD where we had to recreate the KoHana Rum Our Journey Page. through React. I remember how I was having a hard time figuring out how to get the navbar and the footer work just as I wanted. I have asked multiple times how to get the dropdown menu button in the top right hand corner in the navbar to show only when I minimize the tab. Though at the end, with the use of both ChatGPT and Claude, I was able to create a very close mockup website by the time limit.

### 4. Essays
For writing the essays, I used both ChatGPT and Claude to help brainstorm ideas and restructure sentences. For example, I asked: “Can you help me rephrase this paragraph that I wrote about coding standards?” Though since I understand that essays should reflect your own thoughts and experiences, I have never used it to write the entire essay, only to improve clarity and get rid of any grammatical errors. I felt like AI was useful but I did not like how it sometimes gave me an updated response that sounded way different than how I would word things. So in that case, I just used other sites such as grammarly to help me refine my paragraphs. 

### 5. Final Project
In the final project (Sync'd Study), I used ChatGPT to troubleshoot React and Prisma bugs. For example, I asked: “Why does Prisma return 'null' for findUnique even though the ID exists?” The response helped me verify that I was missing a where clause.

Another example was when I asked ChatGPT for help regarding an issue in my schema.prisma file where I couldn't get the foreign key relationship between users and study sessions to work properly. I said, "Why is my relation from StudySession to users not working even though both tables exist in Supabase?" It helped me realize that I was referencing the wrong model name and the types were mismatched (e.g., using text vs uuid).

Also, I asked, “Why aren’t the usernames showing up on the front end even though I can see them stored in the users table on Supabase?” ChatGPT helped me debug and suggested checking if the data was properly fetched and if I was actually selecting the correct joined fields in my API call. It turned out I had forgotten to include the .select() call to pull in user details from the related table.

There were times when it was quite unhelpful, for example when I asked it to update the file again with the new changes, it would either give me the code with the section that I asked for fixed, but the function that used to work will not work anymore, or the layout would be completely different than what I originally had. 

### 6. Learning a concept / tutorial
When reviewing React hooks and unfamiliar syntax like useEffect, I asked: “Explain useEffect in simple terms with an example.” The step-by-step example was easier to understand than many official docs.

Another example was when I was struggling to connect Vercel, Supabase, and Prisma. I asked ChatGPT questions like:

“How do I connect my deployed Vercel app to my Supabase database?”
“Why isn’t Prisma recognizing my Supabase schema on production?”
“How do I open and inspect my Supabase database in pgAdmin?”

AI walked me through checking my .env file configuration, setting the right DATABASE_URL, syncing schema changes with prisma migrate, and using Supabase connection strings to link it with external clients like pgAdmin. These tutorials were especially helpful because they combined multiple technologies that I had never used together before. 

### 7. Answering a question in class or Discord
Before answering classmates’ questions on Discord, I occasionally verified my responses with ChatGPT to ensure accuracy. For instance, I asked: “What happens if you omit a key prop in a React list?”

Also, during small class discussions when the professor asked questions, even if I felt like I already knew the correct answer, I would still quietly ask AI to confirm my thoughts before speaking up. For example, if the professor asked, “What does the spread operator do in JavaScript?”, I would quickly prompt ChatGPT with: “Explain the JavaScript spread operator in one sentence with an example.” This helped reassure me that what I was about to say was accurate and clear, especially when I wasn’t 100% confident.

### 8. Asking or answering a smart-question
I have not used AI at all for this section as I do not think I have not participated in the smart-questions chat in the Disord channel before. I would usually ask my questions in class without using AI since they were all related to my personal things, such as grades and due dates. 

### 9. Coding example
One of the most helpful times I used ChatGPT for a coding example was when I was confused about how to use console.log() properly for debugging. I knew it was useful, but I wasn’t sure where or how to use it to actually see what my variables were doing. I asked ChatGPT: “Can you give me examples of how to use console.log to debug in JavaScript?”

It provided a variety of examples, like printing variables inside a loop, checking if a function is being called, and even how to format logs for better readability. This made it much easier for me to track down errors during WODs and project debugging sessions.

### 10. Explaining code
Since WODs were timed and required quick thinking, I would often take time the night before to study my in-class WOD solutions by asking ChatGPT to explain what each part of the code meant. For example, I asked, “Can you break down what this map and filter chain is doing in this React component?” This helped me understand the logic ahead of time so that I could work faster and more confidently during the actual timed WOD.

### 11. Writing code
One of the most memorable uses of AI for writing code was when I worked on the assignment to recreate a page from a real-world website. I chose the Tiffany & Co. homepage as my design inspiration. The layout was complex and very elegant, and I wasn’t sure how to replicate the structure and styling from scratch. I asked ChatGPT: “Can you help me write the full code to recreate the Tiffany & Co. homepage using React and Bootstrap with similar layout and styling?”

It provided a basic template that included a navbar, hero section, and some responsive cards that closely resembled the original website. While I had to make adjustments to match the font, spacing, and imagery better, it gave me a really strong starting point. It also explained each section of the code so I could modify it to fit my project needs.

This saved me hours of trial and error and helped me better understand how to break down a real commercial site into React components. It also helped me build a habit of reviewing structure and styling patterns across different professional websites.

### 12. Documenting code
I used ChatGPT to help generate documentation for my functions, especially when we were working on components for the Sync’d Study project. I asked: “Can you generate JSDoc comments for this React function that returns a list of study sessions?” ChatGPT provided a formatted block with parameter descriptions, return values, and a short explanation of what the function does.

This was especially helpful because it taught me how to write clear and standardized documentation. Before that, I didn’t really know what was expected beyond a simple comment. It also made my code easier to read for my teammates, and made it easier for me to revisit functions I hadn’t looked at in a while.

### 13. Quality assurance
When ESLint gave me an error, I asked ChatGPT: “How do I fix the missing dependency in useEffect warning?” It explained the warning and how to fix it safely.

It also helped when I asked things like: “What’s wrong with this map function in React?” and provided a clear explanation of key props and best practices. I used this often when testing new features during our final project.

### 14. Other uses in ICS 314
I used AI in several smaller but important ways throughout the course. Before submitting assignments, I often asked ChatGPT to remind me of the correct steps for submitting GitHub repositories or final deliverables to make sure I didn’t miss anything. It helped me stay organized and confident about meeting all requirements.

AI also helped me prepare for my final project proposal presentation. I asked for help drafting a short pitch and practiced explaining the project idea clearly. ChatGPT even helped me anticipate questions I might be asked during the presentation.
Lastly, I used AI to resolve GitHub issues like merge conflicts and push errors. I would ask things like “How do I fix a non-fast-forward error?” and follow the steps to resolve problems quickly.

## III. Impact on Learning and Understanding
In the beginning or even before I took this class, using AI seemed like I was "cheating" in a way. But then after working along with it in my assignments, I have started to realize that maybe using AI is not as bad as I thought. 

The big thing that I felt was that although it may be baby steps when compared to those that are very skilled in coding, using databases, and etc., I strongly feel like AI has really helped me understand the general rules and the way I should and could work around softwares. The very first time that I was introduced to coding was in the late times of high school and so to be honest, the time I was truly introduced to real coding was when I went to my very first ICS class here in college. But what helped that amature coder to have a good understanding of software development was the use of AI. 

AI helped me understand software engineering concepts faster, especially when I was stuck or confused by what the assignment was asking for. It made me more confident in debugging and in explaining code to others. However, it didn't take too long for me to understand the downfall of fully relying on AI. I realized that I needed to think critically about its output, because it could be confidently wrong or provide outdated methods. I remember that for specific WODs, my professor would warn us to not completely rely on AI as it may take us to the wrong and complicated path to the solution. 
But throughout this whole semester and working together with AI right beside me as I complete these assignments, I can definitely say that without the use of AI, I probably would have still been confused on how things worked. For example the differences between Next.js, Typescript, and React. It has helped me gain valuable knowledge in many ways as ChatGPT has challenged me to think about issues and problems through various aspects, not just one point of view.

## IV. Practical Applications
Outside of ICS 314, I used AI to help me in other areas of school and career development. One major example is when I worked on my professional resume. I asked ChatGPT questions like “Can you help me reword this bullet point to sound more professional?” or “What’s a strong summary for a student applying to tech internships?” It gave me great examples and formatting suggestions that helped me polish my resume.

I’ve also used AI in my other classes to summarize content, help me study for exams by asking for practice questions, or clarify difficult readings. If I needed help understanding parts of the textbook, I would paste the exact content into ChatGPT and ask it to organize or simplify the main ideas. It helped reduce my stress and made studying feel more manageable.

Even outside of school, I have been relying a lot on AI, for example having it summarize the recent news that is going on around the world, and etc. 

## V. Challenges and Opportunities
One of the challenges I faced with using AI was figuring out the right prompts to ask. Sometimes I knew what I wanted, but if I didn’t phrase the question clearly, I would get an unrelated or confusing response. There were also times when the code that AI gave me looked good but didn’t actually work in my project. This taught me that while AI is helpful, it doesn’t replace testing and understanding your own code.

However, AI also opened up new opportunities. It let me work independently on things I may have struggled to figure out alone. I was able to explore new tools like Supabase and Prisma more quickly because I had help breaking down how to use them. This made me excited to explore even more advanced tools in future classes and projects.

## VI. Comparative Analysis
When comparing traditional learning with AI-enhanced learning, I found both have strengths. Traditional lectures and discussions are better for understanding theory and getting feedback. But AI helped me reinforce those lessons by giving me instant answers and examples. When I combined both, such as using AI after class to review what we learned, I felt more confident and engaged. 

AI also helped fill in the blanks when I didn’t want to bother a classmate or the professor with small questions. It became a sort of assistant that gave me the freedom to work at my own pace. I really feel like I have a personal tutor no matter when and where I am at. I would often stay up till 3 or 4 in the morning to study or complete assignments but AI is always there for me when I need to ask the simplest questions to the most difficult questions ever. But at the same time, I always had to be careful to verify AI’s answers and not just copy what it gave me without thinking.

## VII. Future Considerations
I think AI will become an even bigger part of software engineering education in the future. Right now, it's mainly used to answer questions or explain concepts, but I can see it being used for things like grading practice code, suggesting more efficient solutions, or even giving feedback on code quality and readability in real time. That could really help students improve faster.

I also hope that future classes encourage students to not just use AI, but to use it responsibly. That means learning how to write clear, specific prompts and knowing how to double-check the responses they get. AI can make things more efficient, but it’s not always perfect, so students need to be taught to treat it as a tool, not a final answer.

It would be really cool if AI tools were built directly into the platforms we already use—like IDEs, course websites, or even coding challenge platforms. That way, students wouldn’t need to keep switching tabs or copying and pasting their code into a separate window. But at the same time, it’s important that these tools are designed to support the learning process, not just hand out solutions. If AI is used in the right way, I think it can actually make classes more interactive and helpful, without taking away the challenge or value of figuring things out ourselves.

## VIII. Conclusion
Reflecting on my time in ICS 314, I’ve realized how much AI has helped me grow—not just as a student, but as someone who’s really starting to understand what software engineering is all about. I used AI in almost every assignment, from the early WODs where I didn’t even know how to phrase my questions properly, to our final project where we were working with real tools like Supabase, Prisma, and Vercel. It wasn’t always easy—actually, most of the time it was really hard—but AI gave me a place to start when I felt lost.

The final project especially pushed me the most. My group and I stayed up so late trying to make everything functional. Debugging took way longer than actually building the pages. But even though it was stressful, I think it was one of the best experiences I’ve had in college so far. I learned how all the pieces—front end, back end, databases—actually connect. And when something broke (which happened a lot), I turned to ChatGPT to help me figure out where I went wrong, whether it was a schema mismatch or a missing select call in an API route. I still had to do a lot of testing and trial and error, but AI helped me understand the logic behind the tools, not just copy code blindly.

Through this class, I stopped thinking of AI as something that “does the work for you” and started seeing it as something that helps you learn how to do the work. It gave me confidence when I wasn’t sure how to move forward and helped me turn vague ideas into something real and working.

Overall, ICS 314 taught me that software engineering isn’t just about writing code—it’s about problem-solving, working with others, testing, and constantly learning. AI helped me throughout all of that, but I also learned that I need to double-check everything it says and think for myself. I know I still have a lot more to learn, but I feel more prepared now, and a big part of that is because of how I learned to use AI effectively in this class.

*This essay was reviewed using AI(ChatGPT) for grammar checking to ensure and correctness and improve readability.*
