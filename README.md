# Analysis of Scheduling Policies 🔄📊

## Introduction
This project analyzes the performance of different CPU scheduling policies based on response times (RT) and wait times (WT) for CPU-bound processes. It includes a graphical representation and considerations for handling aging in future updates.

### Directory Structure 📁
project_root/
│
├── partB/
│ ├── report_partB.txt
│
├── my_plot.png
│
└── test.txt

## Scheduling Policies and Observations 📝

### Round Robin (RR)
- **Response Time (RT):** 18
- **Wait Time (WT):** 177
- **Description:** Processes are executed in a cyclic order, one by one, with the CPU performing a context switch after each tick.

### First-Come, First-Served (FCFS)
- **Response Time (RT):** 24
- **Wait Time (WT):** 144
- **Description:** CPU completes executing one process before moving to the next, resulting in higher response times compared to Round Robin.

### Multi-Level Feedback Queue (MLFQ)
- **Response Time (RT):** 19
- **Wait Time (WT):** 123
- **Description:** New processes are added to the end of the first queue with a time slice of one tick. The initial response time is similar to Round Robin due to similar scheduling behavior.

## Graphical Representation 📊

The provided `my_plot.png` graph visually represents CPU-bound processes organized in queues 1, 2, 3, and 4, where priority is reduced over time. Data used for this graph is stored in `test.txt`.

## Handling Aging 🔧

Aging has not been implemented in the current scheduler version but can be integrated by utilizing a loop at the beginning of the scheduler function to adjust priorities over time.

## Additional Notes ℹ️

- The project assumes a specific directory structure where `partB` contains the report for Part B of networks.
- The README provides a concise overview of the project's structure, analysis, and graphical representation, facilitating easy understanding and navigation for users.

