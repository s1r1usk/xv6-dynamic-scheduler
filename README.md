 xv6 with Custom Dynamic Scheduler

This is a modified version of MIT's xv6 operating system. The default Round Robin scheduler has been replaced with a custom scheduler that dynamically calculates the time quantum for each process.

The new scheduler uses the following formula to compute the time quantum dynamically:
Time Quantum = Time Quantum + (Number of times the process is scheduled in the ready queue / Total execution time of all processes) * Time Quantum

