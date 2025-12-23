# Optimized Round Robin Scheduling for RTOS

This repository contains an **Optimized Round Robin (ORR)** scheduling approach designed for **real-time operating systems (RTOS)**.

## What's in This Repo
- **Slides** explaining the problem, approach, and results
- A **short demo video** showing how to run the project
- The **source code**
- The **original research paper**
- Additional **related research** used to develop better scheduling heuristics

## Heuristic Overview
This project uses a bounded-range heuristic to estimate an effective time quantum:

- Compute an **upper bound** as:

    $$
    \text{Limit Range} = \frac{\text{mean burst} + \text{max burst}}{2}
    $$

This upper bound helps generate more effective (near-optimal) time slices compared to selecting a random quantum or relying on user-defined values.

## How to Run
See the included **demo video** for step-by-step instructions on running the code.

## Notes
If you're interested in experimenting, try adjusting the bound strategy or comparing performance against standard Round Robin using metrics like waiting time, turnaround time, and context switches.
