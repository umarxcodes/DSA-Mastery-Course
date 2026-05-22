# Doubly Linked List and Circular Linked List

## Chapter Metadata

| Field | Value |
|---|---|
| Phase | Phase 2 - Linear Data Structures |
| Chapter | 7 of 37 |
| Difficulty | Intermediate |
| Time to Master | 6-8 hours |
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

- prev and next pointers, reverse traversal, and O(1) deletion given a node
- Doubly linked list implementation with insert/remove/reverse
- Circular list tail-to-head behavior and round-robin use cases
- LRU Cache using doubly linked list plus HashMap with O(1) get/put

## Deep Teaching Notes

### 1. prev and next pointers, reverse traversal, and O(1) deletion given a node

**Beginner explanation:** This is one of the core ideas for Doubly Linked List and Circular Linked List. Start by saying it in plain language before reaching for code. A beginner should understand what problem this idea solves, what input it expects, and what output it creates.

**Why it matters:** In a FAANG interview, this point shows whether you understand the shape of the problem. Interviewers care less about memorized syntax and more about whether your choices match the constraints.

**How to reason about it:** Ask what must be remembered while the algorithm runs. If you need fast lookup, think HashMap or Set. If you need ordered movement, think pointers. If you need all possibilities, think recursion or backtracking. If you need best/count/possible over repeated subproblems, think dynamic programming.

**What to say out loud:** "I am choosing this approach because it matches the constraint: the expensive operation is repeated work, so I want a structure or pattern that removes that repetition."

**Implementation angle in JavaScript:** Prefer clear names, explicit loops when teaching, and built-ins only when you can explain their complexity. JavaScript gives you Array, Map, Set, and flexible objects, but every helper method still has a cost.

**Edge checks:** Confirm behavior for empty input, one item, duplicate values, already-ordered input, reverse-ordered input, and values at the smallest or largest allowed constraints.

### 2. Doubly linked list implementation with insert/remove/reverse

**Beginner explanation:** This is one of the core ideas for Doubly Linked List and Circular Linked List. Start by saying it in plain language before reaching for code. A beginner should understand what problem this idea solves, what input it expects, and what output it creates.

**Why it matters:** In a FAANG interview, this point shows whether you understand the shape of the problem. Interviewers care less about memorized syntax and more about whether your choices match the constraints.

**How to reason about it:** Ask what must be remembered while the algorithm runs. If you need fast lookup, think HashMap or Set. If you need ordered movement, think pointers. If you need all possibilities, think recursion or backtracking. If you need best/count/possible over repeated subproblems, think dynamic programming.

**What to say out loud:** "I am choosing this approach because it matches the constraint: the expensive operation is repeated work, so I want a structure or pattern that removes that repetition."

**Implementation angle in JavaScript:** Prefer clear names, explicit loops when teaching, and built-ins only when you can explain their complexity. JavaScript gives you Array, Map, Set, and flexible objects, but every helper method still has a cost.

**Edge checks:** Confirm behavior for empty input, one item, duplicate values, already-ordered input, reverse-ordered input, and values at the smallest or largest allowed constraints.

### 3. Circular list tail-to-head behavior and round-robin use cases

**Beginner explanation:** This is one of the core ideas for Doubly Linked List and Circular Linked List. Start by saying it in plain language before reaching for code. A beginner should understand what problem this idea solves, what input it expects, and what output it creates.

**Why it matters:** In a FAANG interview, this point shows whether you understand the shape of the problem. Interviewers care less about memorized syntax and more about whether your choices match the constraints.

**How to reason about it:** Ask what must be remembered while the algorithm runs. If you need fast lookup, think HashMap or Set. If you need ordered movement, think pointers. If you need all possibilities, think recursion or backtracking. If you need best/count/possible over repeated subproblems, think dynamic programming.

**What to say out loud:** "I am choosing this approach because it matches the constraint: the expensive operation is repeated work, so I want a structure or pattern that removes that repetition."

**Implementation angle in JavaScript:** Prefer clear names, explicit loops when teaching, and built-ins only when you can explain their complexity. JavaScript gives you Array, Map, Set, and flexible objects, but every helper method still has a cost.

**Edge checks:** Confirm behavior for empty input, one item, duplicate values, already-ordered input, reverse-ordered input, and values at the smallest or largest allowed constraints.

### 4. LRU Cache using doubly linked list plus HashMap with O(1) get/put

**Beginner explanation:** This is one of the core ideas for Doubly Linked List and Circular Linked List. Start by saying it in plain language before reaching for code. A beginner should understand what problem this idea solves, what input it expects, and what output it creates.

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

- `DSA JS/src/data-structures/linked-list/doubly-linked-list/notes.md`
- `DSA JS/src/data-structures/linked-list/doubly-linked-list/implementation.js`
- `DSA JS/src/data-structures/linked-list/circular-linked-list/notes.md`
- `DSA JS/src/data-structures/linked-list/circular-linked-list/implementation.js`

### Imported Notes: `DSA JS/src/data-structures/linked-list/doubly-linked-list/notes.md`

# 🔗 Doubly Linked List (DLL) – Complete DSA Notes

📌 _From Basics to Professional & Interview Level_

---

## 📘 Definition

A **Doubly Linked List** is a linear data structure where:

- Each node contains **three parts**:

  1. `prev` → pointer to previous node
  2. `data` → actual value
  3. `next` → pointer to next node

👉 Unlike a Singly Linked List, traversal is possible in **both directions**.

---

## 🧠 Structure of a Node

```
null ← [prev | data | next] → null
```

### JavaScript Node Class

```js
class Node {
  constructor(data) {
    this.data = data
    this.prev = null
    this.next = null
  }
}
```

---

## 📦 Doubly Linked List Class

```js
class DoublyLinkedList {
  constructor() {
    this.head = null
  }
}
```

---

## ➕ Insertion Operations

### 1️⃣ Insert at Head

```js
insertAtHead(data) {
  let newNode = new Node(data);

  if (this.head !== null) {
    newNode.next = this.head;
    this.head.prev = newNode;
  }


  this.head = newNode;
}
```

### 🧠 Dry Run

Before:

```
null ← 10 ↔ 20 → null
```

Insert `5` at head

After:

```
null ← 5 ↔ 10 ↔ 20 → null
```

---

### 2️⃣ Insert at Tail

```js
insertAtTail(data) {
  let newNode = new Node(data);

  if (this.head === null) {
    this.head = newNode;
    return;
  }

  let temp = this.head;
  while (temp.next !== null) {
    temp = temp.next;
  }

  temp.next = newNode;
  newNode.prev = temp;
}
```

---

### 3️⃣ Insert at Position

```js
insertAtPosition(data, pos) {
  if (pos === 0) {
    this.insertAtHead(data);
    return;
  }

  let newNode = new Node(data);
  let temp = this.head;

  for (let i = 0; i < pos - 1 && temp !== null; i++) {
    temp = temp.next;
  }

  if (temp === null) {
    console.log('Invalid Position');
    return;
  }

  newNode.next = temp.next;
  newNode.prev = temp;

  if (temp.next !== null) {
    temp.next.prev = newNode;
  }

  temp.next = newNode;
}
```

---

## ➖ Deletion Operations

### 4️⃣ Delete Head

```js
deleteHead() {
  if (this.head === null) return;

  this.head = this.head.next;
  if (this.head !== null) this.head.prev = null;
}
```

---

### 5️⃣ Delete Tail

```js
deleteTail() {
  if (this.head === null) return;

  if (this.head.next === null) {
    this.head = null;
    return;
  }

  let temp = this.head;
  while (temp.next !== null) {
    temp = temp.next;
  }

  temp.prev.next = null;
}
```

---

### 6️⃣ Delete by Value

```js
deleteByValue(value) {
  let temp = this.head;

  while (temp !== null && temp.data !== value) {
    temp = temp.next;
  }

  if (temp === null) return;

  if (temp.prev !== null) temp.prev.next = temp.next;
  else this.head = temp.next;

  if (temp.next !== null) temp.next.prev = temp.prev;
}
```

---

## 🖨️ Print Operations

### Forward Print

```js
printForward() {
  let temp = this.head;
  let res = '';

  while (temp !== null) {
    res += temp.data + ' ↔ ';
    temp = temp.next;
  }

  console.log(res + 'null');
}
```

### Backward Print

```js
printBackward() {
  let temp = this.head;

  while (temp && temp.next) {
    temp = temp.next;
  }

  let res = '';
  while (temp !== null) {
    res += temp.data + ' ↔ ';
    temp = temp.prev;
  }

  console.log(res + 'null');
}
```

---

## ⏱️ Time & Space Complexity

| Operation   | Time | Space |
| ----------- | ---- | ----- |
| Insert Head | O(1) | O(1)  |
| Insert Tail | O(n) | O(1)  |
| Delete Head | O(1) | O(1)  |
| Delete Tail | O(n) | O(1)  |
| Search      | O(n) | O(1)  |

---

## 📊 Singly vs Doubly Linked List

| Feature   | Singly LL | Doubly LL |
| --------- | --------- | --------- |
| Traversal | One-way   | Two-way   |
| Memory    | Less      | More      |
| Reverse   | Harder    | Easier    |
| Deletion  | Slower    | Faster    |

---

## 🎯 Interview-Level Points

- Why DLL uses more memory? → extra `prev` pointer
- Why deletion is faster? → direct access to previous node
- Used in:

  - Browser back/forward
  - Undo/Redo
  - Music playlist

---

## ❌ Common Mistakes

- Forgetting to update `prev`
- Breaking links during delete
- Not handling head/tail edge cases

---

## ✅ Summary

- DLL allows **bidirectional traversal**
- Easier deletion & reversal
- Slightly higher memory cost

---

✨ _Prepared for DSA, FAANG & Google-level Interviews_

### Imported Implementation: `DSA JS/src/data-structures/linked-list/doubly-linked-list/implementation.js`

```javascript
// ======================
// NODE CLASS
// ======================
class Node {
  constructor(data) {
    this.prev = null
    this.data = data
    this.next = null
  }
}

// ======================
// DOUBLY LINKED LIST
// ======================
class DoublyLinkedList {
  constructor() {
    this.head = null
  }

  // ======================
  // INSERT AT HEAD
  // ======================
  insertAtHead(data) {
    const newNode = new Node(data)

    if (this.head === null) {
      this.head = newNode
      return
    }

    newNode.next = this.head
    this.head.prev = newNode
    this.head = newNode
  }

  // ======================
  // INSERT AT TAIL
  // ======================
  insertAtTail(data) {
    const newNode = new Node(data)

    if (this.head === null) {
      this.head = newNode
      return
    }

    let temp = this.head
    while (temp.next !== null) {
      temp = temp.next
    }

    temp.next = newNode
    newNode.prev = temp
  }

  // ======================
  // INSERT AT POSITION
  // ======================
  insertAtPosition(data, pos) {
    if (pos < 1) {
      console.log('Invalid position')
      return
    }

    if (pos === 1) {
      this.insertAtHead(data)
      return
    }

    const newNode = new Node(data)
    let temp = this.head

    for (let i = 1; i < pos - 1 && temp !== null; i++) {
      temp = temp.next
    }

    if (temp === null || temp.next === null) {
      console.log('Invalid position')
      return
    }

    newNode.next = temp.next
    newNode.prev = temp
    temp.next.prev = newNode
    temp.next = newNode
  }

  // ======================
  // DELETE AT HEAD
  // ======================
  deleteAtHead() {
    if (this.head === null) {
      console.log('List is empty')
      return
    }

    if (this.head.next === null) {
      this.head = null
      return
    }

    this.head = this.head.next
    this.head.prev = null
  }

  // ======================
  // DELETE AT TAIL
  // ======================
  deleteAtTail() {
    if (this.head === null) {
      console.log('List is empty')
      return
    }

    if (this.head.next === null) {
      this.head = null
      return
    }

    let temp = this.head
    while (temp.next !== null) {
      temp = temp.next
    }

    temp.prev.next = null
  }

  // ======================
  // DELETE AT POSITION
  // ======================
  deleteAtPosition(pos) {
    if (pos < 1 || this.head === null) {
      console.log('Invalid position')
      return
    }

    if (pos === 1) {
      this.deleteAtHead()
      return
    }

    let temp = this.head

    for (let i = 1; i < pos && temp !== null; i++) {
      temp = temp.next
    }

    if (temp === null) {
      console.log('Invalid position')
      return
    }

    if (temp.next === null) {
      temp.prev.next = null
      return
    }

    temp.prev.next = temp.next
    temp.next.prev = temp.prev
  }

  // ======================
  // REVERSE LIST
  // ======================
  reverse() {
    let curr = this.head
    let temp = null

    while (curr) {
      temp = curr.prev
      curr.prev = curr.next
      curr.next = temp
      curr = curr.prev
    }

    if (temp !== null) {
      this.head = temp.prev
    }
  }

  // ======================
  // LENGTH
  // ======================
  length() {
    let count = 0
    let temp = this.head

    while (temp) {
      count++
      temp = temp.next
    }

    console.log(`LENGTH: ${count}`)
  }

  // ======================
  // PRINT LIST
  // ======================
  print() {
    let temp = this.head
    let result = ''

    while (temp) {
      result += temp.data + ' <-> '
      temp = temp.next
    }

    console.log(result + 'null')
  }
}

// ======================
// TESTING
// ======================
const list = new DoublyLinkedList()

list.insertAtHead(100)
list.insertAtHead(300)
list.insertAtHead(600)
list.insertAtHead(900)
list.insertAtHead(10000)

list.insertAtTail(300000000)
list.insertAtPosition(555, 3)

list.print()
list.length()

list.deleteAtHead()
list.deleteAtTail()
list.deleteAtPosition(3)

list.print()
list.reverse()
list.print()
list.length()
```

### Imported Notes: `DSA JS/src/data-structures/linked-list/circular-linked-list/notes.md`

# 🔁 Circular Linked List (DSA Notes)

📌 _Prepared for Google / Amazon / FAANG level interviews_

---

## 📘 Definition

A **Circular Linked List (CLL)** is a linked list in which:

- The **last node points back to the first node (head)**
- There is **NO `null`** at the end
- The list forms a **circle**

👉 Traversal can start from **any node**  
👉 Used when **continuous looping** is required

---

## 🧠 Key Characteristics

✔️ No `null` pointer  
✔️ Last node → points to head  
✔️ Traversal is circular  
✔️ Efficient for repeated tasks

---

## 📊 Types of Circular Linked Lists

1️⃣ **Circular Singly Linked List (CSLL)**  
2️⃣ **Circular Doubly Linked List (CDLL)**

> 📌 In this file, we focus on **Circular Singly Linked List**

---

## 🧱 Node Structure

```js
class Node {
  constructor(data) {
    this.data = data
    this.next = null
  }
}
```

📌 Last node must be updated

insertAtHead(data) {
let newNode = new Node(data);

if (this.head === null) {
newNode.next = newNode;
this.head = newNode;
return;
}

let temp = this.head;
while (temp.next !== this.head) {
temp = temp.next;
}

newNode.next = this.head;
temp.next = newNode;
this.head = newNode;
}

🧪 Dry Run

Initial:

10 → 20 → (back to 10)

Insert 5 at head:

5 → 10 → 20 → (back to 5)

2️⃣ Insert at Tail
insertAtTail(data) {
let newNode = new Node(data);

if (this.head === null) {
newNode.next = newNode;
this.head = newNode;
return;
}

let temp = this.head;
while (temp.next !== this.head) {
temp = temp.next;
}

temp.next = newNode;
newNode.next = this.head;
}

3️⃣ Insert at Position
insertAtPosition(data, pos) {
if (pos === 0) {
this.insertAtHead(data);
return;
}

let temp = this.head;
for (let i = 0; i < pos - 1; i++) {
temp = temp.next;
if (temp === this.head) return;
}

let newNode = new Node(data);
newNode.next = temp.next;
temp.next = newNode;
}

❌ Deletion Operations
1️⃣ Delete Head
deleteHead() {
if (!this.head) return;

if (this.head.next === this.head) {
this.head = null;
return;
}

let temp = this.head;
while (temp.next !== this.head) {
temp = temp.next;
}

temp.next = this.head.next;
this.head = this.head.next;
}

2️⃣ Delete Tail
deleteTail() {
if (!this.head) return;

if (this.head.next === this.head) {
this.head = null;
return;
}

let temp = this.head;
while (temp.next.next !== this.head) {
temp = temp.next;
}

temp.next = this.head;
}

3️⃣ Delete by Value
deleteByValue(value) {
if (!this.head) return;

if (this.head.data === value) {
this.deleteHead();
return;
}

let curr = this.head;
while (curr.next !== this.head && curr.next.data !== value) {
curr = curr.next;
}

if (curr.next.data === value) {
curr.next = curr.next.next;
}
}

🔄 Traversal (Printing)

📌 Use do...while because there is no null

print() {
if (!this.head) return;

let temp = this.head;
let result = "";

do {
result += temp.data + " → ";
temp = temp.next;
} while (temp !== this.head);

console.log(result + "(back to head)");
}

🧠 Why do...while?

✔️ Head must print at least once
✔️ Circular list never reaches null

⏱️ Time & Space Complexity
Operation Time Space
Insert O(n) O(1)
Delete O(n) O(1)
Traverse O(n) O(1)
🆚 Singly vs Circular Linked List
Feature Singly LL Circular LL
Last node null points to head
Loop ❌ ✔️
Traversal linear circular
Use case normal repeating tasks
💼 Real-World Applications

🔁 Round Robin Scheduling

🎵 Music playlist loop

🎮 Turn-based games

🧠 CPU task management

❓ Interview Questions (IMPORTANT)

1️⃣ Difference between SLL & CLL
2️⃣ Why no null in CLL?
3️⃣ How to avoid infinite loop?
4️⃣ Insert/delete head efficiently
5️⃣ Use cases of circular list

⚠️ Common Mistakes

❌ Infinite loop in traversal
❌ Forgetting to link last node
❌ Using while(temp !== null)

✅ Summary

✔️ Circular Linked List has no end
✔️ Last node connects to head
✔️ Efficient for cyclic operations
✔️ Frequently asked in interviews

### Imported Implementation: `DSA JS/src/data-structures/linked-list/circular-linked-list/implementation.js`

```javascript
// ======================
// NODE CLASS
// ======================
class Node {
  constructor(data) {
    this.data = data
    this.prev = null
    this.next = null
  }
}

// ======================
// CIRCULAR DOUBLY LINKED LIST
// ======================
class CircularDoublyLinkedList {
  constructor() {
    this.head = null
  }

  // ======================
  // INSERT AT HEAD
  // ======================
  insertAtHead(data) {
    const newNode = new Node(data)

    if (this.head === null) {
      newNode.next = newNode
      newNode.prev = newNode
      this.head = newNode
      return
    }

    const tail = this.head.prev

    newNode.next = this.head
    newNode.prev = tail
    tail.next = newNode
    this.head.prev = newNode
    this.head = newNode
  }

  // ======================
  // INSERT AT TAIL
  // ======================
  insertAtTail(data) {
    const newNode = new Node(data)

    if (this.head === null) {
      newNode.next = newNode
      newNode.prev = newNode
      this.head = newNode
      return
    }

    const tail = this.head.prev

    tail.next = newNode
    newNode.prev = tail
    newNode.next = this.head
    this.head.prev = newNode
  }

  // ======================
  // DELETE AT HEAD
  // ======================
  deleteAtHead() {
    if (!this.head) {
      console.log('List is empty')
      return
    }

    if (this.head.next === this.head) {
      this.head = null
      return
    }

    const tail = this.head.prev
    this.head = this.head.next
    this.head.prev = tail
    tail.next = this.head
  }

  // ======================
  // DELETE AT TAIL
  // ======================
  deleteAtTail() {
    if (!this.head) {
      console.log('List is empty')
      return
    }

    if (this.head.next === this.head) {
      this.head = null
      return
    }

    const tail = this.head.prev
    const newTail = tail.prev

    newTail.next = this.head
    this.head.prev = newTail
  }

  // ======================
  // DELETE AT POSITION
  // ======================
  deleteAtPosition(pos) {
    if (!this.head || pos < 1) {
      console.log('Invalid position')
      return
    }

    if (pos === 1) {
      this.deleteAtHead()
      return
    }

    let temp = this.head
    let count = 1

    while (count < pos && temp.next !== this.head) {
      temp = temp.next
      count++
    }

    if (count !== pos) {
      console.log('Invalid position')
      return
    }

    // middle or tail node
    temp.prev.next = temp.next
    temp.next.prev = temp.prev
  }

  // ======================
  // LENGTH
  // ======================
  length() {
    if (!this.head) return 0

    let count = 1
    let temp = this.head.next

    while (temp !== this.head) {
      count++
      temp = temp.next
    }

    console.log(`LENGTH: ${count}`)
  }

  // ======================
  // PRINT LIST
  // ======================
  print() {
    if (!this.head) {
      console.log('List is empty')
      return
    }

    let temp = this.head
    let result = ''

    do {
      result += temp.data + ' <-> '
      temp = temp.next
    } while (temp !== this.head)

    console.log(result + '(head)')
  }

  // ======================
  // REVERSE LIST
  // ======================
  reverse() {
    if (!this.head || this.head.next === this.head) return

    let curr = this.head
    let temp = null

    do {
      temp = curr.prev
      curr.prev = curr.next
      curr.next = temp
      curr = curr.prev
    } while (curr !== this.head)

    this.head = temp.prev
  }
}

// ======================
// TESTING
// ======================
const cdll = new CircularDoublyLinkedList()

// INSERT HEAD
cdll.insertAtHead(100)
cdll.insertAtHead(300)
cdll.insertAtHead(600)
cdll.insertAtHead(900)
cdll.insertAtHead(10000)

// INSERT TAIL
cdll.insertAtTail(500000)

// PRINT
cdll.print() // Circular view
cdll.length()

// DELETE HEAD
cdll.deleteAtHead()
cdll.print()

// DELETE TAIL
cdll.deleteAtTail()
cdll.print()

// DELETE POSITION
cdll.deleteAtPosition(3)
cdll.print()

// REVERSE
cdll.reverse()
cdll.print()
```
<!-- DSA-JS-MERGE:END -->

---

**Previous:** [Singly Linked List - Complete Mastery](../Phase-2-Linear-Data-Structures/01-Linked-List-Singly.md) | **Next:** [Stacks - LIFO Mastery](../Phase-2-Linear-Data-Structures/03-Stacks.md)
