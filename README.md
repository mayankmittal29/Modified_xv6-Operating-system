project_root/
│
├── partB/
│   ├── report_partB.txt
│
├── my_plot.png
│
└── test.txt

Analysis of Scheduling Policies:

The project includes an analysis of the performance of different scheduling policies based on response times (rtimes) and wait times (wtimes) for CPU-bound processes. The following observations have been made:

    Round Robin (RR):
        Response Time (RT): 18
        Wait Time (WT): 177
        Description: Processes are executed in a cyclic order, one by one, with the CPU performing a context switch after each tick.

    First-Come, First-Served (FCFS):
        Response Time (RT): 24
        Wait Time (WT): 144
        Description: CPU completes executing one process before moving to the next, resulting in higher response times compared to Round Robin.

    Multi-Level Feedback Queue (MLFQ):
        Response Time (RT): 19
        Wait Time (WT): 123
        Description: New processes are added to the end of the first queue with a time slice of one tick. The initial response time is similar to Round Robin due to similar scheduling behavior.

Graphical Representation:

The provided my_plot.png graph visually represents the CPU-bound processes organized in queues 1, 2, 3, and 4. Priority is being reduced over time. The data used for creating this graph is stored in test.txt.

Handling Aging:

Aging has not been implemented in the current version of the scheduler. However, it can be integrated by utilizing a loop at the beginning of the scheduler function to adjust priorities over time.

Additional Notes:

    The project assumes a specific directory structure where partB contains the report for Part B of networks.
    The README provides a concise overview of the project's structure, analysis, and graphical representation, facilitating easy understanding and navigation for users.
