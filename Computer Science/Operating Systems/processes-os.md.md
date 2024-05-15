Path : [/Computer Science](<..\..\index.md>) [/Operating Systems](<..\index.md>)
## Processes in Operating Systems

### Introduction

A process is a collection of instructions in a specific state, being executed by a computer system. It represents a running program that performs a specific task. Each process has its own memory space, files, and I/O devices.

**Process Management**

Process management is a set of techniques and algorithms used to:

- **Create processes:** Defining and initiating the execution of new processes. 
- **Manage processes:** Monitoring, controlling, and scheduling processes for efficient resource utilization.
- **Terminate processes:** Ending the execution of processes and reclaiming their resources.


### Process States

A process exists in different states during its lifecycle:

**1. New:** Created but not yet started.
**2. Ready:** Waiting to be assigned to a CPU.
**3. Running:** Executing / utilizing CPU resources.
**4. Waiting:** Blocked while waiting for resources, such as I/O devices.
**5. Terminated:** Execution completed or terminated due to an error.


### Process Control Block (PCB)

Every process has a Process Control Block (PCB), which contains information necessary for managing the process. This includes:

- Program address & memory space
- Status & state
- Open files & I/O devices
- CPU registers & scheduling information


### Process Scheduling

Process scheduling is the mechanism to allocate the CPU to processes. Different scheduling algorithms are used to decide which process to run when multiple processes are ready. 

**Common Scheduling Algorithms:**

- **FCFS (First Come First Serve)**: Processes are executed in the order they arrive.
- **SJF (Shortest Job First)**: Processes are executed based on their execution time.
- **Round Robin**: Equal time slices are allocated to each process in turn.


### Process Synchronization

When multiple processes access shared resources, synchronization is needed to prevent conflicts. 

**Synchronization Mechanisms:**

- **Mutexes:** Ensure exclusive access to shared resources.
- **Semaphores:** Count the number of available shared resources.
- **Critical Sections:** Code segments protected by a lock.


### Conclusion

Processes are fundamental entities in operating systems. Understanding process management concepts is crucial for efficient resource utilization and achieving optimal performance in multi-tasking environments.
