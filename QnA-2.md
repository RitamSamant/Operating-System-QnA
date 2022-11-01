
**1. When is Multithreading not useful?**
a) On a single processor machine and a desktop application, you use multi threads so you don't freeze the app but for nothing else really.
b) On a single processor server and a web based app, no need for multi threading because the web server handles most of it.
c) On a multi-processor machine and desktop app, you are suggested to use multi threads and parallel programming. Make as many threads as there are processors.
d) On a multi-processor server and a web based app, no need again for multi threads because the web server handles it.
   In total, if you use multiple threads for other than un-freezing desktop apps and any other generic answer, you will make the app slower if you have a single core machine due to the threads interrupting each other.
Why? Because of the hardware switches. It takes time for the hardware to switch between threads in total. On a multi-core box, go ahead and use 1 thread for each core and you will 
greatly see a ramp up.
    
**2. What is paging?**
Paging is a memory-management scheme that permits the physical address space of a process to be noncontiguous or in other words eliminates the need for contiguous allocation of 
physical memory.
That is we can have logically use memory spaces that physically lie at different locations in the memory
This allows viewing memory spaces that physically lie at different locations in the hardware to be logically viewed as contiguous.
This is possible via mapping of physical and virtual memory that is done by hardware component called memory management unit (MMU). The mapping process that is done by MMU 
is basically paging process.

Frames vs pages
Frames are basically the sliced up physical memory blocks of equal size. Example : 512kb of memory can be divided into 4 parts for 128kb each
While, pages are sliced up logical memory blocks of equal size. While solving any problem always the page size should be equal to frame size.
Page address is called logical address and is a combination of  by page number (denoted as ‘p’) and offset (denoted as ‘d’).
Page number sometimes is also called as VPN(Virtual Page Number).
Logical Address = Page number + page offset

Frame address is called physical address and is a combination of a frame number (denoted as ‘f’) and the offset (denoted as ‘d’).
Frame number is also sometimes referred as PFN (Physical Frame Number).
Physical Address = Frame number + page offset.

There are two ways paging can happen in the system
Using Page Table
Using translation look-aside buffers or TLB’s.

**3. What is Thrashing? && What is Page fault?**
Page Fault and Swapping
 A page fault occurs when the memory access requested (from the virtual  address space) does not map to something that is in RAM. A page must  then be sent from RAM to swap, so 
 that the requested new page can be  brought from swap to RAM. This results in 2 disk I/Os. Now you might know that disk I/Os are very slow as compared to memory access.

  Thrashing
  Now if it happens that your system has to swap pages at such a higher rate that major chunk of CPU time is spent in swapping then this state is known as thrashing. So effectively 
  during thrashing, the CPU spends less time in some actual productive work and more time in swapping.

  Cause of Thrashing
  High degree of multiprogramming: -The CPU scheduler sees the decreasing CPU utilization and increases the degree of multiprogramming as a result. The new process tries to get 
  started by taking frames from running processes, causing more page faults and a longer queue for the paging device. As a result, CPU utilization drops even further, and the CPU 
  scheduler tries to increase the degree of multiprogramming even more
  Lack of frames:- If  a process has less number of frames then less pages of that process will be able to reside in memory and hence it would result in more frequent swaping. This may 
  lead to thrashing. Hence sufficient amount of frames must be allocated .

 Recovery
 Do not allow the system to go into thrashing by instructing the long term scheduler not to bring the processes into memory after the threshold.
 If the system is already in thrashing then instruct the mid term schedular to suspend some of the processes so that we can recover the system from thrashing.
    
    
