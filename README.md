# CPU Scheduling Algorithm

This project implements a CPU scheduling algorithm using a combination of Round Robin (RR) and Priority Queue. The RR queue has a higher priority than the Priority Queue.

## Algorithm

The algorithm works as follows:

1. Each process has properties: `arrive_time`, `priority number`, and `bursts`.
2. The `bursts` start with a CPU burst and end with a CPU burst. In between, we have I/O bursts.
3. When a process in the RR queue has a CPU burst longer than the quantum, the CPU burst decreases to the quantum and goes to the RR queue. The remaining part of that CPU burst goes to the Priority Queue.

## Input

The program reads process information from an `input.txt` file. The input format is as follows:

p1:2, 4, 5, 7, 3

Where the first value is the process name, followed by `arrive_time`, `priority number`, and the `bursts`.

## Output

At the end of the scheduling, the program generates a Gantt chart and calculates standard metrics such as average waiting time, response time, etc. The program also considers dispatcher latency.

The output, including the Gantt chart and the calculated standards, is written to an `output.txt` file.

## Author

This project is developed by Alireza Mehraban, a Computer Science student and backend developer. 

## Contact

For any queries or further information, feel free to reach out at mr.kind1382@gmail.com.
