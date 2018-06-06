# Latency
Here are some key notes on the latency issue and how to overcome this issue.

### Definition
Time required to perform an operation.
*   Average number of cycles.

### Ideal Condition
*   Have enough transactions in flight to saturate the memory bus.
*   Latency can be hidden by having more transactions in flight.
*   Do other operations when stalled.

### Solution
*   Increase active threads or **Instruction Level Parallelism** (ILP).  