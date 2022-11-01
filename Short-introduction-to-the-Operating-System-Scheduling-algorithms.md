
**1. First-Come, First-Served Scheduling**
By far the simplest CPU-scheduling algorithm is the first-come, first-served (FCFS) scheduling algorithm. With this scheme, the process that requests the CPU first is allocated the CPU first.

**2. Shortest-Job-First Scheduling**
This algorithm associates with each process the length of the process’s next CPU burst. When the CPU is available, it is assigned to the process that has the smallest next CPU burst.

**3. Priority Scheduling**
Apriority is associated with each process, and the CPUis allocated to the process with the highest priority.

**4. Round-Robin Scheduling**
It is similar to FCFS scheduling, but preemption is added to enable the system to switch between processes. A small unit of time, called a time quantum or time slice, is defined. A time quantumis generally from 10 to 100 milliseconds in length.

**5. Multilevel Queue Scheduling**
Another class of scheduling algorithms has been created for situations in which processes are easily classified into different groups. A multilevel queue scheduling algorithm partitions the ready queue into several separate queues.

**6. Multilevel Feedback Queue Scheduling**
The multilevel feedback queue scheduling algorithm, in contrast, allows a process tomove between queues. The idea is to separate processes according to the characteristics of their CPU bursts.


For detailed introduction :- https://en.wikipedia.org/wiki/Scheduling_(computing)#Scheduling_disciplines
