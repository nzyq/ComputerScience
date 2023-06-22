## Cache Memory

CPU handles data and instructions much faster than they been read from or written to the Dynamic Random Access Memory(DRAM)

### DRAM and SRAM
Cache memory is CPU internal memory that can be accessed very quickly by the CPU and they also retain their contents as long as they are supplied with power which is why this type of memory is known as ===Static RAM(SRAM)===. On the other hand the ===Dynamic RAM(DRAM)=== uses capacitors to store data and instructions and those capacitors leak their charge very quickly and therefore need to constantly and dynamically refresh with electricity in order for them to store data.

### Instruction Fetch Process

SRAM stores data and instructions from DRAM that is waiting to be used by the CPU over and over again. When CPU needs certain data it always checks for hit from the faster memory first.

Suppose the CPU wants to retrieve a program instruction from memory, the memory address of the next instruction to be fetch is stored in a register called Program Counter(PC, for further details on [[Fetch and Execute Cycle]], the CPU checks the level 1 instruction cache first, if it is what it is looking for it is call a cache hit and the instruction is copied into one of the CPU's registers, in the event of level 1 cache miss the level 2 cache is checked, if this is successful the instruction is copied to the level 1 cache and then into one of the CPU's registers. If there is a level 2 cache miss, the level 3 cache is checked, if results in a hit the instruction is copied into level 2 cache and level 1 cache and then the CPU register. Only if there is a level 3 cache miss, the processor goes to DRAM via the memory bus, the requested instruction is then propagated back through the various levels of cache to the CPU.
![[Pasted image 20221028205024.png]]

Program instructions and data are never retrieved or saved individually, the cache memory is divided into cache lines with each line typically contains 64 bytes[[Unit of measurement for storage data]]. During a data and instruction transfer, the entire cache line is read or written in one go even if the whole line is not needed.

Ex. When level 1 cache is full then the entire cache line is copied to the level 2 cache, finally if necessary the entire cache line will be copied to the DRAM.

