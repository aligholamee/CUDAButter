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

#### Context Switching
* **Registers** and **shared memory** are allocated for a block as long as that block is **active**.
*   Once a block is active it will **stay active** until all threads in that block have completed.
*   Context switching is very fast because registers and shared memory do not need to be saved and restored.