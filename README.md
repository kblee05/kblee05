### Hi there, I'm Kenneth Lee 👋

I am an undergraduate student at **Seoul National University**, currently majoring in **Architecture** and focusing on **Computer Science and Engineering**.

My primary research interests lie in **Computer Systems**, **Compilers**, **Operating Systems**, and **System Architecture**. I am passionate about understanding how software interacts with hardware and building efficient, low-level systems.

I am actively looking for **Research Intern** opportunities where I can contribute to ongoing system research projects.

<br>

### 🎓 Education
- **Seoul National University** (Mar. 2024 - Present)
  - B.S. in Architecture and Architectural Engineering
  - Computer Science and Engineering

<br>

### 🛠 Tech Stack
<p>
  <img src="https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=white"/>
  <img src="https://img.shields.io/badge/C++-00599C?style=flat-square&logo=c%2B%2B&logoColor=white"/>
  <img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black"/>
</p>

<br>

### 📌 Pinned Projects & Experience

#### [Nand2Tetris](https://github.com/kblee05/Nand2Tetris)
> **Building a Modern Computer from First Principles**
> - Constructed a complete general-purpose computer system starting from NAND gates to the Operating System.
> - **Implemented the full compilation toolchain using C++**, establishing a seamless translation pipeline:
>   $Jack Compiler \to VM Translator \to Assembler \to Binary Machine Code$.
> - Developed the Standard Library (OS) including memory management (`alloc`, `deAlloc`), math routines, and I/O drivers.
> - Gained deep understanding of the hardware-software interface and abstraction layers.


### 🛠️ [Memory-Allocator](https://github.com/kblee05/Memory-Allocator)
**Thread-Safe High-Performance Memory Allocator**

* **Architected a custom dynamic memory allocator** (`malloc`, `free`, `realloc`) from scratch, emphasizing low-level memory layout control and efficiency.
* **Implemented a Segregated Free List** with 10 bins (32B to Large) to minimize search time and external fragmentation.
* **Ensured Thread-Safety** by implementing a coarse-grained locking strategy using `pthread_mutex`, while avoiding self-deadlocks in `realloc` via internal unlocked helper functions.
* **Optimized Memory Throughput**, achieving over **960,000 ops/sec** in synthetic benchmarks, outperforming basic glibc-like implementations in specific trace-driven scenarios.
* **Features Advanced Coalescing & Splitting**, reducing internal fragmentation by splitting oversized chunks and merging adjacent free blocks during deallocation.


### 🐚 [Shell](https://github.com/kblee05/SNU-Shell)
**Advanced Unix Shell with Hierarchical Command Execution**

* **Engineered a multi-layered shell architecture** (`Separator -> Logic -> Pipe -> Execution`) to handle complex command flows with high modularity.
* **Implemented Recursive Subshell Execution** using nested parentheses, ensuring precise environment isolation and execution context via depth-aware parsing.
* **Developed a High-Precision Logic Engine** supporting short-circuit operators (`&&`, `||`) and logical negation (`!`) with strict exit status (`last_status`) propagation.
* **Engineered a Robust POSIX Lexer**, utilizing a custom `dynamicstring` library to handle variable token lengths and escape sequences without memory leaks.
* **Deep System Analysis**: Conducted low-level debugging using `ps` and process tree analysis to verify subshell fork-wait behavior and resource reaping.
<br>

### 📫 Contact
- **Email:** kennethbwlee@snu.ac.kr
