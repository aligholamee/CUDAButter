# Performance
Here are some key notes on performance.

### Key Points
The main goal here is to hide latency and increase the throughput of the system. There are two major suggestions made here:

*   Running more threads per multiprocessor.
*   Running more threads per thread block.

### Warning
Not always maximizing the **occupancy** yields in a better **performance**. Sometimes increasing the **occupancy** is the cause of **lower performance**.

# Throughput

### Definition
How many operations complete per cycle.
*   **Arithmetic**
*   **Memory**

### Little's Law
Needed **parallelism** can be obtained by multiplying the **latency** and **throughput**.
*   Higher numbers of ***latency.throughput*** yields in more parallelism.
