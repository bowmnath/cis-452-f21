Consider using an inverted page table *without* hashing.

1. Assume there is just one process running on the system and that the process
   has the following mappings of pages to frames.
   ```
   Page 3 -> Frame 7
   Page 1 -> Frame 2
   Page 2 -> Frame 1
   Page 0 -> Frame 3
   ```
   What does the page table look like?

2. Is it possible to do better than a linear search when looking up a specific
   page in the page table?
   For example, can we find the page/frame mapping we want in logarithmic time
   using a smarter search algorithm?
   Why or why not?

3. Is the following statement true or false:
   The size of the page table is independent of the number of processes running
   on the system.
   Explain.

4. True or false:
   The frame number need not be stored in the page table under this setup.
   Explain.

Next, consider using an inverted page table *with* hashing.

5. In this case,
   does the frame number need to be stored as part of the entry?
   Why or why not?

6. Does each process need a separate page table?
   Explain.

7. Which value do we hash to find the correct row of the table:
   the logical address or the physical address?
   How do you know?
