# ENCS351: Operating System Lab - Process Management Assignments

This repository contains solutions for the **Operating System Lab (ENCS351)** assignments, focusing on **Process Management** concepts: process creation, execution, state management (Zombie/Orphan), and prioritization.

---

## Student and Submission Details

- **Name:** Aditi Saraswat
- **Roll Number:** 2301010020
- **Course Code & Name:** ENCS351 Operating System Lab
- **Program:** B.Tech CSE (Sem-05)
- **Course Teacher:** Mrs. Suman
- **Assignments Covered:** Lab Assignment Sheet-1 & Sheet-2

---

## Lab Assignments Overview

### Lab Assignment Sheet-1: Process Creation and Management

**Technologies Used:** Python (`os`, `subprocess`) and Java (`ProcessBuilder`)

**Tasks:**

1. **Process Creation**: Creates N child processes using Python's `os.fork()` or Java's `ProcessBuilder`. Parent waits for all children.
2. **Command Execution**: Child processes execute system commands (Linux: `ls`, `date`; Windows: `date /t`, `whoami`) using Python's `os.execvp()` or Java's `ProcessBuilder`.
3. **Zombie & Orphan Processes**: Simulates Zombie (parent skips waiting) and Orphan (parent exits first) processes.
4. **Inspecting /proc**: Reads and prints process details (name, state, memory usage, executable path) from `/proc` filesystem in Python; conceptual approach in Java.
5. **Prioritization**: Creates CPU-intensive tasks and assigns different priority levels to observe scheduler impact.

### Lab Assignment Sheet-2: System Startup and Process Simulation

**Technologies Used:** Python (`multiprocessing`, `logging`) and Java (`Thread`, `Logger`)

**Objective:** Simulates system boot-up, concurrent process creation, graceful shutdown, and lifecycle logging to `process_log.txt`.

---

## How to Run Everything

### Prerequisites

- **Python:** Python 3.x installed
- **Java:** JDK 11 or newer installed
- **Environment:**
    - Python scripts: Linux/WSL recommended for `fork` and `/proc`.
    - Java code: Windows recommended (`cmd.exe /c` commands).

---

### Python Execution (Recommended on Linux/WSL)

1. **Clone the repository**
```bash
git clone [YOUR_GITHUB_REPO_URL]
cd [repository_name]
````
2. **Run Lab 1 (Process Management)**
```bash
python process_management.py
```
---
-Terminal displays output for all tasks.

-Sample output is saved in output.txt.

---
3. **Run Lab 2 (System Startup Simulation)**
```bash
python system_simulation.py
```
---
-Terminal displays:

---
```bash
System Starting...
System Shutdown.
```
---
-Lifecycle log file process_log.txt is generated.

---
### Java Execution (Used in Report)
1. Ensure Java source files are under:
```bash
src/org/example/Lab_05/
```
2. Compile the code
```bash
javac -d . src/org/example/Lab_05/*.java
```
3. Run the main execution class
```bash
java org.example.Lab_05.ProcessManagement
```
---
-Console displays outputs for all tasks (Task 1–5), including process creation, command execution, and priority simulation.

---
### Commands Summary
---
-For quick reference, here are all the main commands you need to run the assignments:

---
```bash
# Clone the repository
git clone [YOUR_GITHUB_REPO_URL]
cd [repository_name]

# Python Lab 1
python process_management.py

# Python Lab 2
python system_simulation.py

# Java Compilation
javac -d . src/org/example/Lab_05/*.java

# Java Execution
java org.example.Lab_05.ProcessManagement

```
