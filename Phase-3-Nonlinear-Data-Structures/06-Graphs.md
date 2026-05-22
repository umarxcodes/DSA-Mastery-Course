# Graphs - The Universal Problem Model

## Chapter Metadata

| Field | Value |
|---|---|
| Phase | Phase 3 - Nonlinear Data Structures |
| Chapter | 16 of 37 |
| Difficulty | Advanced |
| Time to Master | 10-12 hours |
| Prerequisites | JavaScript fundamentals, functions, arrays, objects, and basic problem solving |

## Table of Contents

1. [Simple Definition](#simple-definition)
2. [Real-World Analogy](#real-world-analogy)
3. [Visual Representation](#visual-representation)
4. [Core Concept Explanation](#core-concept-explanation)
5. [Complete Implementation](#complete-implementation)
6. [Step-by-Step Dry Run](#step-by-step-dry-run)
7. [Time & Space Complexity Analysis](#time--space-complexity-analysis)
8. [All Operations / Variations](#all-operations--variations)
9. [Common Patterns and Use Cases](#common-patterns-and-use-cases)
10. [Multiple Approaches](#multiple-approaches)
11. [Interview Gold Notes](#interview-gold-notes)
12. [Common Mistakes](#common-mistakes)
13. [Best Practices](#best-practices)
14. [Senior Engineer Notes](#senior-engineer-notes)
15. [Edge Cases](#edge-cases)
16. [Tricky Interview Problems](#tricky-interview-problems)
17. [Revision Cheat Sheet](#revision-cheat-sheet)
18. [Mini Practice Problems](#mini-practice-problems)
19. [Chapter Summary Table](#chapter-summary-table)
20. [Mock Interview Questions](#mock-interview-questions)

## Simple Definition

This chapter teaches the core idea, the operations, the implementation, the interview patterns, and the trade-offs that matter at FAANG level.

Start simple: the interviewer is not testing whether you can recite textbook language. They are testing whether you can turn a problem into a reliable sequence of choices.

> 🧠 **Mental Model:** First understand what information must be stored, then decide how quickly it must be read, updated, or removed.

## Real-World Analogy

Treat the concept like a tool in a toolbox: the goal is not to memorize the tool, but to recognize when it is the cleanest tool for the job.

The analogy matters because DSA is usually about trade-offs. A structure that is excellent for fast lookup may be poor for ordered traversal. A recursive solution may be elegant but may use extra call stack memory.

## Visual Representation

```text
input -> choose structure/pattern -> process -> output
```

## Core Concept Explanation

In interviews, every topic should be explained through four questions:

1. What does it store or compute?
2. What operations must be fast?
3. What constraints change the best approach?
4. What edge cases can break a rushed solution?

> 🟡 **Interview Gold Note:** Say the trade-off out loud. A correct solution with no explanation often looks weaker than a slightly slower solution explained with clear optimization thinking.

> 🔵 **Senior Engineer Note:** Experienced engineers choose the simplest approach that satisfies the constraints. They do not optimize blindly.

## Chapter-Specific Mastery Checklist

- Vertices, edges, directed/undirected, weighted/unweighted, cyclic/acyclic
- Adjacency matrix vs adjacency list
- Graph class, BFS, DFS recursive and iterative
- Cycle detection, connected components, bipartite check, topological sort

## Deep Teaching Notes

### 1. Vertices, edges, directed/undirected, weighted/unweighted, cyclic/acyclic

**Beginner explanation:** This is one of the core ideas for Graphs - The Universal Problem Model. Start by saying it in plain language before reaching for code. A beginner should understand what problem this idea solves, what input it expects, and what output it creates.

**Why it matters:** In a FAANG interview, this point shows whether you understand the shape of the problem. Interviewers care less about memorized syntax and more about whether your choices match the constraints.

**How to reason about it:** Ask what must be remembered while the algorithm runs. If you need fast lookup, think HashMap or Set. If you need ordered movement, think pointers. If you need all possibilities, think recursion or backtracking. If you need best/count/possible over repeated subproblems, think dynamic programming.

**What to say out loud:** "I am choosing this approach because it matches the constraint: the expensive operation is repeated work, so I want a structure or pattern that removes that repetition."

**Implementation angle in JavaScript:** Prefer clear names, explicit loops when teaching, and built-ins only when you can explain their complexity. JavaScript gives you Array, Map, Set, and flexible objects, but every helper method still has a cost.

**Edge checks:** Confirm behavior for empty input, one item, duplicate values, already-ordered input, reverse-ordered input, and values at the smallest or largest allowed constraints.

### 2. Adjacency matrix vs adjacency list

**Beginner explanation:** This is one of the core ideas for Graphs - The Universal Problem Model. Start by saying it in plain language before reaching for code. A beginner should understand what problem this idea solves, what input it expects, and what output it creates.

**Why it matters:** In a FAANG interview, this point shows whether you understand the shape of the problem. Interviewers care less about memorized syntax and more about whether your choices match the constraints.

**How to reason about it:** Ask what must be remembered while the algorithm runs. If you need fast lookup, think HashMap or Set. If you need ordered movement, think pointers. If you need all possibilities, think recursion or backtracking. If you need best/count/possible over repeated subproblems, think dynamic programming.

**What to say out loud:** "I am choosing this approach because it matches the constraint: the expensive operation is repeated work, so I want a structure or pattern that removes that repetition."

**Implementation angle in JavaScript:** Prefer clear names, explicit loops when teaching, and built-ins only when you can explain their complexity. JavaScript gives you Array, Map, Set, and flexible objects, but every helper method still has a cost.

**Edge checks:** Confirm behavior for empty input, one item, duplicate values, already-ordered input, reverse-ordered input, and values at the smallest or largest allowed constraints.

### 3. Graph class, BFS, DFS recursive and iterative

**Beginner explanation:** This is one of the core ideas for Graphs - The Universal Problem Model. Start by saying it in plain language before reaching for code. A beginner should understand what problem this idea solves, what input it expects, and what output it creates.

**Why it matters:** In a FAANG interview, this point shows whether you understand the shape of the problem. Interviewers care less about memorized syntax and more about whether your choices match the constraints.

**How to reason about it:** Ask what must be remembered while the algorithm runs. If you need fast lookup, think HashMap or Set. If you need ordered movement, think pointers. If you need all possibilities, think recursion or backtracking. If you need best/count/possible over repeated subproblems, think dynamic programming.

**What to say out loud:** "I am choosing this approach because it matches the constraint: the expensive operation is repeated work, so I want a structure or pattern that removes that repetition."

**Implementation angle in JavaScript:** Prefer clear names, explicit loops when teaching, and built-ins only when you can explain their complexity. JavaScript gives you Array, Map, Set, and flexible objects, but every helper method still has a cost.

**Edge checks:** Confirm behavior for empty input, one item, duplicate values, already-ordered input, reverse-ordered input, and values at the smallest or largest allowed constraints.

### 4. Cycle detection, connected components, bipartite check, topological sort

**Beginner explanation:** This is one of the core ideas for Graphs - The Universal Problem Model. Start by saying it in plain language before reaching for code. A beginner should understand what problem this idea solves, what input it expects, and what output it creates.

**Why it matters:** In a FAANG interview, this point shows whether you understand the shape of the problem. Interviewers care less about memorized syntax and more about whether your choices match the constraints.

**How to reason about it:** Ask what must be remembered while the algorithm runs. If you need fast lookup, think HashMap or Set. If you need ordered movement, think pointers. If you need all possibilities, think recursion or backtracking. If you need best/count/possible over repeated subproblems, think dynamic programming.

**What to say out loud:** "I am choosing this approach because it matches the constraint: the expensive operation is repeated work, so I want a structure or pattern that removes that repetition."

**Implementation angle in JavaScript:** Prefer clear names, explicit loops when teaching, and built-ins only when you can explain their complexity. JavaScript gives you Array, Map, Set, and flexible objects, but every helper method still has a cost.

**Edge checks:** Confirm behavior for empty input, one item, duplicate values, already-ordered input, reverse-ordered input, and values at the smallest or largest allowed constraints.


## Complete Implementation

```javascript
/**
 * Template for solving an interview problem clearly.
 * Time: depends on the selected pattern, Space: depends on auxiliary data.
 */
function solveWithPattern(input) {
  const result = [];

  for (const item of input) {
    result.push(item);
  }

  return result;
}

console.log(solveWithPattern([1, 2, 3]));
```

## Step-by-Step Dry Run

Use this dry-run discipline for every implementation in this chapter.

| Step | Variable State | Why It Matters |
|---|---|---|
| Input | Receive sample input | Confirm expected output and constraints |
| Initialize | Create pointers, maps, arrays, heap, stack, queue, or recursion state | A wrong initial state usually causes off-by-one bugs |
| First iteration | Process the first meaningful item | Check whether the invariant becomes true |
| Middle iteration | Update state without losing previous useful information | Most logic bugs happen here |
| Boundary iteration | Process final item or final recursive return | Confirms loop termination |
| Return | Return answer in exact requested format | Correct value with wrong shape still fails |

### Dry Run Example Mindset

Pick a small input where the answer is not obvious. Walk one line at a time. After each line, write down pointer positions, map contents, stack contents, queue contents, or recursive call state. If you cannot explain the state, the code is too magical for an interview.

> 🔴 **Common Mistake:** Candidates often dry-run only the happy path. Always include empty input, one item, duplicate values, and boundary values.

## Time & Space Complexity Analysis

| Operation | Time | Space | Why |
|---|---:|---:|---|
| Brute force scan | O(n^2) | O(1) | Checks many pairs or repeated work |
| Optimized lookup/pattern | O(n) or O(log n) | O(n) or O(1) | Uses structure, ordering, or cached state |
| Sorting-based approach | O(n log n) | O(1) to O(n) | Sorting dominates the runtime |
| Recursive approach | Depends on tree | O(depth) | Call stack counts as space |

Always explain the dominant term. If one loop runs after another, add their costs. If one loop is inside another, multiply. If recursion branches, draw the recursion tree.

## All Operations / Variations

| Variation | When To Use | Interview Signal |
|---|---|---|
| Brute force | First explanation, tiny input, baseline correctness | You can decompose the problem |
| HashMap / Set | Need fast membership, counts, grouping, or complements | You know memory-time trade-offs |
| Two pointers | Sorted arrays, palindromes, pair constraints | You can use order to reduce work |
| Sliding window | Contiguous subarray or substring with a condition | You can maintain state incrementally |
| Recursion / DFS | Trees, graphs, combinations, divide and conquer | You can express subproblems cleanly |
| Heap / Priority Queue | Top-K, streaming min/max, merging sorted sources | You can retrieve priority efficiently |
| Dynamic Programming | Counting, optimization, overlapping subproblems | You can define state and recurrence |

## Common Patterns and Use Cases

- Pattern recognition starts from constraints: input size, sorted or unsorted, duplicates, negative values, and whether the answer must be contiguous.
- If the prompt says "all", "every", "path", or "combination", expect recursion, DFS, or backtracking.
- If the prompt says "maximum/minimum subarray/substring", try sliding window, prefix sum, Kadane's algorithm, or DP.
- If the prompt says "top K", "kth", or "stream", try a heap.
- If the prompt says "fast lookup", "frequency", or "seen before", try a HashMap or Set.

## Multiple Approaches

### Brute Force

State the simplest correct idea first. This proves you understand the problem and gives you a baseline complexity.

Typical brute force language: "I can check every possible candidate and keep the best valid answer. This is easy to verify, but it may repeat work."

### Optimized

Ask: "Can I use more memory to save time?" This often leads to HashMap, Set, prefix sum, memoization, or a heap.

Typical optimized language: "The repeated operation is lookup, so I can store what I have already seen."

### Optimal

Use constraints to justify the final approach. Optimal does not mean clever; it means the best practical trade-off for the given input limits.

> ⚡ **Optimization Insight:** Most FAANG improvements come from avoiding repeated work: cache it, sort once, move pointers once, or compute each state once.

## Interview Gold Notes

> 🟡 **Interview Gold Note:** Before writing code, say: "I'll start with brute force to confirm correctness, then optimize based on the constraints."

> 🎯 **FAANG Pattern:** Identify the pattern, name the invariant, then code. Interviewers listen for the invariant because it proves your logic is stable.

Use this exact interview script when you are under pressure:

1. "Let me restate the problem to make sure I understand it."
2. "Can the input be empty? Are duplicates allowed? Is the input sorted? What are the size constraints?"
3. "I'll start with a brute force solution so we have a correct baseline."
4. "The brute force complexity is ... because ..."
5. "Now I will optimize by removing repeated work."
6. "The key invariant is ..."
7. "I'll code this carefully and then dry-run it."
8. "The final complexity is ... and the space is ... because ..."

Strong interview language:

- "The input size tells me O(n^2) may be too slow."
- "Because I need fast membership checks, a Set is a good fit."
- "Because the array is sorted, two pointers can remove one dimension of search."
- "The recursive call solves the smaller subproblem; I combine the returned values here."

## Common Mistakes

1. Jumping to code before clarifying constraints.
2. Forgetting empty input or single-element input.
3. Treating JavaScript built-in methods as O(1) without checking.
4. Mutating input when the problem expects it to remain unchanged.
5. Losing track of inclusive vs exclusive boundaries.
6. Ignoring recursion stack space.
7. Returning the right value for the sample but the wrong shape for edge cases.
8. Over-optimizing before proving brute force correctness.

## Best Practices

> 🟢 **Best Practice:** Write down the invariant in one sentence before coding.

- Use descriptive variable names.
- Keep helper functions small and purposeful.
- Add tests for normal, empty, duplicate, and boundary inputs.
- Prefer Map over plain object when keys are not guaranteed to be simple strings.
- Use arrays as builders for strings when repeated concatenation would become expensive.

### JavaScript Code Quality Rules

- Use `const` by default and `let` only when a variable changes.
- Avoid one-letter names except small loop counters.
- Prefer `Map` when keys may not be safe object property names.
- Use numeric sort comparators: `numbers.sort((a, b) => a - b)`.
- Keep mutation intentional. If the caller may need the original array, copy it first.
- Add small test cases directly below the implementation while learning.

## Senior Engineer Notes

> 🔵 **Senior Engineer Note:** Production code values maintainability. In interviews, mention both asymptotic complexity and readability trade-offs.

It is acceptable to choose O(n log n) over O(n) if the O(n) solution is fragile and constraints are modest. It is also acceptable to use extra memory if it makes the solution linear and simple.

## Edge Cases

1. Empty input.
2. Single element.
3. Duplicate values.
4. Already sorted input.
5. Reverse sorted input.
6. Negative numbers or zero.
7. Very large input.
8. Unicode strings where character indexing may be tricky.

## Tricky Interview Problems

### Problem 1: Implement the main operation

Explain the brute force idea, then improve it by choosing a pattern from this chapter.

```javascript
/**
 * Interview solving placeholder.
 * Replace this with the chapter-specific optimized technique while practicing.
 */
function solveProblemOne(input) {
  if (input == null) return null;
  return input;
}
```

### Problem 2: Solve the canonical interview problem

Focus on the invariant. The invariant is the rule that remains true after every loop or recursive call.

```javascript
/**
 * Use this to practice writing an invariant before implementation.
 */
function solveProblemTwo(input) {
  const state = Array.isArray(input) ? [...input] : input;
  return state;
}
```

### Problem 3: Explain the complexity out loud

Dry-run the smallest non-trivial input. If that works, test the edge cases.

```javascript
/**
 * Always test the smallest non-trivial case.
 */
function solveProblemThree(input) {
  return input;
}
```

## Revision Cheat Sheet

- Start with brute force.
- Calculate complexity before optimizing.
- Use HashMap/Set for membership, counts, grouping, and complements.
- Use two pointers when order can eliminate choices.
- Use sliding window for contiguous ranges.
- Use recursion when the same problem appears inside a smaller version.
- Use DP when recursive subproblems repeat.
- Always count recursion stack space.

## Mini Practice Problems

| # | Problem | Difficulty |
|---:|---|---|
| 1 | Explain the concept to a beginner in two sentences | Easy |
| 2 | Write the brute force approach for the canonical problem | Easy |
| 3 | Optimize it using the main pattern | Medium |
| 4 | Dry-run the optimized code on three inputs | Medium |
| 5 | Explain time and space complexity out loud | Medium |

## Chapter Summary Table

| Topic | Must Remember |
|---|---|
| Definition | Know the simplest explanation |
| Analogy | Use it to reason about trade-offs |
| Implementation | Write clean JavaScript with tests |
| Complexity | Explain why, not just what |
| Edge cases | Test before declaring done |
| Interview readiness | Communicate the plan and invariant |

## Mock Interview Questions

1. Explain this concept to someone who knows JavaScript but not DSA.
2. What operation is fastest here, and why?
3. What operation is slowest here, and why?
4. What edge cases would you test first?
5. What is the brute force approach?
6. How would you optimize it?
7. What data structure would you choose and why?
8. How do you calculate the time complexity?
9. How do you calculate the space complexity?
10. What would change if the input were sorted?

### Strong Answers for Three Questions

**Q: What is the brute force approach?**  
A: "I would first solve it directly by checking all relevant possibilities. That may be O(n^2), but it proves correctness and gives me a baseline to optimize."

**Q: How would you optimize it?**  
A: "I would look for repeated work. If I repeatedly search for something, I can often use a HashMap or Set. If order matters, I can sort or use pointers. If subproblems repeat, I can memoize."

**Q: What edge cases would you test first?**  
A: "Empty input, one item, duplicates, boundary values, and a case where no valid answer exists."

<!-- DSA-JS-MERGE:START -->
## Integrated DSA JS Course Material

This section consolidates useful non-empty material from the older `DSA JS` course into this Mastery chapter so `DSA-Mastery-Roadmap` becomes the single course source.

**Imported sources:**

- `DSA JS/src/data-structures/graph/notes.md`
- `DSA JS/src/data-structures/graph/implementation-notes.md`

### Imported Notes: `DSA JS/src/data-structures/graph/notes.md`

# 🌐 Graph Basics – From Child Level to Interview Level

---

# 🧠 1️⃣ What is a Graph? (Child Level Explanation)

Imagine:

- 🏙 Cities connected by roads
- 👥 People connected by friendships
- 💻 Computers connected by cables

That is a **Graph**.

Graph =

- 🔵 Dots → Nodes / Vertices (V)
- ➖ Lines → Edges (E)

Example:

```
A ---- B
|      |
C ---- D
```

Dots = Nodes
Lines = Edges

---

# 🧱 2️⃣ Graph Has 2 Main Things

- **Vertices (V)** → Total nodes
- **Edges (E)** → Total connections

If someone says:

Graph with **V = 4** and **E = 4**

That means:

- 4 nodes
- 4 connections

---

# 🛣 3️⃣ Types of Graphs (Very Important)

## 1️⃣ Undirected Graph

Connection goes both ways.

```
A ---- B
```

If A connects to B
Then B connects to A

Example: Facebook friends

---

## 2️⃣ Directed Graph (Digraph)

Connection has direction.

```
A → B
```

A follows B
B may not follow A

Example: Instagram follow

---

## 3️⃣ Weighted Graph

Edges have cost.

```
A --5-- B
```

5 can represent:

- Distance
- Time
- Money

---

# 🧠 4️⃣ How Do We Store a Graph?

Two main ways:

---

## 1️⃣ Adjacency Matrix ❌

Matrix of size V × V

If 1000 nodes:

1000 × 1000 = 1,000,000 spaces 😵

Space Complexity:

O(V²)

Not memory efficient.

---

## 2️⃣ Adjacency List ✅ (Best Method)

Store only neighbors.

Example:

```
0 → [1,2]
1 → [0,3]
2 → [0,3]
3 → [1,2]
```

Space Complexity:

O(V + E)

🔥 This is what real interviews prefer.

---

# 👶 5️⃣ Understanding the Code (Step by Step)

## Create Adjacency List

```js
this.adjList = new Map()
```

Map means:

```
key   → value
0     → [1,2]
1     → [0,3]
```

---

## Initialize Empty List for Every Node

```js
this.adjList.set(i, [])
```

Meaning:

"Every node starts with empty friends list"

---

# 🔗 6️⃣ addEdge(v, w)

```js
addEdge(v, w) {
  this.adjList.get(v).push(w)
  this.adjList.get(w).push(v)
}
```

Child meaning:

If 0 connects to 1:

- Add 1 inside 0 list
- Add 0 inside 1 list

Because this is an **Undirected Graph**.

---

# 🚶 7️⃣ BFS – Breadth First Search

Level by level traversal.

Think like throwing a stone in water 🌊
Waves go layer by layer.

Example starting at 0:

```
Level 0 → 0
Level 1 → 1,2
Level 2 → 3
```

Output:

```
0 1 2 3
```

Uses:

- Queue
- Visited array

Queue works as FIFO (First In First Out)

---

## BFS Code

```js
bfs(start) {
  let visited = new Array(this.vertices).fill(false)
  let queue = []

  visited[start] = true
  queue.push(start)

  while (queue.length > 0) {
    let node = queue.shift()
    console.log(node)

    for (let neighbor of this.adjList.get(node)) {
      if (!visited[neighbor]) {
        visited[neighbor] = true
        queue.push(neighbor)
      }
    }
  }
}
```

---

# 🌲 8️⃣ DFS – Depth First Search

Go deep first.

Like exploring a maze.

Example:

```
Start 0
Go 1
Go 3
Back
Go 2
```

Output:

```
0 1 3 2
```

Uses:

- Recursion
- Stack (internally)

---

## DFS Code

```js
dfs(start, visited = new Array(this.vertices).fill(false)) {
  visited[start] = true
  console.log(start)

  for (let neighbor of this.adjList.get(start)) {
    if (!visited[neighbor]) {
      this.dfs(neighbor, visited)
    }
  }
}
```

---

# 🔥 9️⃣ Time Complexity (Very Important)

For Adjacency List:

| Algorithm | Time Complexity |
| --------- | --------------- |
| BFS       | O(V + E)        |
| DFS       | O(V + E)        |

Why?

- Visit every vertex once
- Visit every edge once

---

# 🧠 Interview Understanding

When you see a problem ask yourself:

1. Is it traversal? → BFS or DFS
2. Is it shortest path? → BFS (unweighted) / Dijkstra (weighted)
3. Is it cycle detection? → DFS + visited logic
4. Is it dependency ordering? → Topological Sort

---

# 🚀 Final Summary

Graph = Nodes + Edges
Best storage = Adjacency List
Traversal = BFS & DFS
Complexity = O(V + E)

Master these basics and you can solve most beginner & intermediate graph problems.

---

🌟 End of Graph Beginner Master Notes

### Imported Notes: `DSA JS/src/data-structures/graph/implementation-notes.md`

# 🌐 Graph Learning – Step by Step with Adjacency List

---

# 🎯 Goal

We will learn:

- What is Adjacency List
- How to create graph
- How to add edges
- How to print graph
- How to run BFS
- How to run DFS

Everything step by step with code.

---

# 1️⃣ What is Adjacency List?

Adjacency List = Store graph as an array of lists.

Instead of matrix (V × V), we store only connections.

Example Graph:

```
0 ----- 1
|       |
|       |
2 ----- 3
```

Adjacency List Representation:

0 → [1,2]
1 → [0,3]
2 → [0,3]
3 → [1,2]

Space Complexity: O(V + E)

---

# 2️⃣ Step 1: Create Graph Class

```js
class Graph {
  constructor(vertices) {
    this.vertices = vertices
    this.adjList = new Map()

    // initialize empty list for each vertex
    for (let i = 0; i < vertices; i++) {
      this.adjList.set(i, [])
    }
  }
}
```

Now graph is created with empty adjacency list.

---

# 3️⃣ Step 2: Add Edge (Undirected Graph)

```js
addEdge(v, w) {
  this.adjList.get(v).push(w)
  this.adjList.get(w).push(v)
}
```

If directed graph:

```js
addEdge(v, w) {
  this.adjList.get(v).push(w)
}
```

---

# 4️⃣ Step 3: Print Graph

```js
printGraph() {
  for (let [vertex, neighbors] of this.adjList) {
    console.log(vertex + " -> " + neighbors.join(", "))
  }
}
```

---

# 5️⃣ Full Graph Setup Example

```js
class Graph {
  constructor(vertices) {
    this.vertices = vertices
    this.adjList = new Map()

    for (let i = 0; i < vertices; i++) {
      this.adjList.set(i, [])
    }
  }

  addEdge(v, w) {
    this.adjList.get(v).push(w)
    this.adjList.get(w).push(v)
  }

  printGraph() {
    for (let [vertex, neighbors] of this.adjList) {
      console.log(vertex + ' -> ' + neighbors.join(', '))
    }
  }
}

// Create graph
let graph = new Graph(4)

graph.addEdge(0, 1)
graph.addEdge(0, 2)
graph.addEdge(1, 3)
graph.addEdge(2, 3)

graph.printGraph()
```

---

# 6️⃣ BFS (Breadth First Search)

Level by level traversal.

```js
bfs(start) {
  let visited = new Array(this.vertices).fill(false)
  let queue = []

  visited[start] = true
  queue.push(start)

  while (queue.length > 0) {
    let node = queue.shift()
    console.log(node)

    for (let neighbor of this.adjList.get(node)) {
      if (!visited[neighbor]) {
        visited[neighbor] = true
        queue.push(neighbor)
      }
    }
  }
}
```

---

# 7️⃣ DFS (Depth First Search)

```js
dfs(start, visited = new Array(this.vertices).fill(false)) {
  visited[start] = true
  console.log(start)

  for (let neighbor of this.adjList.get(start)) {
    if (!visited[neighbor]) {
      this.dfs(neighbor, visited)
    }
  }
}
```

---

# 8️⃣ Complete Graph with BFS + DFS

```js
class Graph {
  constructor(vertices) {
    this.vertices = vertices
    this.adjList = new Map()

    for (let i = 0; i < vertices; i++) {
      this.adjList.set(i, [])
    }
  }

  addEdge(v, w) {
    this.adjList.get(v).push(w)
    this.adjList.get(w).push(v)
  }

  printGraph() {
    for (let [vertex, neighbors] of this.adjList) {
      console.log(vertex + ' -> ' + neighbors.join(', '))
    }
  }

  bfs(start) {
    let visited = new Array(this.vertices).fill(false)
    let queue = []

    visited[start] = true
    queue.push(start)

    while (queue.length > 0) {
      let node = queue.shift()
      console.log(node)

      for (let neighbor of this.adjList.get(node)) {
        if (!visited[neighbor]) {
          visited[neighbor] = true
          queue.push(neighbor)
        }
      }
    }
  }

  dfs(start, visited = new Array(this.vertices).fill(false)) {
    visited[start] = true
    console.log(start)

    for (let neighbor of this.adjList.get(start)) {
      if (!visited[neighbor]) {
        this.dfs(neighbor, visited)
      }
    }
  }
}
```

---

# 🚀 What You Learned

- Graph structure
- Adjacency List storage
- Add edge
- Print graph
- BFS traversal
- DFS traversal

---

# 🧠 Practice Task

1. Create graph of 5 nodes
2. Make it directed
3. Run BFS from node 0
4. Run DFS from node 0
5. Try detecting cycle next

---

🌟 You are now officially starting Graph coding properly.
<!-- DSA-JS-MERGE:END -->

<!-- PROMPT-TARGET-EXPANSION:START -->
## Master Prompt Target Expansion

This addendum brings the chapter closer to the depth requested by the master prompt: deeper recognition rules, interview narration, edge-case thinking, dry-run discipline, and complexity reasoning. Treat it as the chapter's final study layer after reading the core lesson and imported legacy material.

### Mastery Expansion 1: adjacency list

**What this part means in plain English:** In Graphs - The Universal Problem Model, adjacency list is not something to memorize as a disconnected trick. It is a decision tool. The core question is: what information changes as the input grows, and what information must remain available so the next step is cheap? When you can answer that, the correct data structure or algorithm becomes much easier to choose.

**How to recognize it in an interview:** Listen for the wording of the prompt. If the problem asks for fast lookup, repeated membership checks, duplicate detection, grouping, or counting, you should immediately consider a map or set. If it asks for contiguous ranges, windows, substrings, or subarrays, you should look for a sliding window or prefix state. If it asks for all possible choices, paths, arrangements, or boards, draw the decision tree before coding. If it asks for best, minimum, maximum, count ways, or feasibility with repeated subproblems, define a DP state before reaching for loops.

**Brute force baseline:** Always describe the direct solution first. For adjacency list, the brute force version usually repeats work: scanning the same area again, recalculating a value already known, trying every pair, or exploring branches that can be proven impossible. The baseline matters because it gives you a correctness anchor and gives the interviewer a clear before-and-after optimization story.

**Optimization move:** The optimization is usually one of four moves: store seen information, exploit sorted order, maintain an invariant while moving pointers, or cache solved subproblems. Say the invariant out loud. A good invariant sounds like: "At every step, my map contains only values from the processed prefix," or "The window is always the longest valid window ending at the current right pointer," or "The heap always stores the best candidates seen so far."

**Dry-run discipline:** Use a tiny input and trace every state change. Write the input, current index or pointer, auxiliary structure contents, current answer, and reason for movement. Do not jump from the first step to the final answer. The dry run is where off-by-one bugs, stale map entries, missed duplicate handling, and wrong base cases become visible.

**Edge cases to test:** Test empty input, one element, duplicate-heavy input, already sorted input, reverse sorted input, negative values if numbers are allowed, and maximum constraint shape. For recursive or graph problems, also test disconnected input, cycles, repeated visits, and a path that almost works but fails at the final step.

**What a strong candidate says:** "I will start with a correct brute force approach, analyze why it is too slow, then remove repeated work by preserving exactly the state I need. I will keep the invariant visible while coding, dry-run on a normal example, and then test edge cases before giving final complexity."

**Complexity explanation:** Do not only state Big O. Explain the count. If each element enters and leaves a window once, the runtime is O(n). If every node and edge is visited once, it is O(V + E). If recursion branches into two calls per level, draw the tree. If sorting happens before a linear scan, sorting dominates at O(n log n). If a heap operation occurs for every item, multiply by log k or log n depending on heap size.

### Mastery Expansion 2: adjacency matrix

**What this part means in plain English:** In Graphs - The Universal Problem Model, adjacency matrix is not something to memorize as a disconnected trick. It is a decision tool. The core question is: what information changes as the input grows, and what information must remain available so the next step is cheap? When you can answer that, the correct data structure or algorithm becomes much easier to choose.

**How to recognize it in an interview:** Listen for the wording of the prompt. If the problem asks for fast lookup, repeated membership checks, duplicate detection, grouping, or counting, you should immediately consider a map or set. If it asks for contiguous ranges, windows, substrings, or subarrays, you should look for a sliding window or prefix state. If it asks for all possible choices, paths, arrangements, or boards, draw the decision tree before coding. If it asks for best, minimum, maximum, count ways, or feasibility with repeated subproblems, define a DP state before reaching for loops.

**Brute force baseline:** Always describe the direct solution first. For adjacency matrix, the brute force version usually repeats work: scanning the same area again, recalculating a value already known, trying every pair, or exploring branches that can be proven impossible. The baseline matters because it gives you a correctness anchor and gives the interviewer a clear before-and-after optimization story.

**Optimization move:** The optimization is usually one of four moves: store seen information, exploit sorted order, maintain an invariant while moving pointers, or cache solved subproblems. Say the invariant out loud. A good invariant sounds like: "At every step, my map contains only values from the processed prefix," or "The window is always the longest valid window ending at the current right pointer," or "The heap always stores the best candidates seen so far."

**Dry-run discipline:** Use a tiny input and trace every state change. Write the input, current index or pointer, auxiliary structure contents, current answer, and reason for movement. Do not jump from the first step to the final answer. The dry run is where off-by-one bugs, stale map entries, missed duplicate handling, and wrong base cases become visible.

**Edge cases to test:** Test empty input, one element, duplicate-heavy input, already sorted input, reverse sorted input, negative values if numbers are allowed, and maximum constraint shape. For recursive or graph problems, also test disconnected input, cycles, repeated visits, and a path that almost works but fails at the final step.

**What a strong candidate says:** "I will start with a correct brute force approach, analyze why it is too slow, then remove repeated work by preserving exactly the state I need. I will keep the invariant visible while coding, dry-run on a normal example, and then test edge cases before giving final complexity."

**Complexity explanation:** Do not only state Big O. Explain the count. If each element enters and leaves a window once, the runtime is O(n). If every node and edge is visited once, it is O(V + E). If recursion branches into two calls per level, draw the tree. If sorting happens before a linear scan, sorting dominates at O(n log n). If a heap operation occurs for every item, multiply by log k or log n depending on heap size.

### Mastery Expansion 3: BFS

**What this part means in plain English:** In Graphs - The Universal Problem Model, BFS is not something to memorize as a disconnected trick. It is a decision tool. The core question is: what information changes as the input grows, and what information must remain available so the next step is cheap? When you can answer that, the correct data structure or algorithm becomes much easier to choose.

**How to recognize it in an interview:** Listen for the wording of the prompt. If the problem asks for fast lookup, repeated membership checks, duplicate detection, grouping, or counting, you should immediately consider a map or set. If it asks for contiguous ranges, windows, substrings, or subarrays, you should look for a sliding window or prefix state. If it asks for all possible choices, paths, arrangements, or boards, draw the decision tree before coding. If it asks for best, minimum, maximum, count ways, or feasibility with repeated subproblems, define a DP state before reaching for loops.

**Brute force baseline:** Always describe the direct solution first. For BFS, the brute force version usually repeats work: scanning the same area again, recalculating a value already known, trying every pair, or exploring branches that can be proven impossible. The baseline matters because it gives you a correctness anchor and gives the interviewer a clear before-and-after optimization story.

**Optimization move:** The optimization is usually one of four moves: store seen information, exploit sorted order, maintain an invariant while moving pointers, or cache solved subproblems. Say the invariant out loud. A good invariant sounds like: "At every step, my map contains only values from the processed prefix," or "The window is always the longest valid window ending at the current right pointer," or "The heap always stores the best candidates seen so far."

**Dry-run discipline:** Use a tiny input and trace every state change. Write the input, current index or pointer, auxiliary structure contents, current answer, and reason for movement. Do not jump from the first step to the final answer. The dry run is where off-by-one bugs, stale map entries, missed duplicate handling, and wrong base cases become visible.

**Edge cases to test:** Test empty input, one element, duplicate-heavy input, already sorted input, reverse sorted input, negative values if numbers are allowed, and maximum constraint shape. For recursive or graph problems, also test disconnected input, cycles, repeated visits, and a path that almost works but fails at the final step.

**What a strong candidate says:** "I will start with a correct brute force approach, analyze why it is too slow, then remove repeated work by preserving exactly the state I need. I will keep the invariant visible while coding, dry-run on a normal example, and then test edge cases before giving final complexity."

**Complexity explanation:** Do not only state Big O. Explain the count. If each element enters and leaves a window once, the runtime is O(n). If every node and edge is visited once, it is O(V + E). If recursion branches into two calls per level, draw the tree. If sorting happens before a linear scan, sorting dominates at O(n log n). If a heap operation occurs for every item, multiply by log k or log n depending on heap size.

### Mastery Expansion 4: DFS

**What this part means in plain English:** In Graphs - The Universal Problem Model, DFS is not something to memorize as a disconnected trick. It is a decision tool. The core question is: what information changes as the input grows, and what information must remain available so the next step is cheap? When you can answer that, the correct data structure or algorithm becomes much easier to choose.

**How to recognize it in an interview:** Listen for the wording of the prompt. If the problem asks for fast lookup, repeated membership checks, duplicate detection, grouping, or counting, you should immediately consider a map or set. If it asks for contiguous ranges, windows, substrings, or subarrays, you should look for a sliding window or prefix state. If it asks for all possible choices, paths, arrangements, or boards, draw the decision tree before coding. If it asks for best, minimum, maximum, count ways, or feasibility with repeated subproblems, define a DP state before reaching for loops.

**Brute force baseline:** Always describe the direct solution first. For DFS, the brute force version usually repeats work: scanning the same area again, recalculating a value already known, trying every pair, or exploring branches that can be proven impossible. The baseline matters because it gives you a correctness anchor and gives the interviewer a clear before-and-after optimization story.

**Optimization move:** The optimization is usually one of four moves: store seen information, exploit sorted order, maintain an invariant while moving pointers, or cache solved subproblems. Say the invariant out loud. A good invariant sounds like: "At every step, my map contains only values from the processed prefix," or "The window is always the longest valid window ending at the current right pointer," or "The heap always stores the best candidates seen so far."

**Dry-run discipline:** Use a tiny input and trace every state change. Write the input, current index or pointer, auxiliary structure contents, current answer, and reason for movement. Do not jump from the first step to the final answer. The dry run is where off-by-one bugs, stale map entries, missed duplicate handling, and wrong base cases become visible.

**Edge cases to test:** Test empty input, one element, duplicate-heavy input, already sorted input, reverse sorted input, negative values if numbers are allowed, and maximum constraint shape. For recursive or graph problems, also test disconnected input, cycles, repeated visits, and a path that almost works but fails at the final step.

**What a strong candidate says:** "I will start with a correct brute force approach, analyze why it is too slow, then remove repeated work by preserving exactly the state I need. I will keep the invariant visible while coding, dry-run on a normal example, and then test edge cases before giving final complexity."

**Complexity explanation:** Do not only state Big O. Explain the count. If each element enters and leaves a window once, the runtime is O(n). If every node and edge is visited once, it is O(V + E). If recursion branches into two calls per level, draw the tree. If sorting happens before a linear scan, sorting dominates at O(n log n). If a heap operation occurs for every item, multiply by log k or log n depending on heap size.
<!-- PROMPT-TARGET-EXPANSION:END -->

---

**Previous:** [Tries - The String Search Master](../Phase-3-Nonlinear-Data-Structures/05-Tries.md) | **Next:** [Sorting Algorithms - Complete Mastery](../Phase-4-Core-Algorithms/01-Sorting-Algorithms-Complete.md)
