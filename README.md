# Job Scheduling using Greedy Algorithm (C)

## Overview

This project implements the **Job Sequencing with Deadlines** problem using a **Greedy Algorithm** in C. The objective is to schedule jobs in such a way that total profit is maximized while meeting job deadlines.

Each job has:

* Deadline
* Profit
* Processing Time

The algorithm prioritizes jobs with higher profit and assigns them to the latest available time slot before their deadline.

---

## Algorithm Used

**Greedy Approach (Job Sequencing with Deadlines)**

### Strategy:

1. Sort jobs in descending order of profit.
2. Initialize time slots as empty.
3. For each job:

   * Assign it to the latest free slot before its deadline.
4. Calculate total profit.

---

## Time Complexity

* Sorting: O(n²)
* Scheduling: O(n²)

Overall Complexity: **O(n²)**

---

## Features

* Accepts user input for job details
* Displays sorted job list
* Generates optimal job schedule
* Calculates total profit
* Saves output to a file (`job_scheduling_output.txt`)

---

## Input Format

User provides:

* Number of jobs (n)
* Number of machines (m) *(currently not used in logic)*
* Job details:

  ```
  Deadline Profit ProcessingTime
  ```

---

## Output

* Displays:

  * Job list
  * Final job schedule
  * Total profit
* Writes results to:

  ```
  job_scheduling_output.txt
  ```

---

## How to Run

### Step 1: Compile

```bash
gcc program.c -o program
```

### Step 2: Execute

```bash
program
```

---

## Example

### Input:

```
Enter number of jobs: 4
Enter number of machines: 1

Enter job details:
2 100 1
1 50 1
2 10 1
1 20 1
```

### Output:

```
Final Job Schedule:
Time Slot 1 -> Job 2
Time Slot 2 -> Job 1

Total Profit = 150
```

---

## Notes

* The number of machines is taken as input but not utilized.
* Assumes each job takes one unit of time for scheduling.
* Uses a simple array-based slot allocation.

---

## Author

[Your Name]

---
