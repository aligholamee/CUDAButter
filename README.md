# CUDAButter
Notes and Best Practices on CUDA Programming with C/C++.

# Basic Concepts

### Grid
A grid is composed of blocks which are completely independent.

### Block
A block is composed of threads which can communicate within their own block.

### Warp
32 threads form a warp.
*   Instructions are issued per warp.
*   If an operand is not ready, then warps are context switched.