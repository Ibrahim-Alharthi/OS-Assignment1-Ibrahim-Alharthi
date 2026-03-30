# Reflection Questions

## Instructions
Answer the following questions about your learning experience. Each answer should be **at least 5-7 sentences** and show your understanding.

---

## Question 1: What did you learn about multithreading?

**Your Answer:**

[Write your answer here. Discuss specific concepts like thread creation, thread states, how threads execute concurrently, what surprised you, etc.]
I learned that multithreading lets one program do many things at the same time. Instead of using "heavy" processes, we use small "threads" that share memory. This makes the program work much faster because threads can talk to each other easily. I found out that each thread moves through different states, like Running and Waiting. It was cool to see how the Time Quantum gives every thread a fair turn. Overall, using threads makes our simulation smooth and stops the computer from lagging. This assignment showed me how to manage many tasks in a simple way.
---

## Question 2: What was the most challenging part of this assignment?

**Your Answer:**

[Describe the specific challenge. Was it understanding the code? Implementing a feature? Using Git? Explain what made it difficult and how it relates to the course concepts.]
The most difficult part was managing the Time Quantum for each thread. It was hard to stop a thread at the exact right time and move it to the back of the queue. I also struggled with Shared Memory because many threads tried to change the same data at once. This relates to the course concept of Race Conditions, where data can get mixed up if we are not careful. I had to learn how to use synchronization to keep the data safe. It was also tricky to track the different thread states like Running and Waiting in the output. Overall, making the simulation fair for every process was the biggest challenge.
---

## Question 3: How did you overcome the challenges you faced?

**Your Answer:**

[Describe your problem-solving approach. Did you read documentation? Ask for help? Debug systematically? What resources did you use? What strategies worked?]

---

## Question 4: How can you apply multithreading concepts in real-world applications?

**Your Answer:**

[Give specific examples from real applications you use (web browsers, games, mobile apps, etc.). Explain why threads are useful in those scenarios. Connect to what you learned in this assignment.]
I can see multithreading in many real-world apps like Web Browsers and Games. For example, in a browser, one thread loads the text while another thread loads the images. In PC Games, one thread handles the graphics and another thread handles the sound at the same time. This is very useful because it stops the app from freezing while it's doing a big task. This assignment taught me that using threads makes apps feel very smooth and responsive. It also showed me that sharing memory between these tasks is much faster than opening many separate programs. Now I understand why my favorite apps can do many things at once without slowing down. Overall, multithreading is the key to making modern software run efficiently for every user
---

## Additional Reflections (Optional)

### What would you like to learn more about?

[Any topics related to threading, concurrency, or operating systems that you're curious about?]

---

### How confident do you feel about multithreading concepts now?

[Rate yourself and explain: Beginner / Intermediate / Confident]

[Explain your rating - what do you understand well? What needs more practice?]

---

### Feedback on the assignment

[Any comments about the assignment? Was it helpful? Too easy/hard? Suggestions for improvement?]
