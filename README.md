# disk-scheduling-algorithms
Programs implementing various disk scheduling algorithms including FCFS, SSTF, SCAN, CSCAN, LOOK, and CLOOK with performance metrics. Ideal for learning and demonstration purposes

## Table of Contents
- [Introduction](#introduction)
- [Algorithms Implemented](#algorithms-implemented)
- [Languages Supported](#languages-supported)
- [Usage](#usage)
- [How to Run](#how-to-run)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Disk scheduling is a technique used by operating systems to decide the order in which requests for disk I/O are processed. Efficient scheduling minimizes seek time, improving overall system performance. This project demonstrates and compares the following disk scheduling algorithms.

## Algorithms Implemented

1. **First-Come-First-Serve (FCFS):**  
   Processes requests in the order they arrive.
2. **Shortest Seek Time First (SSTF):**  
   Picks the request that is closest to the current head position.
3. **SCAN (Elevator):**  
   Moves the head in one direction, servicing requests until it reaches the end, then reverses.
4. **C-SCAN (Circular SCAN):**  
   Similar to SCAN but returns to the beginning of the disk when it reaches the end.

## Languages Supported
The following programming languages are used to implement the algorithms:
- [C](./C)
- [C++](./C++)
- [Java](./Java)
- [Python](./Python)

Each implementation uses the same logic to ensure comparability.

## Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/disk-scheduling-algorithms.git
   cd disk-scheduling-algorithms
   ```
2. Navigate to the folder corresponding to your preferred programming language.

3. Compile and run the code in the language of your choice (instructions provided below).

## How to Run

### **C**
1. Compile the C code:
   ```bash
   gcc disk_scheduling.c -o disk_scheduling
   ```
2. Run the executable:
   ```bash
   ./disk_scheduling
   ```

### C++
1. Compile the C++ code:
   ```bash
   g++ disk_scheduling.cpp -o disk_scheduling
   ```
2. Run the executable:
   ```bash
   ./disk_scheduling
   ```

### Java
1. Compile the Java code:
   ```bash
   javac DiskScheduling.java
   ```
2. Run the program:
   ```bash
   java DiskScheduling
   ```

### Python
1. Run the Python code directly:
   ```bash
   python3 disk_scheduling.py
   ```

## Example Input/Output
Input:  
```plaintext
Enter the number of disk access requests: 8  
Enter the requests (between 0 and 199):  
98  
183  
37  
122  
14  
124  
65  
67  
Select the policy:  
1. FCFS  
2. SSTF  
3. SCAN  
4. CSCAN  
```

Output (FCFS Example):  
```plaintext
----------------
FCFS:  
53 -> 98 -> 183 -> 37 -> 122 -> 14 -> 124 -> 65 -> 67  
Performance: 640  
----------------
```

## Contributing
Contributions are welcome!  
- Fork the repository.
- Create a new branch for your feature or bug fix.
- Commit your changes and create a pull request.
