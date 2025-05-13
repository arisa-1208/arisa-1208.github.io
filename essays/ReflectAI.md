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

## I. Introduction

Artificial Intelligence (AI) has become a transformative tool in education, especially in fields like Software Engineering where problem-solving, creativity, and technical precision are essential. Instead of replacing learning, AI has started to reshape how we learn by giving students new ways to understand concepts, write better code, and overcome technical challenges. In ICS 314, AI tools like ChatGPT, Claude, and GitHub Copilot played an influential role in my coding workflow and learning process. I found myself using these tools for everything from debugging and writing functions to explaining concepts I didn’t fully understand the first time they were discussed in class.

These tools provided on-demand explanations, code examples, and real-time help, which allowed me to work more efficiently and gain a deeper understanding of key software engineering principles. Whether I was working on a timed WOD, writing an essay about coding standards, or trying to fix a broken API route in our final project, AI became a constant resource. At the same time, using AI also taught me the importance of reviewing its responses carefully and learning how to ask better, more specific questions. This essay reflects on how AI has impacted my experience in ICS 314—the challenges, the benefits, and how it shaped the way I now approach software engineering.

---

## II. Personal Experience with AI

### 1. Experience WODs (e.g., E18)
For most of the Experience WODs, I used ChatGPT to help me understand what the assignment was asking for and how to efficiently code my solution. Taking E18: Functional Programming as an example, I asked: “Without using a for or a while loop, can you help me implement the functions using the Array functional methods?” This helped me understand how functional programming worked and how to write the code to get the output I was looking for.

After completing a few of the Experience WODs, I realized that the videos attached to the assignments were actually really helpful. So toward the end of the semester, I started using AI less and relied more on the videos instead. Honestly, watching the videos felt faster and clearer than trying to figure out what to ask AI and how to interpret the output it gave me.

### 2. In-class Practice WODs
I used ChatGPT for the In-class Practice WODs such as for example, the one where we recreated the Murphy’s React mockup using Next.js. I asked both ChatGPT and Claude specific questions like, “Can you help me recreate the navbar so that it looks just like the one seen in the photo?”

For the most part, AI was helpful, but there were times when I had trouble explaining exactly what I wanted. As a result, I sometimes got a navbar that looked completely different from what I was hoping for. That’s when I realized that AI isn’t super reliable, and that we should only be using it as a supportive tool to guide our thinking and not something to blindly depend on.

### 3. In-class WODs
I can say that I used AI for all of the In-class WODs we had. There were definitely times during the WODs when I struggled to explain exactly what I wanted help with. One example was the WOD where we had to recreate the KoHana Rum “Our Journey” page using React. I remember having a hard time figuring out how to get the navbar and footer to work exactly how I wanted.

I asked multiple times how to get the dropdown menu button in the top right corner to only appear when the screen was minimized. In the end, with the help of both ChatGPT and Claude, I was able to create a mockup that came very close to the original design by the time the WOD ended.

### 4. Essays
When writing essays, I used both ChatGPT and Claude to help brainstorm ideas and restructure sentences. For example, I asked: “Can you help me rephrase this paragraph that I wrote about coding standards?” Since I understand that essays should reflect my own thoughts and experiences, I never used AI to write the entire essay—only to improve clarity and fix grammatical errors.

I felt like AI was helpful, but sometimes the rewritten versions sounded way too different from how I would naturally write. In those cases, I preferred using other tools like Grammarly to help me refine my paragraphs while keeping my original voice.

### 5. Final Project
In the final project (Sync'd Study), I used ChatGPT to troubleshoot React and Prisma bugs. For example, I asked: “Why does Prisma return 'null' for findUnique even though the ID exists?” The response helped me verify that I was missing a where clause.

Another example was when I asked ChatGPT for help regarding an issue in my schema.prisma file where I couldn't get the foreign key relationship between users and study sessions to work properly. I said, "Why is my relation from StudySession to users not working even though both tables exist in Supabase?" It helped me realize that I was referencing the wrong model name and the types were mismatched (e.g., using text vs uuid).

Also, I asked, “Why aren’t the usernames showing up on the front end even though I can see them stored in the users table on Supabase?” ChatGPT helped me debug and suggested checking if the data was properly fetched and if I was actually selecting the correct joined fields in my API call. It turned out I had forgotten to include the .select() call to pull in user details from the related table.

There were times when it was quite unhelpful, for example when I asked it to update the file again with the new changes, it would either give me the code with the section that I asked for fixed, but the function that used to work will not work anymore, or the layout would be completely different than what I originally had. 

### 6. Learning a concept / tutorial
When reviewing React hooks and unfamiliar syntax like useEffect, I asked: “Explain useEffect in simple terms with an example.” The step-by-step example was easier to understand than many official docs.

Another time, I was struggling to connect Vercel, Supabase, and Prisma. I asked ChatGPT questions like:

“How do I connect my deployed Vercel app to my Supabase database?”
“Why isn’t Prisma recognizing my Supabase schema on production?”
“How do I open and inspect my Supabase database in pgAdmin?”

AI walked me through checking my .env file configuration, setting the correct DATABASE_URL, syncing schema changes with Prisma migrate, and using Supabase connection strings to link it with external clients like pgAdmin. These tutorials were especially helpful because they combined multiple technologies I hadn’t used together before.

### 7. Answering a question in class or Discord
During class discussions, our professor asked thoughtful and challenging questions like: “What’s the difference between implementing a web app in React versus implementing it in Next.js?” and “Why is risk management important for software development projects?” Even if I had a general idea of the answer, I would quietly ask ChatGPT to help double-check my understanding before speaking up.

For the React vs. Next.js question, AI helped me understand that React focuses on building UI components, while Next.js builds on top of React by adding routing, server-side rendering, and backend integration features, making it better suited for full-stack development. When I asked about risk management, ChatGPT explained that it’s important because it helps teams identify and address potential issues early on, which can prevent delays, reduce costs, and make the development process more predictable.

Using AI like this made me feel more confident in class, especially when I wasn’t totally sure if I had the right answer. It was like having a quick and reliable study buddy that helped me prepare before contributing to the discussion.

### 8. Asking or answering a smart-question
I haven’t used AI for this section because I didn’t participate in the smart-questions chat on the Discord channel. I usually asked my questions in class, and they were more about personal things like grades and due dates.

### 9. Coding example
One of the most helpful times I used ChatGPT for a coding example was when I was confused about how to use console.log() properly for debugging. I knew it was useful, but I wasn’t sure where or how to use it effectively. I asked ChatGPT: “Can you give me examples of how to use console.log to debug in JavaScript?”

It provided a variety of examples, like printing variables inside a loop, checking if a function was being called, and formatting logs for better readability. This made it much easier for me to track down errors during WODs and while debugging our final project.

### 10. Explaining code
Since WODs were timed and required quick thinking, I often took time the night before to study my in-class WOD solutions by asking ChatGPT to explain what each part of the code meant. For example, I asked, “Can you break down what this map and filter chain is doing in this React component?” This helped me understand the logic ahead of time so I could work faster and more confidently during the actual timed WOD.

### 11. Writing code
One of the most memorable uses of AI for writing code was when I worked on the assignment to recreate a page from a real-world website. I chose the Tiffany & Co. homepage as my design inspiration. The layout was complex and elegant, and I wasn’t sure how to replicate the structure and styling from scratch. I asked ChatGPT: “Can you help me write the full code to recreate the Tiffany & Co. homepage using React and Bootstrap with similar layout and styling?”

It provided a basic template with a navbar, hero section, and some responsive cards that resembled the original website. While I had to make several adjustments to match the font, spacing, and imagery better, it gave me a solid starting point. It also explained each section so I could modify it to fit my project.

This saved me hours of trial and error and helped me understand how to break down a commercial site into React components. It also helped me build a habit of reviewing structure and styling patterns from professional websites.

### 12. Documenting code
I used ChatGPT to help generate documentation for my functions, especially during the Sync’d Study project. I asked: “Can you generate JSDoc comments for this React function that returns a list of study sessions?” ChatGPT provided a formatted block with parameter descriptions, return values, and a short explanation of what the function does.

This was really helpful because it taught me how to write clearer, standardized documentation. Before that, I didn’t really know what was expected beyond a simple comment. It also made my code easier for my teammates to understand and for me to revisit later.

### 13. Quality assurance
When ESLint gave me an error, I asked ChatGPT: “How do I fix the missing dependency in useEffect warning?” and it explained how to fix the warning safely. 

It also helped when I asked questions like: “What’s wrong with this map function in React?” and provided clear explanations of key props and best practices. I used this a lot when testing new features during our final project.

### 14. Other uses in ICS 314
I used AI in several smaller but important ways throughout the course. Before submitting assignments, I often asked ChatGPT to remind me of the correct steps for submitting GitHub repositories or final deliverables, just to make sure I didn’t miss anything. It helped me stay organized and confident about meeting all the requirements.

AI also helped me prepare for my final project proposal presentation. I asked for help drafting a short pitch and practiced explaining the project idea clearly. ChatGPT even helped me anticipate questions I might be asked during the presentation.

Lastly, I used AI to resolve GitHub issues like merge conflicts and push errors. I would ask things like “How do I fix a non-fast-forward error?” and follow the steps to solve problems quickly. I felt like this helped me a lot since as someone who never used GitHub before, I probably would have been deleting code that I should not have touched. 

---

## III. Impact on Learning and Understanding
At first, even before this class, I thought using AI felt like “cheating” in a way. But after using it throughout my assignments, I realized that maybe it’s not as bad as I thought.

The biggest thing I noticed is that even though I was making small steps compared to people who are already really good at coding and databases, AI helped me understand the general rules and how to work through problems. I was first introduced to coding late in high school, and to be honest, my first real experience with coding was when I took my first ICS class in college. What helped me grow from a beginner into someone who better understands software development was the support I got from AI.

AI helped me understand software engineering concepts faster, especially when I was stuck or confused about what the assignment was asking. It made me more confident in debugging and explaining code to others. But I also quickly learned not to rely on it too much. Sometimes, AI gave outdated or overly complicated answers, and I realized I needed to think critically and not follow it blindly. I remember that for specific WODs, my professor warned us not to depend on AI completely because it could send us down the wrong path.

Throughout the semester, I worked with AI by my side through every assignment. Without it, I think I would’ve stayed confused about a lot of things, such as the differences between Next.js, TypeScript, and React. AI helped me gain a better understanding of these topics and encouraged me to look at problems from different angles.

---

## IV. Practical Applications
Outside of ICS 314, I used AI to help me in other areas of school and career development. One major example was when I worked on my professional resume. I asked ChatGPT questions like “Can you help me reword this bullet point to sound more professional?” or “What’s a strong summary for a student applying to tech internships?” It gave me good examples and formatting tips that helped me polish my resume.

I also used AI in other classes to summarize content, study for exams by generating practice questions, or clarify difficult readings. If I didn’t understand parts of the textbook, I’d paste the content into ChatGPT and ask it to simplify or explain the main ideas. It made studying less overwhelming.

Even outside of school, I’ve used AI to summarize recent news or help with random tasks. It’s become a regular part of how I get things done. I also ask how I should plan my study times so that it works best for my learning style.

---

## V. Challenges and Opportunities
One challenge I faced when using AI was figuring out how to phrase my prompts. Sometimes I knew what I wanted, but I didn’t know how to ask it clearly. That would lead to unrelated or confusing answers. Also, there were times when AI gave code that looked fine but didn’t actually work in my project. That taught me that AI can’t replace understanding or testing your code for yourself.

At the same time, AI opened up new opportunities. It helped me work independently and explore tools like Supabase and Prisma more quickly because it broke things down step by step. That made me excited to explore even more advanced tools in future projects and classes.

---

## VI. Comparative Analysis
When comparing traditional learning with AI-enhanced learning, I think both have their strengths. Traditional lectures and discussions are great for understanding theory and getting feedback. But AI helped me reinforce those lessons by giving me quick answers and examples right when I needed them. Using both together, like reviewing class material with AI afterward, made me feel more confident and engaged.

AI also filled in gaps when I didn’t want to bother a classmate or professor with a small question. It felt like having a personal tutor available anytime. I’d often be working until 3 or 4 a.m., and AI was always there for me, from the simplest questions to really complex ones. But I also had to make sure I wasn’t blindly copying anything and always verified the responses.

---

## VII. Future Considerations
I think AI will become an even bigger part of software engineering education in the future. Right now, it’s mostly used to answer questions or explain concepts, but I could see it being used to grade practice code, suggest optimizations, or give feedback on readability and structure. That would help students improve faster.

I also hope that future classes teach students not just how to use AI, but how to use it responsibly, like writing clear prompts and double-checking responses. AI makes things faster, but it’s not always perfect, so it should be treated as a helpful resource, not a shortcut.

It would be really cool if AI tools were integrated directly into IDEs or course platforms so students wouldn’t need to switch tabs or copy/paste code. But these tools should support learning, not replace it. If used the right way, I really believe AI can make classes more interactive and helpful without taking away the challenge of figuring things out on your own.

---

## VIII. Conclusion
Reflecting on my time in ICS 314, I’ve realized how much AI has helped me grow and not just as a student, but as someone who’s really starting to understand what software engineering is all about. I used AI in almost every assignment, from the early WODs where I didn’t even know how to phrase my questions properly, to our final project where we were working with real tools like Supabase, Prisma, and Vercel. It wasn’t always easy—actually, most of the time it was really hard—but AI gave me a place to start when I felt lost.

The final project especially pushed me the most. My group and I stayed up so late trying to make everything functional. Debugging took way longer than actually building the pages. But even though it was stressful, I think it was one of the best experiences I’ve had in college so far. I learned how all the pieces, front end, back end, databases, actually connect. And when something broke (which happened a lot), I turned to ChatGPT to help me figure out where I went wrong, whether it was a schema mismatch or a missing select call in an API route. I still had to do a lot of testing and trial and error, but AI helped me understand the logic behind the tools, not just copy code blindly.

Through this class, I stopped thinking of AI as something that “does the work for you” and started seeing it as something that helps you learn how to do the work. It gave me confidence when I wasn’t sure how to move forward and helped me turn vague ideas into something real and working.

Overall, ICS 314 taught me that software engineering isn’t just about writing code but instead it’s about problem-solving, working with others, testing, and constantly learning. AI helped me throughout all of that, but I also learned that I need to double-check everything it says and think for myself. I know I still have a lot more to learn, but I feel more prepared now, and a big part of that is because of how I learned to use AI effectively in this class.

*This essay was reviewed using AI (ChatGPT) for grammar checking and readability improvements.*
