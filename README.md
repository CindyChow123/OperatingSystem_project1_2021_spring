# Pintos Project 1 of CS302 in SUSTECH
**DO NOT EVER COPY IT FOR YOUR CLASS PROJECTS!!**
## Description
This project is originally designed by Stanford for their operating System course and the project
materials are based on the released guide for UC Berkeley CS 162 Operating System.
# Task
## 1 Task 1: Modification of timer sleep in Alarm Clock
In this task, we are asked to modify the inefficiently implemented timer sleep
function. The original implementation uses "busy waiting" strategy to
keep the corresponding thread sleeping instead of working, which results
in wasted CPU resources. In our implementation, we need to come up
with an alternative way to efficiently call a thread to sleep.
## 2 Task 2: Priority Scheduler
Implement a priority scheduler, so that
1. higher-priority threads always run before lower-priority threads,
2. shared resources prefer higher-priority threads, with the modification
of 3 Pintos synchronization primitives (lock, semaphore, condition
variable),
3. Pintos locks have priority donation mechanism when multiple threads
acquire or release the locks.
## 3 Task 3: Advanced Scheduler - a Multi-level Feedback Queue Scheduler
(mlfqs)
A mlfqs must meet the following requirements:
1. Maintain several queues of ready-to-run threads each with a different
priority,
2. Round Robin order is used when selecting a thread from the same
priority queue,
3. scheduler data values should be updated before any kernel threads
see a newly increased timer ticks() value,
4. scheduler data values should be updated using given formulas.
