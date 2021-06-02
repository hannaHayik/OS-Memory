# OS-Memory  

Operating Systems 202 Assignment 3  

Goal: Learn how to manage memory in operating systems  
1. Implemented a Paging framework since xv6 considered all of a process's memory pages are in RAM, We implemented a paging system that uses a file on the disk that behaves like
    swap file and every process is limited to 16 memory pages (4096b) to it's RAM and 16 pages to it's swap file, Kind of simulating modern RAM/Disk memory.  
2. Implemented Copy-On-Write to shared memory pages (ex. fork() creates a process with the same pages as the father process).  
3. Implemented Page replacement algorithms (NFU+Aging, LeastAccessedPage+Aging, 2nd chance FIFO, Advancing Queue) to decide which page to replace for situations like: 
    If a process used all of it's 16 pages in RAM and it needs data that resides in a page that is currently in the swap file (on disk) then we need to decide which page to
    evacuate from the RAM to make some room for the needed page  
4. Changed the Ctrl+P command to show more information about the process's status.  
5. Implemented heavy tests (our framework passed them all).  

Extract ZIP file -> Apply PATCH  

**** NOTE: The ZIP file is NOT mine, You can find the original github page here https://github.com/mit-pdos/xv6-public ****
