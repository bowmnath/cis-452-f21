For the questions below,
consider a page table stored using hashing.
Assume our hash table has 8 entries and we are using modulo
(i.e., "remainder" or `%`) as our "hash" function.

1. Quick check -- which row holds the entry for page 10?

2. What is stored in the entry for page 10?
   (Not the specific value -- we don't know that.
   The general idea.)

3. Given the following mappings of pages to frames,
   what does the page table look like?
   ```
   Page 1 -> Frame 90
   Page 2 -> Frame 43
   Page 6 -> Frame 72
   Page 9 -> Frame 101
   ```

4. Assume the process with the above page table has a logical address space
   large enough to hold 32 pages.
   Furthermore, assume the process is using *only* those pages --
   the others are not in use and therefore do not have physical frames
   associated with them.

   Compared to our standard, forward page table,
   roughly how much memory have we saved by switching to a hash table?
   (Careful -- it might be a slightly smaller savings than you think.)

    You won't be able to get an exact bits or bytes number without more
    information.
    Just consider what is being stored in each setup.

5. How does using a hashing setup affect the *speed* of memory lookups?

6. There is a tradeoff between speed and storage when deciding on the size of
   our hash table.
   Explain why.
