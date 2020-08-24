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
