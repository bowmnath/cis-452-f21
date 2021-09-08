## Welcome to CIS 452!

This is the main website for the course.
The slides, schedule, and links to assignments, labs, and projects,
as well as the official course policies,
will be posted here.
The course also uses other websites for specific purposes.
* [Piazza](http://www.piazza.com) is a question-and-answer forum.
*All official announcements will be sent through Piazza*,
and you are responsible for monitoring Piazza to keep up to date with
announcements
(Piazza by default will send an email when an announcement is posted).
    * Signup link:
      [www.piazza.com/gvsu/fall2021/cis452](http://www.piazza.com/gvsu/fall2021/cis452).
    * You can read the following [Piazza FAQ](misc/piazza-faq.md) if you have
      questions.
* [Zoom](https://zoom.us) will be the video conferencing service for online
  office hours (more about that in the [syllabus](syllabus.md)).
    * Office hours link (Wednesdays only):
      [https://gvsu-edu.zoom.us/j/98637553783?pwd=RzJsazNrcDhFemFRTCtvN2xiblFnUT09](https://gvsu-edu.zoom.us/j/98637553783?pwd=RzJsazNrcDhFemFRTCtvN2xiblFnUT09)
* [Prairielearn](https://prairielearn.engr.illinois.edu/pl/) is where you will
submit all of your assignments, labs, and projects.

That seems like a lot to monitor,
but don't worry -- you really need only actively follow Piazza.
I will release announcements there any time assignments are posted,
and I will post links to them directly on this page.

Be sure to read through the [syllabus](syllabus.md) for course policies,
contact information, and other important info.

Because the course was previously taught online,
there are lecture videos at the previous course website
([https://github.com/bowmnath/cis-452-f20](https://github.com/bowmnath/cis-452-f20))
that you are welcome to use to review the material.
I would not suggest using these as a substitute for coming to class
because the coverage will change slightly from semester to semester
and because we will be doing activities in class to reinforce understanding
of the concepts.

## Schedule

** Note: This is an estimated timeline and subject to change. **

| Week | Topics | Readings and Activities | Deliverables |
| ---- | ------ | ----------------------- | ------------ |
|  1   | Introduction <br>([slides](slides/what-is-os.pdf)) <br> Multiprogramming motivation <br>([slides](slides/multiprogramming-basic.pdf)) <br> Interrups <br>([slides](slides/interrupts.pdf)) <br> System calls <br>([slides](slides/system-calls.pdf))  | Chapter 1<br> Chapter 2 | **Wednesday 9/1 @ 5PM** [Partner survey](https://forms.gle/eu6q5wxQcTNTFRq9A)<br>**Friday 9/3** [Syllabus quiz](https://www.prairielearn.org/pl/course_instance/128860/assessment/2313420) |
|  2   | Process concepts <br>([slides](slides/process-intro.pdf)) <br> Process scheduling <br>([slides](slides/process-scheduling.pdf)) <br> Process lifecycle <br>([slides](slides/process-lifecycle.pdf))  | 3.1 - 3.3 | **Wednesday 9/8** Lab 1 due<br> |
|  3   | Interprocess communication<br> ([IPC slides](slides/process-ipc.pdf))  <br>([POSIX shared mem slides](slides/process-shm-posix.pdf))  <br>([Message passing slides](slides/process-message.pdf))  <br>([Pipes slides](slides/process-pipes.pdf))  <br> Threads <br>([Thread overview slides](slides/thread-overview.pdf))  <br>([Thread models slides](slides/thread-models.pdf))  <br>([Thread issues slides](slides/thread-issues.pdf))  | Chapter 3<br> Chapter 4 | **Monday 9/13** [HW Chapters 1 & 2](https://www.prairielearn.org/pl/course_instance/128860/assessment/2313584) due <br>**Wednesday 9/15** [Project 1](https://www.prairielearn.org/pl/course_instance/128860/assessment/2313556) due<br>**Wednesday 9/15** [Lab 2](https://www.prairielearn.org/pl/course_instance/128860/assessment/2313666) due |
|  4   | Process synchronization <br>([slides](slides/parallel-intro.pdf)) <br> Syncrhonization algorithms <br>([slides](slides/parallel-critical-section.pdf)) <br> File descriptors <br> ([slides](slides/file-descriptors.pdf))  | 5.1 - 5.3 | **Wednesday 9/22** Lab 3 due |
|  5   | Synchronization hardware <br>([slides](slides/sync-hardware.pdf))  <br> Mutex and Semaphores <br>([mutex slides](slides/sync-mutex.pdf))  <br>([semaphore slides](slides/sync-semaphore.pdf))  <br>([issues slides](slides/sync-issues.pdf))  <br> Classic problems of synchronization <br>([slides 1](slides/sync-classic.pdf))  <br>([slides 2](slides/sync-philosophers.pdf))  | 5.4 - 5.7 | **Wednesday 9/29** Lab 4 due |
|  6   | Monitors <br>([intro slides](slides/sync-monitor-intro.pdf))  <br>([usage slides](slides/sync-monitor-philosophers.pdf))  <br>([implementation slides](slides/sync-monitor-implementation.pdf))  <br> Deadlock <br>([deadlock criteria slides](slides/sync-deadlock-intro.pdf))  <br>([graphs slides](slides/sync-deadlock-graph.pdf))  | 5.8, 5.11 | **Tuesday 10/5** Project 2 due<br>**Wednesday 10/6** Lab 5 due |
|  7   | CPU scheduling concepts<br> ([concepts slides](slides/scheduling-concepts.pdf)) <br> Scheduling criteria and metrics<br> ([criteria slides](slides/scheduling-criteria.pdf))  <br> FCFS Scheduling<br> ([fcfs slides](slides/scheduling-fcfs.pdf))  | 6.1 - 6.2 | **Wednesday 10/13** Lab 6 due |
|  8   | Scheduling algorithms<br> ([SJF slides](slides/scheduling-sjf.pdf)) <br> ([Burst time slides](slides/scheduling-bursts.pdf)) <br> ([Priority slides](slides/scheduling-priority.pdf)) <br> ([Round-robin slides](slides/scheduling-rr.pdf)) <br> ([Multilevel queue slides](slides/scheduling-multilevel.pdf)) <br> ([Feedback queue slides](slides/scheduling-feedback.pdf)) <br> ([Thread and multiprocessor slides](slides/scheduling-threads.pdf))  | 6.3 - 6.5 | **Wednesday 10/20** Lab 7 due |
|  9   | Memory management<br> ([Memory intro slides](slides/memory-intro.pdf))<br> ([Virtual addresses slides](slides/memory-addresses.pdf))<br> ([Linking and Loading slides](slides/memory-loading-linking.pdf))<br> ([Swapping slides](slides/memory-swapping.pdf)) <br> ([Contiguous allocation slides](slides/memory-contiguous.pdf))<br> ([Fragmentation slides](slides/memory-fragmentation.pdf))  | 7.1 - 7.3 | **Tuesday 10/26** Project 3 due<br>**Midterm Exam** **Thursday October 28 (during lab)** |
|  10  | Segmentation<br> ([slides](slides/memory-segmentation.pdf))<br> Paging<br> ([intro slides](slides/paging-intro.pdf))<br> ([details slides](slides/paging-details.pdf))<br> ([TLB slides](slides/paging-tlb.pdf))<br> ([table structure slides](slides/paging-table.pdf)) | 7.4 - 7.6 | |
|  11  | Virtual memory<br> ([Intro slides](slides/virtual-intro.pdf))<br> ([Demand Paging slides](slides/virtual-demand-paging.pdf))<br>([Copy-on-Write slides](slides/virtual-copy-on-write.pdf))<br> Memory performance<br>([Performance slides](slides/virtual-access-time.pdf))<br> Page replacement concepts<br>([Replacement slides](slides/virtual-replacement.pdf))<br> Page replacement algorithms<br>([FIFO slides](slides/virtual-fifo.pdf)) <br>([OPT and LRU slides](slides/virtual-opt-lru.pdf)) <br>LRU Implementation<br>([Implementation slides](slides/virtual-lru-implement.pdf)) <br>([LRU approximation (more bits) slides](slides/virtual-lru-more-bits.pdf)) <br>([LRU approximation (second chance) slides](slides/virtual-lru-second-chance.pdf))<br>Page Buffering<br>([slides](slides/virtual-page-buffering.pdf)) | 8.1 - 8.4 | **Wednesday 11/10** Lab 8 due<br> |
|  12  | Frame allocation<br> ([slides](slides/virtual-frame-allocation.pdf))<br> Thrashing<br> ([Thrashing slides](slides/virtual-thrashing.pdf))<br>([Thrashing Avoidance slides](slides/virtual-models.pdf))<br>Memory mapping<br> ([slides](slides/virtual-mmap-files.pdf)) | 8.5 - 8.10 | **Wednesday 11/17** Lab 9 due<br> |
|      | Virtual Memory Misc.<br> ([slides](slides/virtual-misc.pdf))<br>Thanksgiving break 11/25 - 11/29 | | |
|  14  | File system concepts<br>([files slides](slides/storage-files.pdf))<br>([directories slides](slides/storage-directories.pdf))<br>([links slides](slides/storage-links.pdf))<br>([directory implementation slides](slides/storage-implement-directories.pdf))<br>File system allocation<br>([contiguous allocation slides](slides/storage-allocation-contiguous.pdf))<br>([linked allocation slides](slides/storage-allocation-linked.pdf))<br>([indexed allocation slides](slides/storage-allocation-index.pdf)) | Chapter 10<br>Chapter 11<br>Chapter 9 |**Wednesday 12/01** Lab 10 due |
|  15  | Hard Disks<br>([hard disks slides](slides/storage-disk.pdf))<br>([disk scheduling slides](slides/storage-scheduling.pdf))<br>Protection and security<br>([protection slides](slides/security-protection.pdf))<br>([security slides](slides/security-security.pdf)) | Chapter 13<br>Chapter 14 | **Wednesday 12/08** Lab 11 due |
|  16  | **Final Exam** **Monday, December 13, 12pm - 1:50pm** | | **Sunday, 12/12** Project 4 due |

## Other helpful links

[cislab.hpc.gvsu.edu](https://cislab.hpc.gvsu.edu) --
Remote access to EOS.
Does not require VPN connection.
