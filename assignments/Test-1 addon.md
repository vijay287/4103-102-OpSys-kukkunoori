## Test 1 Helper
Multi*
Define the following and give examples of each.
1.Multi-tasking :
Multitasking is defined in terms of operating system, in which multiple processes, also called tasks, can execute (i.e., run) on a single computer seemingly simultaneously and without interfering with each other.
Example :
The operating system is able to keep track of where you are in these tasks and go from one to the other without losing information.
 
2. Multi-programming :
Multiprogramming is the technique of running several programs at a time using timesharing creating logical parallelism.Helps in keeping several jobs in memory simultaneously.
Example :
Time shared systems
 
3.Multi-processing:
Multiprocessing is the ability of an operating system to execute multiple processes at the same time. It refers to the hardware (i.e., the CPU units) rather than the software (i.e., running processes). If the hardware provides more than one processor, then that is multiprocessing.
Example:
Dual core and Quad core processors.
4.Multi-threaded:
Threads are the light wait processes. Multithreading is the ability of an operating system to execute different threads at the same time. It is a technique in which a process is divided into threads and each thread runs simultaneously.
Example:
Web Servers, GUI
Review Questions From Chapters 3
1.What is an instruction trace?
We can characterize the behavior of a process by listing the sequence of instructions that execute for that process. Such a listing is referred to as a trace of the process. This is done by showing how the traces of various processes are interleaved.
2.What common events lead to the creation of a process?
Four common events lead to the creation of process. They are: 1. New batch job 2.Interactive log-on 3.Created by OS to provide a service 4.Spawned by existing process
3.What does it mean to preempt a process?
Process preemption is a situation where a process will be interrupted so that the other processes which are waiting in the queue will be executed after unit time. It is executing and could continue to execute, but is preempted so that another process can be executed. A process will be executed for a certain amount of time to which it is set. Each process will stop after the unit time and if it is not accomplished it will wait in the queue for it's turn.
4. What is swapping and what is its purpose?
Definition:
Swapping is defined as the moving a part or all of a process from main memory to disk.
Purpose:
When none of the processes in main memory is in the Ready state, the operating system swaps one of the blocked processes out into disk into a suspend queue, so that another process may be brought into main memory to execute.
5.Why does Figure 3.9b have two blocked states?
There are two independent concepts here: whether a process is waiting on an event (blocked or not) and whether a process has been swapped out of main memory (suspended or not). To accommodate this 2 by 2 combination,we need four states which are two blocked states and two ready states:
• Ready: The process is in main memory and available for execution.
• Blocked: The process is in main memory and awaiting an event.
• Blocked/Suspend: The process is in secondary memory and awaiting an event.
• Ready/Suspend: The process is in secondary memory but is available for execution as soon as it is loaded into main memory.
6.List four characteristics of a suspended process?
1.The process is not immediately available for execution.
2.The process may or may not be waiting on an event. If it is, this blocked condition is independent of the suspend condition, and occurrence of the blocking event does not enable the process to execute immediately.
3.The process was placed in a suspended state by an agent: either itself, a parent process, or the OS, for the purpose of preventing its execution.
4.The process may not be removed from this state until the agent explicitly orders the removal.
7.List three general categories of information in a process control block?
Three general categories of information in a process control block are listed below:
Process Identification: Each process is given a unique numeric identifier which holds ids of process, parent and user respectively.
Process State Information: Process State Information holds the contents of processor registers. Process registers include program counter, status registers and general purpose registers.
Process control information: This category is used be OS to manage the process. This include Scheduling & state information: ex: Ready, running etc. B. Data structuring: linking of various process in a queue. C. Memory management: describing memory in an easy way D. Resource ownership and utilization E. Process privileges F. Inter Process communication.
8.Why are two modes (user and kernel) needed?
Kernel mode in the trusted mode in the operating systems and it given access to all the hardware and CPU resources to execute low-level instructions. User mode is restricted access to hardware and CPU resources and is limited to system calls. The above mentioned modes are needed in operating system as all the programs will run in user mode whereas software runs in kernel mode, these two modes are required to run multiple programs at a time effectively.
9.What is the difference between interrupt and a trap?
Interrupts: Interrupt, an operating system function is an interruption to the normal execution of the program. When the CPU receives an interrupt, it stops the normal flow of execution of the program and transfers the control to interrupting device. Traps: Trap, an operating system function detected by CPU when there is any abnormal condition. Traps and interrupts are events that breakdown the normal flow of program execution, some of the differences between them are listed below. Whenever a program is run, the error is thrown at the same place as its trap. Then CPU asks OS for required service for program execution. Interrupts, on the other hand stops the flow of program and waits for completion until the required service is not done. Traps are synchronous events whereas interrupts are asynchronous.
10.Give three examples of an interrupt.
1.	Clock interrupt.
2.	I/O interrupt.
3.	Memory fault.
11.What is the difference between a mode switch and a process switch?
A process switch may occur any time that the OS has gained control from the currently running process where as a mode switch may occur without changing the state of the process that is currently in the Running state.

