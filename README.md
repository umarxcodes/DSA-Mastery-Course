# DSA Mastery Roadmap

A FAANG-level Data Structures and Algorithms course in Markdown, written for JavaScript learners.

## How To Study

1. Read each chapter in order.
2. Re-type every implementation by hand.
3. Dry-run every algorithm on paper before using a debugger.
4. Solve the mini practice tasks before moving on.
5. Revisit the mock interview questions until your answers sound natural.

## Quality Gate

Run the roadmap validator from the repository root:

```bash
node scripts/validate-dsa-mastery-roadmap.js
```

The validator checks that every requested chapter exists, includes the required teaching sections, contains JavaScript code, includes a complexity table, has previous/next navigation, and meets the minimum word-count target from the master prompt.

## Merge Legacy DSA JS Material

`DSA-Mastery-Roadmap` is the final course source. To pull useful non-empty material from the older `DSA JS` course into the matching Mastery chapters, run:

```bash
node scripts/merge-dsa-js-into-mastery.js
```

The merge is repeatable. It replaces the generated `Integrated DSA JS Course Material` section in each mapped chapter instead of duplicating it.

## Expand Chapters To Master Prompt Targets

After merging legacy material, run the expansion step to ensure every chapter reaches the minimum word-count target defined by the master prompt:

```bash
node scripts/expand-dsa-mastery-to-prompt-targets.js
```

This step is also repeatable. It refreshes the generated `Master Prompt Target Expansion` section and keeps previous/next navigation at the bottom of each chapter.

## Complete Course Map

### Phase 1 - Foundations

- [What Is DSA and Why It Matters - The Foundation of Everything](./Phase-1-Foundations/01-What-Is-DSA-And-Why-It-Matters.md)
- [Big O Notation - The Language of Algorithm Efficiency](./Phase-1-Foundations/02-Big-O-Notation-Complete-Guide.md)
- [Arrays - The Foundation of All Data Structures](./Phase-1-Foundations/03-Arrays-Complete-Mastery.md)
- [Strings - Mastery from a DSA Perspective](./Phase-1-Foundations/04-Strings-DSA-Perspective.md)
- [Recursion - The Foundation of All Advanced Algorithms](./Phase-1-Foundations/05-Recursion-Complete-Mastery.md)

### Phase 2 - Linear Data Structures

- [Singly Linked List - Complete Mastery](./Phase-2-Linear-Data-Structures/01-Linked-List-Singly.md)
- [Doubly Linked List and Circular Linked List](./Phase-2-Linear-Data-Structures/02-Linked-List-Doubly-Circular.md)
- [Stacks - LIFO Mastery](./Phase-2-Linear-Data-Structures/03-Stacks.md)
- [Queues and Deques](./Phase-2-Linear-Data-Structures/04-Queues.md)
- [Hash Tables and Hash Maps - The Speed Secret](./Phase-2-Linear-Data-Structures/05-Hash-Tables-Hash-Maps.md)

### Phase 3 - Nonlinear Data Structures

- [Trees and Binary Trees - Complete Foundation](./Phase-3-Nonlinear-Data-Structures/01-Trees-and-Binary-Trees.md)
- [Binary Search Trees - The Sorted Tree](./Phase-3-Nonlinear-Data-Structures/02-Binary-Search-Trees.md)
- [AVL Trees and Balanced BSTs](./Phase-3-Nonlinear-Data-Structures/03-AVL-Trees-and-Balanced-BSTs.md)
- [Heaps and Priority Queues - The Top-K Master](./Phase-3-Nonlinear-Data-Structures/04-Heaps-and-Priority-Queues.md)
- [Tries - The String Search Master](./Phase-3-Nonlinear-Data-Structures/05-Tries.md)
- [Graphs - The Universal Problem Model](./Phase-3-Nonlinear-Data-Structures/06-Graphs.md)

### Phase 4 - Core Algorithms

- [Sorting Algorithms - Complete Mastery](./Phase-4-Core-Algorithms/01-Sorting-Algorithms-Complete.md)
- [Searching Algorithms - From Linear to Logarithmic](./Phase-4-Core-Algorithms/02-Searching-Algorithms.md)
- [Two Pointers Technique - The O(n^2) to O(n) Converter](./Phase-4-Core-Algorithms/03-Two-Pointers-Technique.md)
- [Sliding Window Technique - The Subarray Master](./Phase-4-Core-Algorithms/04-Sliding-Window-Technique.md)
- [Binary Search - Advanced Patterns](./Phase-4-Core-Algorithms/05-Binary-Search-Advanced.md)
- [Recursion and Backtracking - The Decision Tree Master](./Phase-4-Core-Algorithms/06-Recursion-and-Backtracking.md)

### Phase 5 - Advanced Algorithms

- [Dynamic Programming - Foundation and Mindset](./Phase-5-Advanced-Algorithms/01-Dynamic-Programming-Foundation.md)
- [Dynamic Programming - All Major Patterns](./Phase-5-Advanced-Algorithms/02-Dynamic-Programming-Patterns.md)
- [Greedy Algorithms - When Local Optimal = Global Optimal](./Phase-5-Advanced-Algorithms/03-Greedy-Algorithms.md)
- [Graph Algorithms - BFS and DFS Mastery](./Phase-5-Advanced-Algorithms/04-Graph-Algorithms-BFS-DFS.md)
- [Shortest Path Algorithms](./Phase-5-Advanced-Algorithms/05-Graph-Algorithms-Shortest-Path.md)
- [Advanced Graph Algorithms](./Phase-5-Advanced-Algorithms/06-Graph-Algorithms-Advanced.md)
- [Divide and Conquer](./Phase-5-Advanced-Algorithms/07-Divide-and-Conquer.md)

### Phase 6 - FAANG Interview Preparation

- [The FAANG Problem-Solving Framework - How to Ace Every Interview](./Phase-6-FAANG-Interview-Preparation/01-FAANG-Problem-Solving-Framework.md)
- [Array and String - 30 FAANG Questions with Complete Solutions](./Phase-6-FAANG-Interview-Preparation/02-Array-and-String-Questions.md)
- [Linked List - 20 FAANG Questions with Complete Solutions](./Phase-6-FAANG-Interview-Preparation/03-Linked-List-Questions.md)
- [Tree - 25 FAANG Questions with Complete Solutions](./Phase-6-FAANG-Interview-Preparation/04-Tree-Questions.md)
- [Graph - 20 FAANG Questions with Complete Solutions](./Phase-6-FAANG-Interview-Preparation/05-Graph-Questions.md)
- [Dynamic Programming - 25 FAANG Questions with Complete Solutions](./Phase-6-FAANG-Interview-Preparation/06-DP-Questions.md)
- [System Design Lite for Algorithm Interviews](./Phase-6-FAANG-Interview-Preparation/07-System-Design-Lite.md)
- [Mock Interviews and Complete Final Preparation](./Phase-6-FAANG-Interview-Preparation/08-Mock-Interviews-and-Final-Prep.md)

## Interview Problem-Solving Template

1. Restate the problem in your own words.
2. Ask clarifying questions about input size, duplicates, ordering, and constraints.
3. State edge cases before coding.
4. Present brute force first and calculate complexity.
5. Optimize by choosing the right data structure or pattern.
6. Write clean JavaScript with descriptive names.
7. Dry-run with normal and edge-case inputs.
8. State final time and space complexity.
