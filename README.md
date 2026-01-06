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

#### 🎮 [Nand2Tetris](https://github.com/kblee05/Nand2Tetris)
**Building a Modern Computer from First Principles (Logic Gates to OS)**
* **Constructed a complete 16-bit computer system** starting from NAND gates, establishing a deep understanding of hardware-software abstraction layers.
* **Engineered a full compilation toolchain in C++**, implementing a seamless translation pipeline:
  $$Jack\ Compiler \to VM\ Translator \to Assembler \to Binary\ Machine\ Code$$.
* **Developed a Minimalist Operating System (Jack OS)** with advanced memory management (`alloc`, `deAlloc`), math routines, and low-level I/O drivers.
* **Verified system integrity** by successfully running a complex Tetris application on the custom-built hardware/software stack.

---

#### 🛠️ [Memory-Allocator](https://github.com/kblee05/Memory-Allocator)
**Thread-Safe High-Performance Memory Allocator (Custom Malloc)**
* **Architected a dynamic memory allocator in C** with a focus on low-level memory layout control and minimal fragmentation overhead.
* **Implemented a Segregated Free List** with 10 optimized bins (32B to Large) to achieve high-speed chunk search and allocation.
* **Ensured Robust Thread-Safety** via `pthread_mutex` with an internal **Unlocked Helper Pattern** to eliminate self-deadlocks during `realloc`.
* **Benchmarked against glibc malloc**, achieving a throughput of **960,000+ ops/sec** and demonstrating competitive performance in specific trace-driven scenarios.
* **Engineered Advanced Memory Recovery** using splitting for oversized chunks and boundary-tag based coalescing to maximize heap utilization.

---

#### 🐚 [Shell](https://github.com/kblee05/SNU-Shell)
**Advanced Unix Shell with Hierarchical Command Execution Engine**
* **Designed a 5-layer shell architecture** (`Separator -> Logic -> Pipe -> Redirection -> Execution`) to ensure modularity and predictable command flow.
* **Implemented Recursive Subshell Execution** with nested parentheses, managing precise environment isolation via `fork`, `waitpid`, and depth-aware parsing.
* **Developed a High-Precision Logic Engine** for short-circuit evaluation (`&&`, ||) and logical negation (`!`) with strict exit status propagation.
* **Engineered a POSIX-compliant Lexer** utilizing a custom `dynamicstring` library to handle complex tokenization and escape sequences with zero memory leaks.
* **Conducted Deep System Profiling** using `ps` and process tree analysis to verify complex process hierarchies and resource reaping behavior.
<br>

### 📫 Contact
- **Email:** kennethbwlee@snu.ac.kr
