#flashcards/lowlevel

What is a memory page in OS?
?
A **memory page** is part of how the **operating system** manages and allocates memory for processes (programs). When a program asks for memory (e.g., for variables, arrays, etc.), the OS assigns memory in **fixed-sized chunks**, called **pages**. The size of these pages is typically **4 KB** on most systems.
+++

How does an array use memory?
?
When you create an array, its memory is typically allocated in **contiguous blocks** (meaning the memory for all elements of the array is placed next to each other).
+++

What is the typical block size for filesystems and why does it matter?
?
The typical block size for filesystems (like ext4) and disk sectors is 4 KB. Matching buffer size to the block size ensures fewer I/O operations, faster reads/writes, and improved overall performance.
+++

