# Trees and Binary Trees - Complete Foundation

## Chapter Metadata

| Field | Value |
|---|---|
| Phase | Phase 3 - Nonlinear Data Structures |
| Chapter | 11 of 37 |
| Difficulty | Intermediate |
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

- Root, parent, child, leaf, height, depth, subtree, and edge terminology
- Full, complete, perfect, balanced, and skewed binary trees
- Recursive and iterative inorder, preorder, postorder, and level-order traversal
- Depth, invert, symmetric, LCA, path sum, max path sum, serialize/deserialize, diameter

## Deep Teaching Notes

### 1. Root, parent, child, leaf, height, depth, subtree, and edge terminology

**Beginner explanation:** This is one of the core ideas for Trees and Binary Trees - Complete Foundation. Start by saying it in plain language before reaching for code. A beginner should understand what problem this idea solves, what input it expects, and what output it creates.

**Why it matters:** In a FAANG interview, this point shows whether you understand the shape of the problem. Interviewers care less about memorized syntax and more about whether your choices match the constraints.

**How to reason about it:** Ask what must be remembered while the algorithm runs. If you need fast lookup, think HashMap or Set. If you need ordered movement, think pointers. If you need all possibilities, think recursion or backtracking. If you need best/count/possible over repeated subproblems, think dynamic programming.

**What to say out loud:** "I am choosing this approach because it matches the constraint: the expensive operation is repeated work, so I want a structure or pattern that removes that repetition."

**Implementation angle in JavaScript:** Prefer clear names, explicit loops when teaching, and built-ins only when you can explain their complexity. JavaScript gives you Array, Map, Set, and flexible objects, but every helper method still has a cost.

**Edge checks:** Confirm behavior for empty input, one item, duplicate values, already-ordered input, reverse-ordered input, and values at the smallest or largest allowed constraints.

### 2. Full, complete, perfect, balanced, and skewed binary trees

**Beginner explanation:** This is one of the core ideas for Trees and Binary Trees - Complete Foundation. Start by saying it in plain language before reaching for code. A beginner should understand what problem this idea solves, what input it expects, and what output it creates.

**Why it matters:** In a FAANG interview, this point shows whether you understand the shape of the problem. Interviewers care less about memorized syntax and more about whether your choices match the constraints.

**How to reason about it:** Ask what must be remembered while the algorithm runs. If you need fast lookup, think HashMap or Set. If you need ordered movement, think pointers. If you need all possibilities, think recursion or backtracking. If you need best/count/possible over repeated subproblems, think dynamic programming.

**What to say out loud:** "I am choosing this approach because it matches the constraint: the expensive operation is repeated work, so I want a structure or pattern that removes that repetition."

**Implementation angle in JavaScript:** Prefer clear names, explicit loops when teaching, and built-ins only when you can explain their complexity. JavaScript gives you Array, Map, Set, and flexible objects, but every helper method still has a cost.

**Edge checks:** Confirm behavior for empty input, one item, duplicate values, already-ordered input, reverse-ordered input, and values at the smallest or largest allowed constraints.

### 3. Recursive and iterative inorder, preorder, postorder, and level-order traversal

**Beginner explanation:** This is one of the core ideas for Trees and Binary Trees - Complete Foundation. Start by saying it in plain language before reaching for code. A beginner should understand what problem this idea solves, what input it expects, and what output it creates.

**Why it matters:** In a FAANG interview, this point shows whether you understand the shape of the problem. Interviewers care less about memorized syntax and more about whether your choices match the constraints.

**How to reason about it:** Ask what must be remembered while the algorithm runs. If you need fast lookup, think HashMap or Set. If you need ordered movement, think pointers. If you need all possibilities, think recursion or backtracking. If you need best/count/possible over repeated subproblems, think dynamic programming.

**What to say out loud:** "I am choosing this approach because it matches the constraint: the expensive operation is repeated work, so I want a structure or pattern that removes that repetition."

**Implementation angle in JavaScript:** Prefer clear names, explicit loops when teaching, and built-ins only when you can explain their complexity. JavaScript gives you Array, Map, Set, and flexible objects, but every helper method still has a cost.

**Edge checks:** Confirm behavior for empty input, one item, duplicate values, already-ordered input, reverse-ordered input, and values at the smallest or largest allowed constraints.

### 4. Depth, invert, symmetric, LCA, path sum, max path sum, serialize/deserialize, diameter

**Beginner explanation:** This is one of the core ideas for Trees and Binary Trees - Complete Foundation. Start by saying it in plain language before reaching for code. A beginner should understand what problem this idea solves, what input it expects, and what output it creates.

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

- `DSA JS/src/data-structures/tree/notes.md`
- `DSA JS/src/data-structures/tree/implementation.js`
- `DSA JS/src/data-structures/tree/traversal/bfs/notes.md`
- `DSA JS/src/data-structures/tree/traversal/dfs/basic.md`
- `DSA JS/src/data-structures/tree/traversal/dfs/node.md`
- `DSA JS/src/data-structures/tree/traversal/dfs/traversal.md`
- `DSA JS/src/data-structures/tree/traversal/dfs/complete-binary-tree-traversal.md`

### Imported Notes: `DSA JS/src/data-structures/tree/notes.md`

# 🌳 Important Tree Problems – Complete Learning Notes

---

# 1️⃣ Example Tree Used in All Problems

```
        1
      /   \
     2     3
    / \   / \
   4   5 6   7
```

---

# 2️⃣ Count of Nodes

## 📌 Problem

Count total number of nodes in a binary tree.

## 🧠 Idea

Every node contributes 1 + left subtree count + right subtree count.

## ✅ Recursive Formula

Count(root) =
1 + Count(left) + Count(right)

## 💻 Code

```js
function countNodes(root) {
  if (!root) return 0

  return 1 + countNodes(root.left) + countNodes(root.right)
}
```

## ⏱ Complexity

Time: O(n)
Space: O(h)

---

# 3️⃣ Sum of All Nodes

## 📌 Problem

Find sum of all node values in tree.

## 🧠 Idea

Root value + sum(left) + sum(right)

## 💻 Code

```js
function sumNodes(root) {
  if (!root) return 0

  return root.value + sumNodes(root.left) + sumNodes(root.right)
}
```

## ⏱ Complexity

Time: O(n)
Space: O(h)

---

# 4️⃣ Height of Tree

## 📌 Problem

Find height of tree.

Height = Maximum number of edges from root to leaf.

## 🧠 Idea

Height(root) =
1 + max(height(left), height(right))

## 💻 Code

```js
function height(root) {
  if (!root) return -1 // edge-based height

  return 1 + Math.max(height(root.left), height(root.right))
}
```

## ⏱ Complexity

Time: O(n)
Space: O(h)

---

# 5️⃣ Diameter of Tree

## 📌 Problem

Diameter = Longest path between any two nodes.

Path may or may not pass through root.

## 🧠 Idea

Diameter at root =
height(left) + height(right)

We check for every node.

## 💻 Code (Optimized O(n))

```js
let diameter = 0

function findHeight(root) {
  if (!root) return 0

  let left = findHeight(root.left)
  let right = findHeight(root.right)

  diameter = Math.max(diameter, left + right)

  return 1 + Math.max(left, right)
}

function getDiameter(root) {
  diameter = 0
  findHeight(root)
  return diameter
}
```

## ⏱ Complexity

Time: O(n)
Space: O(h)

---

# 6️⃣ Sum of Kth Level

## 📌 Problem

Find sum of nodes at level K.

Level starts from 0 (root level = 0)

## 🧠 Idea

Use BFS (Queue) and track level.

## 💻 Code

```js
function sumAtKLevel(root, k) {
  if (!root) return 0

  let queue = [root]
  let level = 0

  while (queue.length > 0) {
    let size = queue.length

    if (level === k) {
      let sum = 0
      for (let node of queue) {
        sum += node.value
      }
      return sum
    }

    for (let i = 0; i < size; i++) {
      let node = queue.shift()

      if (node.left) queue.push(node.left)
      if (node.right) queue.push(node.right)
    }

    level++
  }

  return 0
}
```

## ⏱ Complexity

Time: O(n)
Space: O(n)

---

# 7️⃣ Complete Working Setup

```js
class Node {
  constructor(value) {
    this.value = value
    this.left = null
    this.right = null
  }
}

let root = new Node(1)
root.left = new Node(2)
root.right = new Node(3)
root.left.left = new Node(4)
root.left.right = new Node(5)
root.right.left = new Node(6)
root.right.right = new Node(7)

console.log('Count:', countNodes(root))
console.log('Sum:', sumNodes(root))
console.log('Height:', height(root))
console.log('Diameter:', getDiameter(root))
console.log('Sum at level 2:', sumAtKLevel(root, 2))
```

---

# 🔥 Final Revision Summary

- Count = 1 + left + right
- Sum = value + left + right
- Height = 1 + max(left, right)
- Diameter = leftHeight + rightHeight
- Kth level sum = BFS level tracking

Master these 5 → You are strong in Tree recursion 🚀

### Imported Implementation: `DSA JS/src/data-structures/tree/implementation.js`

```javascript
class TreeNode {
  constructor(value) {
    this.value = value
    this.left = null
    this.right = null
  }

  // preorder
  preOrder(root) {
    if (root === null) return
    console.log(root.value)
    this.preOrder(root.left)
    this.preOrder(root.right)
  }

  // inorder
  inOrder(root) {
    if (root === null) return
    this.inOrder(root.left)
    console.log(root.value)
    this.inOrder(root.right)
  }

  // post order

  postOrder(root) {
    if (root === null) return
    this.postOrder(root.left)
    this.postOrder(root.right)
    console.log(root.value)
  }

  //   level order
  levelOrder(root) {
    if (!root) return

    let queue = [root]

    while (queue.length > 0) {
      let node = queue.shift()
      console.log(node.value)
      if (node.left) queue.push(node.left)
      if (node.right) queue.push(node.right)
    }
  }

  //   count node
  countNode(root) {
    if (!root) return 0
    return 1 + this.countNode(root.left) + this.countNode(root.right)
  }

  sumOfNode(root) {
    if (!root) return 0
    return root.value + this.sumOfNode(root.left) + this.sumOfNode(root.right)
  }

  height(root) {
    if (!root) return -1 // edge-based height

    return 1 + Math.max(this.height(root.left), this.height(root.right))
  }
}

const root = new TreeNode(1)
root.left = new TreeNode(2)
root.right = new TreeNode(3)
root.left.left = new TreeNode(4)
root.left.right = new TreeNode(5)
root.right.left = new TreeNode(6)
root.right.right = new TreeNode(7)

console.log('Pre order')
root.preOrder(root)
console.log('level order')
root.levelOrder(root)
console.log('count the nodes')
console.log(root.countNode(root))
console.log('sum of nodes is ')
console.log(root.sumOfNode(root))
console.log('Height')
console.log(root.height(root))
```

### Imported Notes: `DSA JS/src/data-structures/tree/traversal/bfs/notes.md`

# 🌳 Tree Traversal – Level Wise (BFS) Notes

---

# 1️⃣ What is Level Wise Traversal?

Level Wise Traversal = Visiting all nodes **level by level**, from top to bottom.

Also called **Breadth First Search (BFS)**.

Think: "Read tree row by row"

---

# 2️⃣ Example Tree

```
        1
      /   \
     2     3
    / \   / \
   4   5 6   7
```

---

# 3️⃣ Algorithm Steps

1. Create a queue and enqueue root node.
2. While queue is not empty:
   - Dequeue a node
   - Print its value
   - Enqueue its left child (if exists)
   - Enqueue its right child (if exists)

---

# 4️⃣ JavaScript Code (Level Order Traversal)

```js
class Node {
  constructor(value) {
    this.value = value
    this.left = null
    this.right = null
  }
}

// Create tree
let root = new Node(1)
root.left = new Node(2)
root.right = new Node(3)
root.left.left = new Node(4)
root.left.right = new Node(5)
root.right.left = new Node(6)
root.right.right = new Node(7)

function levelOrder(root) {
  if (!root) return

  let queue = [root]

  while (queue.length > 0) {
    let node = queue.shift()
    console.log(node.value)

    if (node.left) queue.push(node.left)
    if (node.right) queue.push(node.right)
  }
}

console.log('Level Order Traversal:')
levelOrder(root)
```

---

# 5️⃣ Expected Output

```
1
2
3
4
5
6
7
```

---

# 6️⃣ Notes / Key Points

- Uses **Queue** data structure
- Visits nodes **level by level**
- Time Complexity: O(n)
- Space Complexity: O(n) (for queue)
- Useful for:
  - Finding shortest path in tree
  - Printing levels
  - BFS-based tree problems

---

# 7️⃣ Quick Comparison with DFS

| Traversal Type   | Order          | Data Structure  | Use Case                      |
| ---------------- | -------------- | --------------- | ----------------------------- |
| Inorder (DFS)    | L R Root       | Recursion/Stack | BST sorted output             |
| Preorder (DFS)   | Root L R       | Recursion/Stack | Copy/Serialize tree           |
| Postorder(DFS)   | L R Root       | Recursion/Stack | Delete tree, height calc      |
| Level Order(BFS) | Level by level | Queue           | Shortest path, level printing |

---

# 8️⃣ Visualization

Level 1: 1

Level 2: 2 3

Level 3: 4 5 6 7

---

# 9️⃣ Revision Summary

- Level Order = BFS = Top to bottom, left to right
- Use queue to maintain order
- Visit all nodes at current level before next level
- Time O(n), Space O(n)

### Imported Notes: `DSA JS/src/data-structures/tree/traversal/dfs/basic.md`

# 🌳 Tree Fundamentals (Core Structural Terminology)

> These are foundational concepts used in Data Structures, Databases, File Systems, Compilers, and Distributed Systems.

---

# 1️⃣ Basic Tree Example (Reference Diagram)

We will use this tree for understanding all terms:

                A
              /   \
             B     C
            / \     \
           D   E     F
              /
             G

---

# 2️⃣ Parent

## 📌 Definition

A **parent** is a node that has one or more children.

If there is an edge from node `u` to node `v`,
then:

- `u` = Parent
- `v` = Child

## 📌 Examples (From Diagram)

- A is parent of B and C
- B is parent of D and E
- E is parent of G

## 📌 Formal Definition

If `(u → v)` is an edge, then `u` is parent of `v`.

## 📌 Properties

- Every node except root has exactly ONE parent.
- Root has NO parent.

---

# 3️⃣ Child

## 📌 Definition

A **child** is a node directly connected below another node.

## 📌 Examples

- B and C are children of A
- D and E are children of B
- G is child of E

## 📌 Types

- Left Child
- Right Child (in Binary Trees)

---

# 4️⃣ Ancestor

## 📌 Definition

An **ancestor** of a node is any node on the path from root to that node.

Includes:

- Parent
- Grandparent
- Root

## 📌 Example (Node G)

Path from Root → G:
A → B → E → G

Ancestors of G:

- A
- B
- E

## 📌 Important

Every node is NOT considered its own ancestor (in most definitions).

## 📌 Time Complexity Insight

Finding ancestors requires:

- O(h) where h = height of tree

---

# 5️⃣ Subtree

## 📌 Definition

A **subtree** is a tree formed by a node and all its descendants.

Every node can be considered root of its own subtree.

## 📌 Example

Subtree rooted at B:

            B
           / \
          D   E
             /
            G

Subtree rooted at E:

            E
           /
          G

## 📌 Important Property

Total number of subtrees in a tree = number of nodes.

---

# 6️⃣ Depth

## 📌 Definition

Depth of a node = number of edges from root to that node.

Formula:
Depth(node) = Distance from root

## 📌 Example

Node A:
Depth = 0

Node B:
Depth = 1

Node G:
Depth = 3

## 📌 Formula Insight

If root depth = 0:
Depth = Level - 1

---

# 7️⃣ Level

## 📌 Definition

Level of a node = number of nodes from root to that node (including root).

Alternative Definition:
Level = Depth + 1

## 📌 Example

Node A:
Level = 1

Node B:
Level = 2

Node G:
Level = 4

---

# 8️⃣ Depth vs Level (Interview Difference)

| Concept | Definition                | Root Value |
| ------- | ------------------------- | ---------- |
| Depth   | Number of edges from root | 0          |
| Level   | Number of nodes from root | 1          |

Relation:
Level = Depth + 1

---

# 9️⃣ Visual Depth & Level Table

| Node | Depth | Level | Parent |
| ---- | ----- | ----- | ------ |
| A    | 0     | 1     | NULL   |
| B    | 1     | 2     | A      |
| C    | 1     | 2     | A      |
| D    | 2     | 3     | B      |
| E    | 2     | 3     | B      |
| F    | 2     | 3     | C      |
| G    | 3     | 4     | E      |

---

# 🔟 Interview-Level Observations

1. Height of Tree = Max Depth
2. Nodes at same depth are on same level.
3. Number of ancestors of a node = Depth of node.
4. Every node defines a subtree.
5. Root has:
   - No parent
   - Depth = 0
   - Level = 1

---

### Imported Notes: `DSA JS/src/data-structures/tree/traversal/dfs/node.md`

# 🌳 Tree Data Structure – Beginner Starter Notes

---

# 1️⃣ What is a Tree?

A **Tree** is a non-linear data structure made of nodes connected by edges.

It represents hierarchical data.

Examples in real life:

- File System
- Organization Structure
- DOM (HTML structure)

---

# 2️⃣ Basic Terminology

## 📌 Node

Each element in a tree is called a node.

## 📌 Edge

Connection between two nodes.

## 📌 Root

Topmost node of the tree.

- Only one root in a tree.
- Has no parent.

Example:

        A
       / \
      B   C

Here:

- A = Root

---

# 3️⃣ Parent and Child

If a node is connected below another node:

Upper node → Parent  
Lower node → Child

Example:

        A
       / \
      B   C

- A is parent of B and C
- B and C are children of A

---

# 4️⃣ Leaf Node

A node with NO children.

Example:

        A
       / \
      B   C
     /
    D

Leaf nodes:

- D
- C

---

# 5️⃣ Depth

Depth = Number of edges from root to that node.

Root depth = 0

Example:

        A
       /
      B
     /
    C

Depth of:
A = 0  
B = 1  
C = 2

---

# 6️⃣ Height

Height = Maximum depth in the tree.

In above example:
Height = 2

---

# 7️⃣ Subtree

Subtree = A node and all its children.

Example:

        A
       / \
      B   C
     /
    D

Subtree of B:

      B
     /
    D

---

# 8️⃣ Types of Trees (Basic)

## 1. Binary Tree

Each node has at most 2 children.

## 2. Binary Search Tree (BST)

Left < Root < Right

---

# 9️⃣ Basic Binary Tree Structure (JavaScript)

```js
class Node {
  constructor(value) {
    this.value = value
    this.left = null
    this.right = null
  }
}

let root = new Node(1)
root.left = new Node(2)
root.right = new Node(3)



// Diagram


    1
   / \
  2   3



---

# 🔟 Why Tree is Important?

Used in:
- Searching (BST)
- Heaps
- File systems
- Databases
- Networking
- AI decision making

---

# 🧠 Interview Tip

Tree is based on:
- Recursion
- DFS
- BFS

If you master recursion → Tree becomes easy.

---

# 🚀 Quick Revision

- Tree = Nodes + Edges
- Root = Top node
- Leaf = No children
- Depth = Distance from root
- Height = Max depth
- Subtree = Node + descendants
- Binary Tree = Max 2 children

---
```

### Imported Notes: `DSA JS/src/data-structures/tree/traversal/dfs/traversal.md`

# 🌳 Tree Traversal – Super Simple Beginner Notes

---

# 1️⃣ What is Tree Traversal?

Tree Traversal = Visiting every node of a tree exactly once.

Think like:
👉 "How do I read the whole tree?"

---

# 2️⃣ Example Tree (We Will Use This)

```
        1
      /   \
     2     3
    / \
   4   5
```

---

# 3️⃣ Types of Tree Traversal

There are TWO main categories:

1. DFS (Depth First Search)
   - Inorder
   - Preorder
   - Postorder

2. BFS (Breadth First Search)
   - Level Order Traversal

---

# 🌿 PART 1: DFS Traversals

DFS = Go deep first, then come back.

Important Rule:
We use RECURSION.

---

# 4️⃣ Inorder Traversal (Left → Root → Right)

Order:

1. Go Left
2. Print Root
3. Go Right

Memory Trick:
👉 L R Root

Example Output:
4 → 2 → 5 → 1 → 3

```js
function inorder(root) {
  if (root === null) return
  inorder(root.left)
  console.log(root.value)
  inorder(root.right)
}
```

---

# 5️⃣ Preorder Traversal (Root → Left → Right)

Order:

1. Print Root
2. Go Left
3. Go Right

Memory Trick:
👉 Root L R

Example Output:
1 → 2 → 4 → 5 → 3

```js
function preorder(root) {
  if (root === null) return
  console.log(root.value)
  preorder(root.left)
  preorder(root.right)
}
```

---

# 6️⃣ Postorder Traversal (Left → Right → Root)

Order:

1. Go Left
2. Go Right
3. Print Root

Memory Trick:
👉 L R Root

Example Output:
4 → 5 → 2 → 3 → 1

```js
function postorder(root) {
  if (root === null) return
  postorder(root.left)
  postorder(root.right)
  console.log(root.value)
}
```

---

# 🌊 PART 2: BFS Traversal

## Level Order Traversal (Level by Level)

Visit nodes row by row using a queue.

Example Output:
1 → 2 → 3 → 4 → 5

```js
function levelOrder(root) {
  if (!root) return
  let queue = [root]
  while (queue.length > 0) {
    let node = queue.shift()
    console.log(node.value)
    if (node.left) queue.push(node.left)
    if (node.right) queue.push(node.right)
  }
}
```

---

# 7️⃣ Traversal Summary Table

| Traversal   | Output    |
| ----------- | --------- |
| Inorder     | 4 2 5 1 3 |
| Preorder    | 1 2 4 5 3 |
| Postorder   | 4 5 2 3 1 |
| Level Order | 1 2 3 4 5 |

---

# 8️⃣ Time & Space Complexity

- Time Complexity: O(n) for all traversals
- Space Complexity: O(h) for DFS (recursion stack), O(n) for BFS (queue)

Where h = height of tree

---

# 9️⃣ Quick Tips

- DFS → Recursion
- BFS → Queue
- Inorder → Sorted order in BST
- Preorder → Used for copying tree
- Postorder → Useful for deletion
- Level Order → Shortest path / levels

---

# ✅ End of Tree Traversal Notes

### Imported Notes: `DSA JS/src/data-structures/tree/traversal/dfs/complete-binary-tree-traversal.md`

```js
class Node {
  constructor(value) {
    this.value = value
    this.left = null
    this.right = null
  }
}

// Step 2️⃣: Create Sample Tree
/*
            1
          /   \
         2     3
        / \
       4   5
*/

let root = new Node(1)
root.left = new Node(2)
root.right = new Node(3)
root.left.left = new Node(4)root.left.right = new Node(5)


// =============================
// 🔹 Inorder Traversal
// Left → Root → Right
// =============================

function inorder(root) {
  if (root === null) return

  inorder(root.left)
  console.log(root.value)
  inorder(root.right)
}

// =============================
// 🔹 Preorder Traversal
// Root → Left → Right
// =============================

function preorder(root) {
  if (root === null) return

  console.log(root.value)
  preorder(root.left)
  preorder(root.right)
}

// =============================
// 🔹 Postorder Traversal
// Left → Right → Root
// =============================

function postorder(root) {
  if (root === null) return

  postorder(root.left)
  postorder(root.right)
  console.log(root.value)
}

// =============================
// 🚀 Run All Traversals
// =============================

console.log('Inorder Traversal:')
inorder(root)

console.log('Preorder Traversal:')
preorder(root)

console.log('Postorder Traversal:')
postorder(root)
```
<!-- DSA-JS-MERGE:END -->

<!-- PROMPT-TARGET-EXPANSION:START -->
## Master Prompt Target Expansion

This addendum brings the chapter closer to the depth requested by the master prompt: deeper recognition rules, interview narration, edge-case thinking, dry-run discipline, and complexity reasoning. Treat it as the chapter's final study layer after reading the core lesson and imported legacy material.

### Mastery Expansion 1: recursive DFS

**What this part means in plain English:** In Trees and Binary Trees - Complete Foundation, recursive DFS is not something to memorize as a disconnected trick. It is a decision tool. The core question is: what information changes as the input grows, and what information must remain available so the next step is cheap? When you can answer that, the correct data structure or algorithm becomes much easier to choose.

**How to recognize it in an interview:** Listen for the wording of the prompt. If the problem asks for fast lookup, repeated membership checks, duplicate detection, grouping, or counting, you should immediately consider a map or set. If it asks for contiguous ranges, windows, substrings, or subarrays, you should look for a sliding window or prefix state. If it asks for all possible choices, paths, arrangements, or boards, draw the decision tree before coding. If it asks for best, minimum, maximum, count ways, or feasibility with repeated subproblems, define a DP state before reaching for loops.

**Brute force baseline:** Always describe the direct solution first. For recursive DFS, the brute force version usually repeats work: scanning the same area again, recalculating a value already known, trying every pair, or exploring branches that can be proven impossible. The baseline matters because it gives you a correctness anchor and gives the interviewer a clear before-and-after optimization story.

**Optimization move:** The optimization is usually one of four moves: store seen information, exploit sorted order, maintain an invariant while moving pointers, or cache solved subproblems. Say the invariant out loud. A good invariant sounds like: "At every step, my map contains only values from the processed prefix," or "The window is always the longest valid window ending at the current right pointer," or "The heap always stores the best candidates seen so far."

**Dry-run discipline:** Use a tiny input and trace every state change. Write the input, current index or pointer, auxiliary structure contents, current answer, and reason for movement. Do not jump from the first step to the final answer. The dry run is where off-by-one bugs, stale map entries, missed duplicate handling, and wrong base cases become visible.

**Edge cases to test:** Test empty input, one element, duplicate-heavy input, already sorted input, reverse sorted input, negative values if numbers are allowed, and maximum constraint shape. For recursive or graph problems, also test disconnected input, cycles, repeated visits, and a path that almost works but fails at the final step.

**What a strong candidate says:** "I will start with a correct brute force approach, analyze why it is too slow, then remove repeated work by preserving exactly the state I need. I will keep the invariant visible while coding, dry-run on a normal example, and then test edge cases before giving final complexity."

**Complexity explanation:** Do not only state Big O. Explain the count. If each element enters and leaves a window once, the runtime is O(n). If every node and edge is visited once, it is O(V + E). If recursion branches into two calls per level, draw the tree. If sorting happens before a linear scan, sorting dominates at O(n log n). If a heap operation occurs for every item, multiply by log k or log n depending on heap size.

### Mastery Expansion 2: iterative DFS

**What this part means in plain English:** In Trees and Binary Trees - Complete Foundation, iterative DFS is not something to memorize as a disconnected trick. It is a decision tool. The core question is: what information changes as the input grows, and what information must remain available so the next step is cheap? When you can answer that, the correct data structure or algorithm becomes much easier to choose.

**How to recognize it in an interview:** Listen for the wording of the prompt. If the problem asks for fast lookup, repeated membership checks, duplicate detection, grouping, or counting, you should immediately consider a map or set. If it asks for contiguous ranges, windows, substrings, or subarrays, you should look for a sliding window or prefix state. If it asks for all possible choices, paths, arrangements, or boards, draw the decision tree before coding. If it asks for best, minimum, maximum, count ways, or feasibility with repeated subproblems, define a DP state before reaching for loops.

**Brute force baseline:** Always describe the direct solution first. For iterative DFS, the brute force version usually repeats work: scanning the same area again, recalculating a value already known, trying every pair, or exploring branches that can be proven impossible. The baseline matters because it gives you a correctness anchor and gives the interviewer a clear before-and-after optimization story.

**Optimization move:** The optimization is usually one of four moves: store seen information, exploit sorted order, maintain an invariant while moving pointers, or cache solved subproblems. Say the invariant out loud. A good invariant sounds like: "At every step, my map contains only values from the processed prefix," or "The window is always the longest valid window ending at the current right pointer," or "The heap always stores the best candidates seen so far."

**Dry-run discipline:** Use a tiny input and trace every state change. Write the input, current index or pointer, auxiliary structure contents, current answer, and reason for movement. Do not jump from the first step to the final answer. The dry run is where off-by-one bugs, stale map entries, missed duplicate handling, and wrong base cases become visible.

**Edge cases to test:** Test empty input, one element, duplicate-heavy input, already sorted input, reverse sorted input, negative values if numbers are allowed, and maximum constraint shape. For recursive or graph problems, also test disconnected input, cycles, repeated visits, and a path that almost works but fails at the final step.

**What a strong candidate says:** "I will start with a correct brute force approach, analyze why it is too slow, then remove repeated work by preserving exactly the state I need. I will keep the invariant visible while coding, dry-run on a normal example, and then test edge cases before giving final complexity."

**Complexity explanation:** Do not only state Big O. Explain the count. If each element enters and leaves a window once, the runtime is O(n). If every node and edge is visited once, it is O(V + E). If recursion branches into two calls per level, draw the tree. If sorting happens before a linear scan, sorting dominates at O(n log n). If a heap operation occurs for every item, multiply by log k or log n depending on heap size.
<!-- PROMPT-TARGET-EXPANSION:END -->

---

**Previous:** [Hash Tables and Hash Maps - The Speed Secret](../Phase-2-Linear-Data-Structures/05-Hash-Tables-Hash-Maps.md) | **Next:** [Binary Search Trees - The Sorted Tree](../Phase-3-Nonlinear-Data-Structures/02-Binary-Search-Trees.md)
