For the next few questions,
assume the page size is 32 bytes
and that there is at least one free frame on the system.
Consider the following page table that includes a valid bit:

```
010  0
000  1
110  0
111  1
```

1. Give an example of a *page* access that will generate a page fault.

2. Give an example of a *memory* request from the process that will generate a
   page fault.
   (You need to be able to answer the previous question to answer this one.)

3. How much data is transferred between disk and memory when a page fault
   occurs in this scenario?

4. If a process accesses page 3 (0-indexed),
   does the operating system get involved?
   Why or why not?

5. When a process is allocated an additional frame,
   the frame is filled with zeros.
   What could go wrong if this were not the case?

For the next few questions,
consider a system with a page size of 4 KB.
Assume the disk has a bandwidth of 1 KB / second
and that memory has a bandwidth of 10 MB / second.

6. What is the time required to service a page fault?
   You may assume the only cost of a page fault is disk I/O
   (i.e., you may ignore the cost of a context switch, updating memory, etc.).

7. How long does a memory access take assuming the program requests 1 byte of
   memory?

8. What is the maximum page fault rate the system can have while maintaining
   an effective memory access rate of 105 nanoseconds?

9. Consider question (3) above.
   How would the answer change,
   if at all,
   if we removed the assumption that there were free frames available in the
   system?
