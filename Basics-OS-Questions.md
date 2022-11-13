
**1. Why is the operating system important?**

OS is the most essential and vital part of a computer without which it is considered useless. It enables an interface or acts like a link for interaction between computer software that is installed on OS and users. It also helps to communicate with hardware and also maintains balance among hardware and CPU. It also provides services to users and a platform for programs to run on. It performs all common tasks applications require. 


**2. What's the main purpose of an OS? What are the different types of OS?**
The main purpose of an OS is to execute user programs and make it easier for users to understand and interact with computers as well as run applications. It is specially designed to ensure that the computer system performs better by managing all computational activities. It also manages computer memory, processes, and operation of all hardware and software.

Types of OS:
Batched OS (Example: Payroll System, Transactions Process, etc.)
Multi-Programmed OS (Example: Windows O/S, UNIX O/S, etc.)
Timesharing OS (Example: Multics, etc.)
Distributed OS (LOCUS, etc.)
Real-Time OS (PSOS, VRTX, etc.)


**3. What are the benefits of a multiprocessor system?**

A Multiprocessor system is a type of system that includes two or more CPUs. It involves the processing of different computer programs at the same time mostly by a computer system with two or more CPUs that are sharing single memory. 

Benefits:
Such systems are used widely nowadays to improve performance in systems that are running multiple programs concurrently. 
By increasing the number of processors, a greater number of tasks can be completed in unit time. 
One also gets a considerable increase in throughput and is cost-effective also as all processors share the same resources.
It simply improves the reliability of the computer system.


**4. What is GUI?**

GUI (Graphical User Interface) is basically a type of user interface that allows users to use graphics to interact with OS. GUI is created because it is more user-friendly, less complex, and easier to understand rather than a command-line interface. Its main goal is to increase efficiency and ease of use. Instead of having to memorize commands, users can just click on a button to simply execute the procedure. Examples of GUI include Microsoft Windows, macOS, Apple’s iOS, etc.


**5. What is RAID structure in OS? What are the different levels of RAID configuration?**

RAID (Redundant Arrays of Independent Disks) is a method used to store data on Multiple hard disks therefore it is considered as data storage virtualization technology that combines multiple hard disks. It simply balances data protection, system performance, storage space, etc. It is used to improve the overall performance and reliability of data storage. It also increases the storage capacity of the system and its main purpose is to achieve data redundancy to reduce data loss. 

Nowadays, RAID is available in various schemes or RAID level as given below:
RAID 0 - Non-redundant striping: This level is used to increase the performance of the server.
RAID 1 - Mirroring and duplexing: This level is also known as disk mirroring and is considered the simplest way to implement fault tolerance.
RAID 2 - Memory-style error-correcting codes: This level generally uses dedicated hamming code parity I.e., a liner form of error correction code.
RAID 3 - Bit-interleaved Parity: This level requires a dedicated parity drive to store parity information.
RAID 4 - Block-interleaved Parity: This level is similar to RAID 5 but the only difference is that this level confines all parity data to a single drive.
RAID 5 - Block-interleaved distributed Parity: This level provides far better performance than disk mirroring and fault tolerance.
RAID 6 - P+Q Redundancy: This level generally provides fault tolerance for two drive failures.


**6. Explain demand paging?**

Demand paging is a method that loads pages into memory on demand. This method is mostly used in virtual memory. In this, a page is only brought into memory when a location on that particular page is referenced during execution. The following steps are generally followed:

Attempt to access the page.
If the page is valid (in memory) then continue processing instructions as normal.
If a page is invalid then a page-fault trap occurs.
Check if the memory reference is a valid reference to a location on secondary memory. If not, the process is terminated (illegal memory access). Otherwise, we have to page in the required page.
Schedule disk operation to read the desired page into main memory.
Restart the instruction that was interrupted by the operating system trap


**7. What do you mean by RTOS?**

Real Time Operating System (RTOS) is an operating system that is used for real-time applications i.e., for those applications where data processing should be done in a fixed and small measure of time. It performs much better on tasks that are needed to be executed within a short time. It also takes care of execution, monitoring, and all-controlling processes. It also occupies less memory and consumes fewer resources. 

Types of RTOS:

a.Hard Real-Time
b.Firm Real-Time
c.Soft Real-Time


**8. What do you mean by process synchronization?**

Process synchronization is basically a way to coordinate processes that use shared resources or data. It is very much essential to ensure synchronized execution of cooperating processes so that will maintain data consistency. Its main purpose is to share resources without any interference using mutual exclusion. There are two types of process synchronization:

a.Independent Process
b.Cooperative Process


**9. What is IPC? What are the different IPC mechanisms?**

IPC (Interprocess Communication) is a mechanism that requires the use of resources like a memory that is shared between processes or threads. With IPC, OS allows different processes to communicate with each other. It is simply used for exchanging data between multiple threads in one or more programs or processes. In this mechanism, different processes can communicate with each other with the approval of the OS.

Different IPC Mechanisms:

a.Pipes
b.Message Queuing
c.Semaphores
d.Socket
e.Shared Memory
f.Signals


**10. What do you mean by overlays in OS?**

Overlays is basically a programming method that divides processes into pieces so that instructions that are important and need can be saved in memory. It does not need any type of support from the OS. It can run programs that are bigger in size than physical memory by only keeping only important data and instructions that can be needed at any given time. 


**11. Write top 10 examples of OS?**

Some of the top OS’s that are used mostly are given below:
a.MS-Windows
b.Ubuntu
c.Mac OS
d.Fedora
e.Solaris
f.Free BSD
g.Chrome OS
h.CentOS
i.Debian 
j.Android

*[Source- InterviewBit]
