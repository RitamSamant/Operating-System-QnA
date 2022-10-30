
**Q1) How MULTIPROGRAMMING HELP IN REDUCING CPU IDLE TIME ?**

in order to reduce the idle waiting time of the cpu (which happens when the job leaves the
job-pool(collection of all the jobs to be performed) and go for execution(i/o),CPU reamins idle)

with help of multiprogramming as soon as the job leave for i/o the os chooses another job from the queue.
so here the previous job do its i/o task and new job start doing it bound tasks reducing the cpu idle time


**Q2) WHAT IS MULTIPROCESSING?

Ability of the system to have more than one processors within the system
multiprocessing is possible because the processors share the:
i) computer bus
ii) clock
iii) memory
iv) peripheral devices
so basically a dual core processor can do 2 process at a time and a octa-core processor can do 8 process at a time


**Q3) WHAT IS MULTITHREADING?**

it is a process in which we can allow different code segments to run concurrently within
the context of the process.

formally,it is the ablity of a process to be used by many users at the single time and also manage different requests by the user

for ex: using VLC media player we can use one thread to open VLC player another to run songs another thread to add music

for ex : web server client architecture , here many request by clients are handled by the server using threads

multithreading increases the responsiveness of the system also it reduces the cost as we dont need to manage separte process for each users

NOTE: i will try post a complete article on multithreading as it is a very vast topic and here only the introduction is given


**Q4) what is meant by POST?**

Power On Self Test.
it is used to initialize the hardware devices of the computer
how?
in order to boot the system BIOS is used (now UEFI)
bios stand for (Basic Input Output System)
POST -> BIOS CHECK -> CMOS RAM ->CPU ->HARDWARE DEVICE ->SECONDARY STORAGE DEVICE
The POST first checks the bios and then tests the CMOS RAM. If there is no problem with this then POST continues to check the CPU, hardware devices such as the Video Card, the secondary storage devices such as the Hard Drive, Floppy Drives, Zip Drive or CD/DVD Drives. If some errors found then an error message is displayed on the screen or a number of beeps are heard. These beeps are known as POST beep codes. refer here
LIMITATIONS OF BIOS
can root upto 2TB device
runs in 16 bit processor mode
the complete process of loading with BIOS
BIOS -> goes of POST -> check for MBR ->retrive the BOOT-LOADER ->loads the system in RAM
and finally loads the OS


**Q5) WHAT IS MBR?**

It is a programme which runs when the computer is turning ON to find the OS.

*COLLECTED.
