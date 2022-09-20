# **COSC 80 - Reporting / Notes**

## **What are Processes?**

**Programs** - Programs are Passive entities in a computer, they are called passive entities because a program can sit in a computer even though it is not running.

Programming languages like C and C++ can be compiled into machine code, those machines code are sometimes called a binary executable or a **program**.

**Process** - When a program is running or executed it is already called a process, any kind of program be it built-in, installed, or developed using a programming language; as long as it's running on a computer either implicitly at the background or explicitly where the user can see the GUI of that program, it is already a process.

## **Process Scheduling**

Process scheduling is the activity where processes are handled. Examples are when; starting a program, exiting a process, waiting for processes, continuing a process. All of these are part of process scheduling.

Operating systems uses various types of queues to manage process, these queues are:

- Job Queue
- Ready Queue
- Waiting Queue

[![process-queues](./process-queues-diag.jpg)](https://www.tutorialspoint.com/operating_system/os_process_scheduling.htm)


- Job Queues - in most cases the job queue resides in the secondary memory.

    The job queue contains programs that are not allocated yet in the main memory, It waits for the ready queue to be available before pushing processes in to it.

- Ready Queue - The ready queue contains programs that are already allocated in the main memory, they reside in the main memory (which is not always true if the OS uses [Demand Paging](http://en.wikipedia.org/wiki/Demand_paging)), but these processes are not yet running on the CPU.

    The processes here can be in its initial state, or on a partially processed state meaning; the CPU executed them for a some time then was only re-queued back to the ready queue.

- Waiting Queue - This queue contains processes that are waiting for Input or Output events.

    An example of these processes are:
    
    - Built-in processes embedded in the OS that waits for mouse click events and keyboard press events.
    - A C or C++ programs that uses `scanf` or `cin >>` to get inputs.


-----

**sources**
- https://padakuu.com/process-concept-56-article
- https://www.tutorialspoint.com/operating_system/os_process_scheduling.htm
- https://www.javatpoint.com/os-process-queues
- https://www.youtube.com/watch?v=OrM7nZcxXZU&list=PLBlnK6fEyqRgKl0MbI6kbI5ffNt7BF8Fn
- https://www.youtube.com/watch?v=2h3eWaPx8SA
- https://www.youtube.com/watch?v=THqcAa1bbFU