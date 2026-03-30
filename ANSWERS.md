# Assignment Questions

## Instructions
Answer all 4 questions with detailed explanations. Each answer should be **3-5 sentences minimum** and demonstrate your understanding of the concepts.

---

## Question 1: Thread vs Process

**Question**: Explain the difference between a **thread** and a **process**. Why did we use threads in this assignment instead of creating separate processes?

**Your Answer:**

[Write your answer here. Consider: What is a process? What is a thread? How do they differ in terms of memory, resources, creation overhead? Why are threads more suitable for this simulation?]
A process is a independent program with its own memory, while a thread is a worker inside a process that shares memory with others, making it better for this simulation because it allows faster performance and easy sharing
---

## Question 2: Ready Queue Behavior

**Question**: In Round-Robin scheduling, what happens when a process doesn't finish within its time quantum? Explain using an example from your program output.

**Your Answer:**

[Write your answer here. Describe the specific behavior - where does the process go? When does it run again? Give an example from your actual program output showing a process that was re-queued.]
its return to the ready queue , its run when the front process finshed the time quantum and now the process turn to go out to the cpu , 
Example from my output:
```
P1 executing quantum [3000ms] 
  ? Quantum progress: [███████████████] 100%
  ? P1 completed quantum 3000ms │ Overall progress: [██████████████░░░░░░] 72%
     Remaining time: 1146ms
  ? P1 yields CPU for context switch

  ? P1 (Priority: 1) added to ready queue │ Burst time: 4146ms
┌─ Ready Queue ─────────────────────────────────────────────────────────────────
│ [P3 ? P4 ? P5 ? P6 ? P7 ? P8 ? P9 ? P10 ? P11 ? P12 ? P1]
└───────────────────────────────────────────────────────────────────────────────
[Paste a relevant snippet from your program output here showing a process being re-queued]
```

**Explanation of example:**
[Explain what's happening in the output snippet you pasted]
the burst time of the p1 is 4146ms and the quantum is 3000ms the remaning is 1146ms so the p1 go back to ready queue and start runing when the front processes finished the quantum
---

## Question 3: Thread States

**Question**: A thread can be in different states: **New**, **Runnable**, **Running**, **Waiting**, **Terminated**. Walk through these states for one process (P1) from your simulation.

**Your Answer:**

[Write your answer here. For each state, explain when P1 enters that state during the simulation. Use your understanding of the code to trace through the lifecycle.]

1. **New**: [When is P1 in New state?] the New state when the program first creates it and it is ready to start

2. **Runnable**: [When does P1 become Runnable?] becomes Runnable when it enters the ready queue It is waiting for its turn to use the cpu

3. **Running**: [When is P1 Running?] Running when the cpu is doing its work in its time 

4. **Waiting**: [When/why would P1 be Waiting?] waiting if it has to stop for a moment (like waiting for a resource or because its time is up) before it can run again

5. **Terminated**: [When is P1 Terminated?] terminated when it finishes all its work and leaves the system

---

## Question 4: Real-World Applications

**Question**: Give **TWO** real-world examples where Round-Robin scheduling with threads would be useful. Explain why this scheduling algorithm works well for those scenarios.

**Your Answer:**

### Example 1: [Name of application/scenario] website

**Description**: 
[Describe the real-world scenario or application]
server handle many users who are visiting the website at the same time
**Why Round-Robin works well here**: 
[Explain why Round-Robin scheduling is suitable. Consider fairness, responsiveness, predictability, etc.]
every user gets a time, so no one has to wait too long for their page to load
### Example 2: [Name of application/scenario]
Operating Systems
**Description**: 
[Describe the real-world scenario or application]
Running many apps at once
**Why Round-Robin works well here**: 
[Explain why Round-Robin scheduling is suitable. Consider fairness, responsiveness, predictability, etc.]
The cpu switches so fast between apps that they all seem to run at the same time without freezing
---

## Summary

**Key concepts I understood through these questions:**
1. Threads are fast, lightweight "workers" that share the same memory
2. This system is fair because it gives every task a specific time slice
3. I learned how a task moves from "New" to "Terminated."

**Concepts I need to study more:**
1. How to stop threads from making mistakes when sharing data
2. How to pick the best time limit for the fastest performance
