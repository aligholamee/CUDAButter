# Occupancy
Some key points about occupancy in CUDA.

### Definition
Occupancy is the **number of actice warps** divided by **maximum number of active warps**.
*   Since resources are allocated for the **entire block** and resources are **limited**, utilizing too many resources per thread may limit the occupancy.

### Occupancy Limiters
*   Register Usage
*   Shared Memory Usage
*   Block Size

