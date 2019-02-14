## Scheduling 2
#### Panturu Sara - 3AHIF

1. **Multiple Queues**


| Run | 1 | 2 | 3 | 4 | 5 |
| -- | -- | -- | -- | -- | -- |
Queue | 1 | 2 | 4 | 8 | 15 |
Acc | 1 | 3 | 7 | 15 | 30 |

It must be swapped in 5 times.

2. **Shortest Process Next**

E3 = T0/8 + T1/8 + T2/4 + T3/2

A: 50/8 + 150/8 + 300/4 + 85/2
A = 142,5

B: 300/8 + 150/8 + 85/4 + 50/2
B = 102,5

B  will be taken by the scheduler because of its lower time.

3. **CPU-bound and I/O-bound Processes**

CPU-bound: needs high quanta but low priority
I/O-bound: needs low quanta but high priority

It is important to distinguish between CPU and I/O-bound processes because an I/O-bound process needs small quanta and this causes frequent context switches which cause high administration costs.

4. **Real Time Schedulable**

Sum of (Ci/Pi) <= 1

35/50 + 20/100 + 10/200 + $x$/250 <= 1

0,95 + $x$/250 <= 1

$x$ <= (1 - 0,95) * 250

$x$ <= 12,5

The largest value of $x$ is 12,5.
