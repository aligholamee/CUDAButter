# Occupancy

Some key points about occupancy in CUDA.

### Definition

Occupancy is the **number of active warps** divided by **maximum number of active warps**.
*   Since resources are allocated for the **entire block** and resources are **limited**, utilizing too many resources per thread may limit the occupancy.

### Occupancy Limiters

*   Register Usage
*   Shared Memory Usage
*   Block Size

### Register Usage Limitation

#### Example 1

*   There are 32K registers available per SM.
*   There are maximum number of 1560 threads per SM.
*   Kernel uses 20 registers per thread.
*   Thus, the number of active threads are 32K/20 = 1560.
*   Thus, the occupancy is 1560/1560 = 1.




