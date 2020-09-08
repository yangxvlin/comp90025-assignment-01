# comp90025-assignment-01
COMP90025 - Parallel and Multicore Computing - 2020S2 - Assignment1

# Quiz Instructions
Project 1 will be broken into small weekly quizzes, often of a single question, requiring an answer of a few hundred words.

Some of the questions will be revision of undergraduate concepts, and some will be about new content learned in this subject

# Week 2 homework: basic computer architecture
## Question 1 (10 pts)
```
Describe, in up to 100 words, the roles of the following main components:
- CPU
- Memory
- Bus
and how they work together. Talk about "address", "word size", "clock frequency", "instruction", "data" and the fetch-decode-execute-writeback concept, in relation to these main components.
```
- ```
    CPU is a piece of hardware that executes stored program instructions.

    Memory holds the instructions and data processed by CPU.

    CPU access the RAM using a Fetch-Decode-Execute-Writeback cycle. CPU read instruction from RAM in Fetch and put results back in Writeback from locations in memory as identified by the addresses. Each stage in the cycle demands a clock cycle and clock frequency is clock cycles per second to measure the performance of a CPU.

    The bus carries data, address, and control information in Fetch-Decode-Execute-Writeback cycle to connect CPU and memory. The standard single unit of bits for information transferred in between is word size. It shows the memory address size and the largest integer can be processed in a single instruction.
    ```

    my answer
- results
  - <img src="./docs/week 2.png" />
# Week 3 homework: Processor architecture
## Question 1 (10 pts)
```
Explain in about 300 words the role of registers and cache in a computer. How are they similar?  How are they different?  Where do they fit in the overall architecture?  How do they make computers run fast?
```
- ```
    Register is a quickly directly accessible location inside a computer's processor. It can hold an instruction being executed, a storage address, or immediately used data. Register can improve overall system speed because it has fastest accessing speed (1 clock cycle) because of a smaller capacity compared to cache. As it is an internal CPU “memory”, accesses to registers are faster than any other kind of memory accesses.

    Cache is a hardware/software component that is fast copy of recently used data from the main memory which can accelerate memory access speed. Cache makes computer run fast because the frequent slower small memory storage retrievals from main memory (Processor-Memory read operation time gap) is reduced as it is stored in cache with a faster access speed because of a smaller capacity compared to RAM.

    Both provide faster memory storage access for the processor. All of them are integrated in a CPU chip. The similarities are both can store data/instructions information. They have common goals to speed up the computer’s execution. Both have a faster-accessing speed than RAM. Register and L1 cache are both separated per core.

    The differences are: Registers are normally at the top of the memory hierarchy and provide the fastest way to access data. While cache is below register but above RAM with a larger storage size than register but with a slower accessing speed (3-5 times larger). Register is closer to ALU than cache. Register holds the data that CPU is currently processing whereas, cache holds instruction/data might be required. Cache has different level hierarchy inside it while register only has different types for various specialization. For example, general-purpose register can store a data or memory location address, but data registers can be assigned to a variety of functions by the programmer. Register is separated per core while L2&L3 cache is shared between cores. The memory inside the cache is addressable, whereas registers (almost always) are not.
    ```

    my answer
- results
  - <img src="./docs/week 3.png" />