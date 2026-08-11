### **Program Description**

The Payroll Processing program simulates a simple **Batch Operating System** environment. It reads employee payroll details from an input file, processes the salary calculations, and stores the processed results in an output file.

For each employee, the program calculates:

* **Basic Salary**
* **Basic Rate Allowance (BRA)** = 20% of Basic Salary
* **Dearness Allowance (DA)** = 10% of Basic Salary
* **Updated Salary** = Basic Salary + BRA + DA

### **Input Format**

The `input.txt` file contains employee ID and basic salary values.

Example:

```text
101 25000
102 30000
103 28000
```

### **Output Format**

The processed details are stored in `output.txt`.

Example:

```text
ID      BASIC Salary
101     32500
102     39000
103     36400
```

### **Execution**

Compile the C program using:

```bash
gcc payroll.c -o payroll
```

Run the program using:

```bash
./payroll
```

On successful execution, the following message is displayed:

```text
Successfully Executed!
```

The calculated payroll details are then written to `output.txt`.

---

# PROJECT - 2 : PROCESS CONTROL BLOCK (PCB)

## 2.1 PCB Structure

A **Process Control Block (PCB)** is a data structure maintained by the operating system to store important information about a process.

The PCB contains details such as:

* Process ID (PID)
* Process State
* Program Counter
* Priority
* CPU registers and other process-related information

### Program

The `snippet-1_pcb_snippet.c` program demonstrates the basic structure of a PCB by defining fields such as **Process ID, Program Counter, and Priority**.

Example structure:

```c
struct PCB {
    int processID;
    int programCounter;
    int priority;
};
```

---

## 2.2 Context Switching

**Context switching** is the process in which the operating system saves the state of a currently running process and loads the saved state of another process.

During a context switch, information such as the **program counter, process state, and CPU-related information** is saved and restored.

The `snippet-2_pcb_contextSwitch.c` program demonstrates the basic concept of context switching using PCB information.

### Steps Involved

1. Save the current process information.
2. Store the information in its PCB.
3. Select the next process to execute.
4. Load the next process's PCB information.
5. Restore its execution state.
6. Continue execution of the selected process.

---

# PROJECT STRUCTURE

```text
OS-Projects/
│
├── project-1_Payroll_Simulation.zip
│
├── snippet-1_pcb_snippet.c
│
├── snippet-2_pcb_contextSwitch.c
│
└── README.md
```

---

# Technologies Used

* **Programming Language:** C
* **Operating System Concepts:** Batch Processing, Process Control Block, Context Switching
* **File Handling:** C File I/O
* **Compiler:** GCC
* **Version Control:** Git & GitHub

---

# Learning Outcomes

Through these projects, the following Operating System concepts are demonstrated:

* Batch OS processing
* File handling in C
* Process Control Block (PCB)
* Process information management
* Program Counter
* Process Priority
* Context Switching
* Basic process management concepts

---

# Author

**Purna Chandra Kumar Panigrahi**

GitHub: **Purna-Chandra-kumar**
