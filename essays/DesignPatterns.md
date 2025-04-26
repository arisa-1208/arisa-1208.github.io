---
layout: essay
type: essay
title: "The Secret Recipes Behind Great Code: A Reflection on Design Patterns"
# All dates must be YYYY-MM-DD format!
date: 2025-04-24
published: true
labels:
  - Programming
  - Design Patterns
  - Software-Engineering
---

<img width="200px" class="rounded float-start pe-4" src="../img/IMG_5643.jpg">

&nbsp; 

Have you ever tried cooking without a recipe? You just grab a bunch of random ingredients and hope it turns out okay. Sometimes it does, but other times it’s a complete disaster.
Honestly, coding without design patterns feels the same way. You might get lucky and make something that works, but it’ll probably be messy, confusing, and way harder to fix later.

In software development, design patterns are like trusted recipes that developers have created over time. They’re not strict rules — more like helpful guides that give you a starting point when you run into a common problem. Instead of having to figure out everything from scratch every time, you can pull a "recipe" from the design pattern book and know you're on the right track. It makes your code more organized, easier to understand, and easier for other people to work with, too. It also saves you a lot of time when the project gets bigger, because you don’t have to untangle a mess you accidentally made earlier.

## Why Do Design Patterns Even Matter?

Imagine trying to build a house without blueprints. Every construction team would have to come up with a new way to stack bricks, wire electricity, or put in plumbing.
Most houses would end up looking weird, falling apart, or being impossible to fix. It would be chaotic.
Design patterns in coding help avoid that kind of chaos. They give us blueprints that are already tested and known to work.

Another huge reason why design patterns are important is that they help teams work together better.
If I tell another developer, "Hey, I used a Singleton here," they’ll immediately understand what I mean. I don’t have to explain every detail of how it works. It saves a lot of time and makes collaboration smoother.

Even when working alone, design patterns can make a difference. It’s easy to lose track of your own code after a few weeks or months. Using patterns makes it easier to come back later and still understand what you were trying to do. It gives your code structure and a kind of "language" that you and others can read.

## How I’ve Used Design Patterns in My Code

When I first started coding, I didn’t even realize I was using design patterns. I just did whatever felt natural. But once I learned more, I started seeing how much easier it is when you actually know the patterns and use them on purpose.

One project where I really got to use design patterns was my final project for my software engineering class, called Sync’d Study.
Sync’d Study is a web application designed to help students at the University of Hawai‘i at Mānoa optimize their study time through peer-organized, in-person study sessions. Students can propose or join study sessions for different subjects, and depending on the course, they can sign up as "sensei" (helpers), "grasshoppers" (learners), or both.

When building Sync’d Study, I used the Singleton Pattern to manage our database connection. I made sure there was only one active connection that the whole app could use, which helped prevent crashes or weird bugs when multiple users interacted with the database at the same time.
I also used the Observer Pattern for our calendar system. When study sessions were added, edited, or deleted, multiple parts of the app — like the calendar view, the session list, and notifications — needed to update right away. Instead of coding each update manually, I set it up so those parts could "subscribe" to changes. This made everything a lot smoother and reduced the chances of missing an update.

Thinking back, I also used parts of the Factory Pattern in Sync’d Study without fully realizing it at first. We had different user types — sensei, grasshopper, or both — and instead of putting messy if statements all over the place, I set up a system that created the right type of user object depending on the situation. Later, when I learned more about design patterns, I realized I had built a basic Factory without even planning it that way!

Outside of Sync’d Study, I have used these patterns in smaller projects, too. For example, in a personal project where I was building a simple online store mockup, I used a Factory to create different product objects depending on their category. It made adding new types of products much easier without having to rewrite everything.

## What I Learned From Using Design Patterns

One of the biggest things I learned from using design patterns is that good code is not just about making things work — it’s about making things easy to understand and easy to change later.
When you’re first building a project, it’s tempting to take shortcuts and just focus on getting it done. But in bigger projects, or when you come back to your code after a few months, those shortcuts turn into headaches. Design patterns help prevent that by forcing you to think about structure from the start.

I also learned that you don’t have to use a pattern exactly the way it’s written. Sometimes you have to adjust it a little to fit your specific project. And that’s okay — design patterns are meant to be flexible tools, not rigid instructions.
Finally, working with patterns made me a better teammate. It’s so much easier to collaborate when everyone understands the structure and logic behind the code.

Learning about design patterns gave me more confidence, because now when I face a new coding challenge, I know there’s probably a pattern that can help me solve it — and if not, I at least know how to organize my thinking better.

## Final Thoughts

So, if someone asked me, "What are design patterns?" I would say they’re like recipes for solving common coding problems — smart, reusable solutions that make your code cleaner, faster to build, and easier to work with.
And if they asked, "What design patterns have you used?" I could confidently say I’ve used Singleton for managing shared resources, Observer for keeping different parts of the app updated, and Factory for creating flexible objects, especially in real-world projects like Sync’d Study.

Design patterns don’t magically make your project perfect, but they give you a much better starting point. Just like following a good recipe when cooking, using the right design pattern makes it much more likely you’ll end up with something people actually want to use and that you can be proud of.
At the end of the day, it’s about working smarter, not harder — and being able to build things that last.

*This essay was reviewed using AI(ChatGPT) for grammar checking to ensure and correctness and improve readability.*
