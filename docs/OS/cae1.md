
# Question bank



<iframe src="https://drive.google.com/file/d/1QTdMaDsm3UGllLTA7Afj3QjZjpfgDzA7/preview" width="640" height="880" allow="autoplay"></iframe>

## 1. Explain Operating System History?

Operating systems have a rich history that dates back to the earliest days of computing. Here's a brief overview:

Early Computers (1940s-1950s):
- The first electronic computers, such as the ENIAC and UNIVAC, were huge machines designed for specific tasks like calculations and data processing.
- These early computers didn't have operating systems in the modern sense. Programs were written directly in machine code and executed one at a time.

Batch Processing Systems (1950s-1960s):
- As computers became more widespread, the need for more efficient use of resources arose.
- Batch processing systems were developed to queue up tasks (or jobs) and execute them in batches.
- Operating systems like the IBM OS/360 were created to manage this process, handling tasks such as job scheduling, memory management, and I/O operations.

Time-Sharing Systems (1960s-1970s):
- Time-sharing systems allowed multiple users to interact with a computer simultaneously.
- This era saw the development of operating systems like MULTICS and later Unix, which introduced features like virtual memory, file systems, and a hierarchical directory structure.

Personal Computers (1980s-Present):
- The advent of personal computers led to the development of operating systems like MS-DOS, Mac OS, and eventually Windows and Linux.
- Graphical user interfaces (GUIs) became standard, making computers more accessible to non-technical users.
- Today, operating systems continue to evolve with advancements in technology, including mobile operating systems like Android and iOS, as well as cloud-based operating systems for distributed computing.

## 2. Draw operating system component diagram and explain in details?

**Component Diagrams**  are used to show code modules of a system in  [Unified Modeling Language (UML)](https://www.geeksforgeeks.org/unified-modeling-language-uml-introduction/). They are generally used for modeling subsystems. It represents how each and every component acts during execution and running of a system program. They are also used to show and represent structure and organization of all components. These code modules include application program, ActiveX control, Java Beans, backend databases, or some ASP programs. The component diagrams represent implementation of view models. The component diagrams are for representing interfaces and dependencies among software architecture. The word component simply means modules of a class that usually represents an independent subsystem.  
These components have ability to interface with rest of system. The component diagram is used to explain working and behavior of various components of a system and is static diagrams of UML. They are also used for subsystem modeling. The main purpose of component diagram is simply to show relationship among various components of a system.

The component and interface are as shown below :![](https://media.geeksforgeeks.org/wp-content/uploads/20200702185801/Untitled-Diagram-346.png)**Example –**  Following is a component diagram for the ‘On-line Course Registration’ system. This diagram shows conceptual view of server-side components.![](https://media.geeksforgeeks.org/wp-content/uploads/20200702185827/Untitled-Diagram-437.png)**Advantages :**

-   Component diagrams are very simple, standardized, and very easy to understand.
-   It is also useful in representing implementation of system.
-   These are very useful when you want to make a design of some device that contains an input-output socket.
-   Use of reusable components also helps in reducing overall development cost.
-   It is very easy to modify and update implementation without causing any other side effects.

**Disadvantages :**

-   They cannot be used for designing Software like web pages, applications, etc.
-   It also requires sponsoring equipment and actuators for each and every component.
## 3. Explain Batch Operating System in detail?

A batch operating system is a type of operating system that executes jobs in batches without user interaction. Here's a detailed explanation:

- **Definition**: In a batch operating system, tasks or jobs are collected into batches and executed without direct user interaction. Each batch typically consists of multiple tasks, and the operating system executes these tasks in sequence.

- **Job Submission**: Users submit their jobs to the system through job control languages or batch queues. These jobs are stored in a job queue until they can be executed.

- **Job Scheduling**: The operating system scheduler selects jobs from the job queue based on priority, resource availability, and other criteria. It then allocates resources (such as CPU time and memory) to each job for execution.

- **Job Execution**: Once a job is selected for execution, the operating system loads the necessary program and data into memory and begins executing the job. The job continues until it completes or encounters an error.

- **Job Management**: The operating system manages the execution of multiple jobs simultaneously, ensuring that each job receives its fair share of resources. It may also handle job dependencies and priorities to optimize system performance.

- **Output Processing**: After a job completes, the operating system handles the output, which may include printing results or storing them in files. The output is typically directed to designated devices or storage locations.

- **Examples**: Early mainframe computers, such as the IBM 360 series, used batch operating systems like OS/360. These systems were commonly used for tasks such as payroll processing, accounting, and scientific computing.

- **Advantages**:
  - Efficient resource utilization: Batch processing allows the system to execute jobs continuously, maximizing CPU and I/O device utilization.
  - Streamlined workflow: Users can submit multiple jobs for processing without waiting for each job to complete, improving overall system throughput.
  - Automated execution: Batch operating systems automate the execution of jobs, reducing the need for manual intervention and increasing system reliability.

- **Disadvantages**:
  - Lack of interactivity: Batch operating systems lack user interaction during job execution, making them unsuitable for tasks requiring real-time response or user input.
  - Long turnaround times: Jobs may spend significant time waiting in the job queue before execution, leading to longer turnaround times for users.
  - Limited flexibility: Batch processing is best suited for repetitive, non-interactive tasks, limiting the types of applications that can be run efficiently.

## 4. Explain Multi-programming and multitask operating system?

Multi-programming and multitasking are techniques used in operating systems to improve system efficiency and user productivity. Here's an explanation of each:

- **Multi-programming**:
- **Definition**: Multi-programming is a technique where multiple programs are loaded into memory simultaneously, allowing the CPU to switch between them for execution.
- **Objective**: The primary goal of multi-programming is to maximize CPU utilization by keeping the CPU busy with productive work at all times.
- **Operation**: In a multi-programmed system, the operating system maintains a pool of ready-to-execute programs in memory. When a program needs to perform I/O operations or encounters a blocking condition, the operating system switches to another program that can execute immediately.
- **Advantages**: 
  - Improved CPU utilization: Multi-programming ensures that the CPU is always busy executing programs, reducing idle time and improving overall system throughput.
  - Faster response times: By allowing multiple programs to execute concurrently, multi-programming can reduce the response time for individual tasks.
  - Enhanced system efficiency: Multi-programming enables efficient use of system resources, allowing multiple users or tasks to share the available computing resources
    **Examples**: Mainframe operating systems like IBM z/OS and UNIX-like operating systems such as Linux and FreeBSD employ multi-programming techniques to manage multiple concurrent processes.
-  **Multitasking**:
  
  - **Definition**: Multitasking is a broader concept that encompasses the simultaneous execution of multiple tasks or processes within a single computing environment.
  - **Objective**: The primary goal of multitasking is to improve user productivity by allowing users to perform multiple tasks concurrently without interference.
  -   **Operation**: In a multitasking operating system, the CPU switches rapidly between multiple tasks, giving the illusion of parallel execution. Each task is allocated a time slice or quantum during which it can execute before being preempted.
  - **Advantages**:
  -   Increased productivity: Multitasking allows users to perform multiple tasks simultaneously, such as browsing the web while listening to music or editing documents.
  -   Enhanced responsiveness: Users can switch between tasks seamlessly, leading to a more responsive computing experience.
  -   Efficient resource utilization: Multitasking optimizes resource usage by allowing multiple tasks to share system resources such as CPU time and memory.
  - **Examples**: Modern desktop operating systems like Windows, macOS, and Linux support multitasking, enabling users to run multiple applications concurrently on their computers.
I summary, multi-programming focuses on maximizing CPU utilization by keeping the CPU busy with productive work, while multitasking allows users to perform multiple tasks simultaneously within a single computing environment, improving user productivity and system responsiveness.

## 5.  Explain distributed OS and Real-time OS?

-  **Distributed Operating System (DOS)**:

-   **Definition**: A distributed operating system is a type of operating system that manages resources and coordinates communication between multiple independent computers interconnected via a network.
-   **Objective**: The primary goal of a distributed operating system is to provide a unified computing environment across a network of computers, allowing users and applications to access resources transparently.
-   **Features**:
    -   Transparency: Distributed operating systems hide the complexities of network communication and resource management from users and applications, providing a seamless computing experience.
    -   Scalability: Distributed operating systems can scale horizontally by adding more nodes to the network, allowing for increased computing power and resource availability.
    -   Fault tolerance: Distributed operating systems are designed to withstand failures in individual nodes or network components, ensuring continued operation and data integrity.
-   **Examples**: Distributed operating systems include Google's Kubernetes, Microsoft's Windows Distributed File System (DFS), and the Apache Hadoop distributed file system (HDFS).
-  **Real-time Operating System (RTOS)**:

-   **Definition**: A real-time operating system is a type of operating system that guarantees a deterministic response time for processing tasks, ensuring that critical tasks are completed within predefined deadlines.
-   **Objective**: The primary goal of a real-time operating system is to provide timely and predictable responses to external events or stimuli, making it suitable for applications with stringent timing requirements.
-   **Characteristics**:
    -   Determinism: Real-time operating systems prioritize tasks based on their deadlines, ensuring that critical tasks are executed within specified time constraints.
    -   Low latency: Real-time operating systems minimize processing delays and overhead, allowing tasks to respond quickly to external events.
    -   Predictability: Real-time operating systems provide predictable performance under varying workloads and system conditions, enabling accurate timing analysis and scheduling.
-   **Types**:
    -   Hard real-time: In hard real-time systems, missing task deadlines can lead to system failure or unacceptable consequences. Examples include control systems for aircraft and medical devices.
    -   Soft real-time: In soft real-time systems, missing task deadlines may degrade system performance but do not result in catastrophic failure. Examples include multimedia streaming and video games.
-   **Examples**: Real-time operating systems include VxWorks, FreeRTOS, and QNX Neutrino, which are commonly used in embedded systems, industrial automation, and mission-critical applications.
In ummary, distributed operating systems manage resources and coordinate communication between multiple computers interconnected via a network, while real-time operating systems guarantee deterministic response times for processing tasks, making them suitable for applications with stringent timing requirements.
## 6. Draw and explain working of System call?

**System Call**

A system call is a method for a computer program to request a service from the kernel of the  [operating system](https://www.javatpoint.com/os-tutorial)  on which it is running. A system call is a method of interacting with the operating system via programs. A system call is a request from computer software to an operating system's kernel.

The  **Application Program Interface (API)**  connects the operating system's functions to user programs. It acts as a link between the operating system and a process, allowing user-level programs to request operating system services. The kernel system can only be accessed using system calls. System calls are required for any programs that use resources.

There are various examples of Windows and Unix system calls. These are as listed below in the table:

| Process              | Windows                          | Unix                         |
|----------------------|----------------------------------|------------------------------|
| Process Control      | CreateProcess()                  | Fork()                       |
|                      | ExitProcess()                    | Exit()                       |
|                      | WaitForSingleObject()            | Wait()                       |
| File Manipulation    | CreateFile()                     | Open()                       |
|                      | ReadFile()                       | Read()                       |
|                      | WriteFile()                      | Write()                      |
|                      | CloseHandle()                    | Close()                      |
| Device Management    | SetConsoleMode()                 | Ioctl()                      |
|                      | ReadConsole()                    | Read()                       |
|                      | WriteConsole()                   | Write()                      |
| Information Maintenance | GetCurrentProcessID()          | Getpid()                     |
|                      | SetTimer()                       | Alarm()                      |
|                      | Sleep()                          | Sleep()                      |
| Communication        | CreatePipe()                     | Pipe()                       |
|                      | CreateFileMapping()              | Shmget()                     |
|                      | MapViewOfFile()                  | Mmap()                       |
| Protection           | SetFileSecurity()                | Chmod()                      |
|                      | InitializeSecurityDescriptor()   | Umask()                      |
|                      | SetSecurityDescriptorgroup()     | Chown()                      |

**Types of System Calls**

Process Control
Process control is the system call that is used to direct the processes. Some process control examples include creating, load, abort, end, execute, process, terminate the process, etc.

File Management
File management is a system call that is used to handle the files. Some file management examples include creating files, delete files, open, close, read, write, etc.

Device Management
Device management is a system call that is used to deal with devices. Some examples of device management include read, device, write, get device attributes, release device, etc.

Information Maintenance
Information maintenance is a system call that is used to maintain information. There are some examples of information maintenance, including getting system data, set time or date, get time or date, set system data, etc.

Communication
Communication is a system call that is used for communication. There are some examples of communication, including create, delete communication connections, send, receive messages, etc.

## 7. List out and explain types of system calls?

System calls are functions provided by the operating system that allow applications to request services from the operating system's kernel. There are several types of system calls, including:

1. **Process Control**:
   - These system calls are used to manage processes, such as creating or terminating processes, waiting for process termination, and getting or setting process attributes.

2. **File Management**:
   - These system calls are used to manage files and directories, including opening, closing, reading from, writing to, and manipulating file attributes.

3. **Device Management**:
   - These system calls control devices connected to the system, such as reading from or writing to devices, requesting device status, or controlling device operations.

4. **Information Maintenance**:
   - These system calls provide information about the system or processes, such as getting or setting the system time, querying system or process attributes, or getting system configuration information.

5. **Communication**:
   - These system calls allow processes to communicate with each other, either within the same system (interprocess communication) or between different systems (network communication).

6. **Memory Management**:
   - These system calls control memory allocation and deallocation, allowing processes to allocate or release memory, map files into memory, or manipulate memory protection settings.

Each type of system call serves a specific purpose and provides a standardized interface for applications to interact with the operating system kernel, abstracting away low-level details and ensuring portability and security.

## 8. Explain user mode and kernel mode?

**User Mode**:
- User mode is the mode in which most applications run. In this mode, applications have limited access to system resources and cannot directly execute privileged instructions or access kernel memory.
- User mode provides a safe environment for applications to run without risking the stability and security of the system. Applications typically interact with the operating system through system calls when they need access to privileged resources or services.

**Kernel Mode**:
- Kernel mode is the privileged mode in which the operating system kernel runs. In this mode, the kernel has full access to system resources and can execute privileged instructions, access hardware devices, and manage system resources directly.
- Kernel mode provides the necessary privileges for the operating system to perform critical system functions, such as process management, memory management, and device I/O operations.

**Key Differences**:
- Access to Resources: User mode applications have restricted access to system resources and must request access through system calls, while the kernel has unrestricted access to all system resources.
- Privileged Instructions: User mode cannot execute privileged instructions directly, while kernel mode can execute privileged instructions that control hardware and system behavior.
- Protection: User mode provides isolation and protection between applications, preventing one application from affecting the stability or security of other applications or the system, while kernel mode has full control over system resources and can enforce protection mechanisms.

## 9. Compare user mode and system mode?

User Mode:
- User mode is the mode in which most applications run.
- Applications in user mode have limited access to system resources.
- User mode provides a safe environment for applications to run without risking the stability and security of the system.
- Applications interact with the operating system through system calls to access privileged resources or services.
- User mode provides isolation between applications, preventing one application from affecting the stability or security of other applications or the system.

System Mode (Kernel Mode):
- System mode, also known as kernel mode, is the privileged mode in which the operating system kernel runs.
- The kernel has full access to system resources and can execute privileged instructions, access hardware devices, and manage system resources directly.
- Kernel mode provides the necessary privileges for the operating system to perform critical system functions, such as process management, memory management, and device I/O operations.
- The kernel enforces protection mechanisms to ensure system stability and security, controlling access to system resources and preventing unauthorized actions.
- System mode is responsible for managing system-wide resources and providing essential services to user mode applications.

In summary, user mode is the mode in which applications run with limited access to system resources, while system mode (kernel mode) is the privileged mode in which the operating system kernel runs, with full access to system resources and control over system behavior.

## 10. Draw and explain the process life cycle or process state diagram ?

Process States
State Diagram

![OS Process State Diagram](https://static.javatpoint.com/operating-system/images/os-process-state-diagram.png)

The process, from its creation to completion, passes through various states. The minimum number of states is five.

The names of the states are not standardized although the process may be in one of the following states during execution.

1. New
A program which is going to be picked up by the OS into the main memory is called a new process.

2. Ready
Whenever a process is created, it directly enters in the ready state, in which, it waits for the CPU to be assigned. The OS picks the new processes from the secondary memory and put all of them in the main memory.

The processes which are ready for the execution and reside in the main memory are called ready state processes. There can be many processes present in the ready state.

3. Running
One of the processes from the ready state will be chosen by the OS depending upon the scheduling algorithm. Hence, if we have only one CPU in our system, the number of running processes for a particular time will always be one. If we have n processors in the system then we can have n processes running simultaneously.

4. Block or wait
From the Running state, a process can make the transition to the block or wait state depending upon the scheduling algorithm or the intrinsic behavior of the process.

When a process waits for a certain resource to be assigned or for the input from the user then the OS move this process to the block or wait state and assigns the CPU to the other processes.

5. Completion or termination
When a process finishes its execution, it comes in the termination state. All the context of the process (Process Control Block) will also be deleted the process will be terminated by the Operating system.

6. Suspend ready
A process in the ready state, which is moved to secondary memory from the main memory due to lack of the resources (mainly primary memory) is called in the suspend ready state.

If the main memory is full and a higher priority process comes for the execution then the OS have to make the room for the process in the main memory by throwing the lower priority process out into the secondary memory. The suspend ready processes remain in the secondary memory until the main memory gets available.

7. Suspend wait
Instead of removing the process from the ready queue, it's better to remove the blocked process which is waiting for some resources in the main memory. Since it is already waiting for some resource to get available hence it is better if it waits in the secondary memory and make room for the higher priority process. These processes complete their execution once the main memory gets available and their wait is finished.



## 11. Draw process control block and explain in detail ?

Process Control Block is a data structure that contains information of the process related to it. The process control block is also known as a task control block, entry of the process table, etc.

It is very important for process management as the data structuring for processes is done in terms of the PCB. It also defines the current state of the operating system.

Structure of the Process Control Block
The process control stores many data items that are needed for efficient process management. Some of these data items are explained with the help of the given diagram −

![Process Control Block in Operating System](https://www.tutorialspoint.com/assets/questions/media/12231/PCB%20in%20Operating%20System.png)


The following are the data items −

Process State
This specifies the process state i.e. new, ready, running, waiting or terminated.

Process Number
This shows the number of the particular process.

Program Counter
This contains the address of the next instruction that needs to be executed in the process.

Registers
This specifies the registers that are used by the process. They may include accumulators, index registers, stack pointers, general purpose registers etc.

List of Open Files
These are the different files that are associated with the process

CPU Scheduling Information
The process priority, pointers to scheduling queues etc. is the CPU scheduling information that is contained in the PCB. This may also include any other scheduling parameters.

Memory Management Information
The memory management information includes the page tables or the segment tables depending on the memory system used. It also contains the value of the base registers, limit registers etc.

I/O Status Information
This information includes the list of I/O devices used by the process, the list of files etc.

Accounting information
The time limits, account numbers, amount of CPU used, process numbers etc. are all a part of the PCB accounting information.

## 12. Explain process Switching?

Process switching is the mechanism by which the operating system switches the CPU from one process to another. This switching allows multiple processes to share the CPU's execution time, enabling multitasking and concurrent execution of multiple programs. Here's how process switching works:

1. **Interrupt Handling**: Process switching typically begins with an interrupt or an exception. Interrupts can be generated by hardware devices, such as a timer interrupt indicating the end of a time slice, or by software, such as a system call requesting a service from the operating system.

2. **Context Switching**: When an interrupt occurs, the CPU saves the context of the currently executing process, including its program counter, register values, and other relevant state information, onto the process's stack or control block.

3. **Scheduling**: The operating system's scheduler selects the next process to execute based on scheduling algorithms and policies. This decision may consider factors such as process priority, CPU burst duration, and system load.

4. **Loading New Process**: Once the next process is selected, the operating system loads the saved context of the selected process from its control block or process table into the CPU registers, preparing it for execution.

5. **Execution**: The CPU resumes execution of the selected process from the point where it was interrupted, allowing the process to continue executing until it completes its quantum, encounters a blocking condition, or is preempted by another process.

6. **Repeat**: The process of switching between processes continues as long as there are runnable processes in the system and the CPU scheduler determines that a context switch is necessary.

Process switching is a fundamental operation in multitasking operating systems, enabling efficient sharing of CPU resources among multiple processes and providing users with the illusion of concurrent execution of multiple programs.

## 13. Draw Queuing diagram and explain it?

Process Queues
The Operating system manages various types of queues for each of the process states. The PCB related to the process is also stored in the queue of the same state. If the Process is moved from one state to another state then its PCB is also unlinked from the corresponding queue and added to the other state queue in which the transition is made.

![Process Queues](https://static.javatpoint.com/operating-system/images/process-queues.png)

There are the following queues maintained by the Operating system.

1. Job Queue
In starting, all the processes get stored in the job queue. It is maintained in the secondary memory. The long term scheduler (Job scheduler) picks some of the jobs and put them in the primary memory.

2. Ready Queue
Ready queue is maintained in primary memory. The short term scheduler picks the job from the ready queue and dispatch to the CPU for the execution.

3. Waiting Queue
When the process needs some IO operation in order to complete its execution, OS changes the state of the process from running to waiting. The context (PCB) associated with the process gets stored on the waiting queue which will be used by the Processor when the process finishes the IO.

## 14.	Draw and explain mid-term scheduler?	

The long-term execution of processes in a computer system is managed by a medium-term scheduler, also referred to as a mid-term scheduler. Based on a set of predetermined criteria and priorities, this kind of scheduler decides which processes should be executed next.

Typically, processes that are blocked or waiting must be managed by the medium-term scheduler. These processes are not running right now, but they are still awaiting the occurrence of an event in order to start running. Which of these blocked processes should be unblocked and allowed to continue running is up to the medium-term scheduler to decide.

The system’s overall resource utilization must be managed via the medium-term scheduler. This entails keeping track of how much memory, CPU, and other resources are being used by the various processes and modifying resource allocation as needed.

The operating system kernel often houses the medium-term scheduler’s implementation. It is in charge of controlling the system’s overall resource utilization as well as the scheduling of programs that are stalled or waiting.

![Medium Term Scheduler in Operating System](https://media.geeksforgeeks.org/wp-content/uploads/20200705221657/MRT.png)

Responsibilities of Medium Term Scheduler
The medium-term scheduler’s responsibility for ensuring equitable resource distribution among all processes is one of its main responsibilities. This is necessary to guarantee that every process has an equal chance to run and prevent any one process from using up all of the system resources.
The medium-term scheduler’s responsibility for ensuring effective process execution is another crucial task. This may entail modifying the priority of processes based on their present condition or resource utilization, or modifying the resource distribution to various processes based on their present requirements.
So, the operating system’s medium-term scheduler controls the scheduling and resource distribution of processes that are blocked or waiting. It aids in ensuring that resources are distributed equally throughout all of the processes and that they are carried out effectively.

## 15. Compare process and program?


| Parameters         | Program                                                                                  | Process                                                                              |
|--------------------|------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------|
| Definition         | A Program is an organized set of operations designed to accomplish a specific objective. | A Process is the active execution of a program.                                     |
| Resource Management| A Program uses only its memory for storage.                                              | A Process requires substantial resources.                                           |
| Nature             | A program is inherently passive and will not function until executed.                     | A process is an instance of a program being executed.                                |
| Overheads          | A Program does not incur significant overhead.                                           | A Process incurs substantial overhead.                                              |
| Creation           | A new program can be created independently, without the need to duplicate an existing one.| The creation of a new process necessitates the duplication of the parent process.    |
| Lifespan           | A Program has a relatively long lifespan as it is stored in memory and can only be deleted manually.| A Process has a short lifespan, as it ends once the task is completed.            |
| Resources Required | A Program does not require resources as it is saved on disk files.                        | A Process uses resources such as memory address, I/O, disk, CPU, printer, etc.     |
| Entity Type        | A Program is a static or passive entity found on a computer's secondary memory.          | A Process is a dynamic or active entity found on a computer's primary memory.       |
| Control Block      | There is no control block for Programs.                                                  | A Process has its own control block, known as the Process Control Block.            |

##  16.	Compare process and thread?	


| S.NO | Process Description                                        | Thread Description                                                                                    |
|------|-----------------------------------------------------------|------------------------------------------------------------------------------------------------------|
| 1.   | Process means any program is in execution.                | Thread means a segment of a process.                                                                 |
| 2.   | The process takes more time to terminate.                 | The thread takes less time to terminate.                                                             |
| 3.   | It takes more time for creation.                           | It takes less time for creation.                                                                     |
| 4.   | It also takes more time for context switching.            | It takes less time for context switching.                                                            |
| 5.   | The process is less efficient in terms of communication.  | Thread is more efficient in terms of communication.                                                  |
| 6.   | Multiprogramming holds the concepts of multi-process.     | We don’t need multi programs in action for multiple threads because a single process consists of multiple threads. |
| 7.   | The process is isolated.                                  | Threads share memory.                                                                                 |
| 8.   | The process is called the heavyweight process.           | A Thread is lightweight as each thread in a process shares code, data, and resources.                 |
| 9.   | Process switching uses an interface in an operating system. | Thread switching does not require calling an operating system and causes an interrupt to the kernel. |
| 10.  | If one process is blocked then it will not affect the execution of other processes. | If a user-level thread is blocked, then all other user-level threads are blocked. |
| 11.  | The process has its own Process Control Block, Stack, and Address Space. | Thread has Parents’ PCB, its own Thread Control Block, and Stack and common Address space. |
| 12.  | Changes to the parent process do not affect child processes. | Since all threads of the same process share address space and other resources so any changes to the main thread may affect the behavior of the other threads of the process. |
| 13.  | A system call is involved in it.                         | No system call is involved, it is created using APIs.                                                 |
| 14.  | The process does not share data with each other.          | Threads share data with each other.                                                                  |

## 17.Draw and explain working of single and multi-threaded model?	

A thread is a light weight process which is similar to a process where every process can have one or more threads. Each thread contains a Stack and a Thread Control Block. There are four basic thread models : 

1. User Level Single Thread Model : 
 
    - Each process contains a single thread.
    - Single process is itself a single thread.
    - process table contains an entry for every process by maintaining its PCB.
    
    ![](https://media.geeksforgeeks.org/wp-content/uploads/20200624084814/1-1-2.png)

2. User Level Multi Thread Model : 
 
    - Each process contains multiple threads.
    - All threads of the process are scheduled by a thread library at user level.
    - Thread switching can be done faster than process switching.
    - Thread switching is independent of operating system which can be done within a process.
    - Blocking one thread makes blocking of entire process.
    - Thread table maintains Thread Control Block of each thread of a process.
    - Thread scheduling happens within a process and not known to Kernel.
    
    ![](https://media.geeksforgeeks.org/wp-content/uploads/20200624084840/2-245-1.png)

3. Kernel Level Single Thread Model : 
 
    - Each process contains a single thread.
    - Thread used here is kernel level thread.
    - Process table works as thread table.
    
    ![](https://media.geeksforgeeks.org/wp-content/uploads/20200624084918/3-1100.png)

4. Kernel Level Multi Thread Model : 
 
    - Thread scheduling is done at kernel level.
    - Fine grain scheduling is done on a thread basis.
    - If a thread blocks, another thread can be scheduled without blocking the whole process.
    - Thread scheduling at Kernel process is slower compared to user level thread scheduling.
    - Thread switching involves switch.
    
    ![](https://media.geeksforgeeks.org/wp-content/uploads/20200624084952/4108-2.png)

Sure, let's address each question one by one:

## 18. List out and explain multi-threaded model?

**Multi-threaded Model**:

- In a multi-threaded model, a process is divided into multiple threads of execution, each capable of running independently.
- Threads within the same process share the same memory space, allowing them to access shared data and resources directly.
- Multi-threading enables concurrent execution of multiple tasks within a single process, improving efficiency and responsiveness.
- Threads can communicate with each other through shared memory or synchronization mechanisms provided by the operating system.

**Advantages of Multi-threaded Model**:

1. Improved Responsiveness: Multi-threading allows applications to remain responsive even while performing CPU-intensive tasks by utilizing multiple threads.
2. Enhanced Resource Utilization: Threads within the same process can share resources efficiently, reducing overhead and improving overall system performance.
3. Simplified Programming Model: Multi-threading simplifies programming by allowing developers to parallelize tasks within a single process, avoiding the complexities of inter-process communication.
4. Enhanced Scalability: Multi-threading enables applications to scale across multiple CPU cores, leveraging parallelism to improve throughput and scalability.

**Example**:

Consider a web server application. In a multi-threaded model, the server can create a separate thread for each incoming client connection. Each thread handles the client's requests independently, allowing the server to serve multiple clients concurrently without blocking other clients.

## 19. Explain FCFS and SJF CPU scheduling algorithm with example?

**FCFS (First-Come, First-Served)**:

- In FCFS scheduling, processes are executed in the order they arrive in the ready queue.
- It is a non-preemptive scheduling algorithm, meaning once a process starts executing, it continues until it completes or enters the waiting state.
- Example:
  - Consider three processes arriving in the order P1, P2, and P3, with burst times of 10, 5, and 8 milliseconds, respectively.
  - The scheduling order would be P1, P2, and P3, and the average waiting time would be ((0 + 10) + (10 + 5) + (10 + 5 + 8)) / 3 = 32/3 milliseconds.

**SJF (Shortest Job First)**:

- In SJF scheduling, the process with the shortest burst time is selected for execution next.
- It is a non-preemptive or preemptive scheduling algorithm, depending on whether new shorter jobs can preempt currently running jobs.
- Example:
  - Consider three processes with burst times of 6, 3, and 8 milliseconds, respectively.
  - The scheduling order would be P2, P1, and P3, and the average waiting time would be ((0 + 3) + (3 + 6) + (3 + 6 + 8)) / 3 = 25/3 milliseconds.

## 20. Solve FCFS and SJF CPU scheduling algorithm for given example?

**FCFS Example**:

- Given Processes: P1, P2, P3
- Burst Times: 10, 5, 8 milliseconds respectively
- FCFS Scheduling:
  - P1 starts at time 0, completes at time 10
  - P2 starts at time 10, completes at time 15
  - P3 starts at time 15, completes at time 23
- Average Waiting Time: ((0 + 10) + (10 + 5) + (10 + 5 + 8)) / 3 = 32/3 milliseconds.

**SJF Example**:

- Given Processes: P1, P2, P3
- Burst Times: 6, 3, 8 milliseconds respectively
- SJF Scheduling:
  - P2 starts at time 0, completes at time 3
  - P1 starts at time 3, completes at time 9
  - P3 starts at time 9, completes at time 17
- Average Waiting Time: ((0 + 3) + (3 + 6) + (3 + 6 + 8)) / 3 = 25/3 milliseconds.

## 21. Explain Priority and Round Robin CPU scheduling algorithm with example?

**Priority Scheduling**:

- Priority scheduling assigns priorities to processes and selects the process with the highest priority for execution.
- It can be either preemptive or non-preemptive, where higher priority processes can preempt lower priority ones.
- Example:
- Consider three processes with priorities P1 (high), P2 (medium), and P3 (low).
- The scheduling order would be P1, P2, and P3, assuming P1 has the highest priority.

**Round Robin Scheduling**:

- Round Robin scheduling allocates a fixed time slice (quantum) to each process in a circular manner.
- If a process doesn't complete within its time slice, it's preempted and placed back in the ready queue.
- Example:
- Consider three processes with time slices of 10 milliseconds each.
- Each process gets 10 milliseconds of CPU time before being preempted and placed back in the ready queue.

