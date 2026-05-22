# Stacks - LIFO Mastery

## Chapter Metadata

| Field | Value |
|---|---|
| Phase | Phase 2 - Linear Data Structures |
| Chapter | 8 of 37 |
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

- LIFO behavior, browser history, undo/redo, and call stack
- Stack implementation with array and linked list
- Balanced parentheses, Reverse Polish notation, queue using stacks
- Min stack, monotonic stack, next greater element, daily temperatures, histogram

## Deep Teaching Notes

### 1. LIFO behavior, browser history, undo/redo, and call stack

**Beginner explanation:** This is one of the core ideas for Stacks - LIFO Mastery. Start by saying it in plain language before reaching for code. A beginner should understand what problem this idea solves, what input it expects, and what output it creates.

**Why it matters:** In a FAANG interview, this point shows whether you understand the shape of the problem. Interviewers care less about memorized syntax and more about whether your choices match the constraints.

**How to reason about it:** Ask what must be remembered while the algorithm runs. If you need fast lookup, think HashMap or Set. If you need ordered movement, think pointers. If you need all possibilities, think recursion or backtracking. If you need best/count/possible over repeated subproblems, think dynamic programming.

**What to say out loud:** "I am choosing this approach because it matches the constraint: the expensive operation is repeated work, so I want a structure or pattern that removes that repetition."

**Implementation angle in JavaScript:** Prefer clear names, explicit loops when teaching, and built-ins only when you can explain their complexity. JavaScript gives you Array, Map, Set, and flexible objects, but every helper method still has a cost.

**Edge checks:** Confirm behavior for empty input, one item, duplicate values, already-ordered input, reverse-ordered input, and values at the smallest or largest allowed constraints.

### 2. Stack implementation with array and linked list

**Beginner explanation:** This is one of the core ideas for Stacks - LIFO Mastery. Start by saying it in plain language before reaching for code. A beginner should understand what problem this idea solves, what input it expects, and what output it creates.

**Why it matters:** In a FAANG interview, this point shows whether you understand the shape of the problem. Interviewers care less about memorized syntax and more about whether your choices match the constraints.

**How to reason about it:** Ask what must be remembered while the algorithm runs. If you need fast lookup, think HashMap or Set. If you need ordered movement, think pointers. If you need all possibilities, think recursion or backtracking. If you need best/count/possible over repeated subproblems, think dynamic programming.

**What to say out loud:** "I am choosing this approach because it matches the constraint: the expensive operation is repeated work, so I want a structure or pattern that removes that repetition."

**Implementation angle in JavaScript:** Prefer clear names, explicit loops when teaching, and built-ins only when you can explain their complexity. JavaScript gives you Array, Map, Set, and flexible objects, but every helper method still has a cost.

**Edge checks:** Confirm behavior for empty input, one item, duplicate values, already-ordered input, reverse-ordered input, and values at the smallest or largest allowed constraints.

### 3. Balanced parentheses, Reverse Polish notation, queue using stacks

**Beginner explanation:** This is one of the core ideas for Stacks - LIFO Mastery. Start by saying it in plain language before reaching for code. A beginner should understand what problem this idea solves, what input it expects, and what output it creates.

**Why it matters:** In a FAANG interview, this point shows whether you understand the shape of the problem. Interviewers care less about memorized syntax and more about whether your choices match the constraints.

**How to reason about it:** Ask what must be remembered while the algorithm runs. If you need fast lookup, think HashMap or Set. If you need ordered movement, think pointers. If you need all possibilities, think recursion or backtracking. If you need best/count/possible over repeated subproblems, think dynamic programming.

**What to say out loud:** "I am choosing this approach because it matches the constraint: the expensive operation is repeated work, so I want a structure or pattern that removes that repetition."

**Implementation angle in JavaScript:** Prefer clear names, explicit loops when teaching, and built-ins only when you can explain their complexity. JavaScript gives you Array, Map, Set, and flexible objects, but every helper method still has a cost.

**Edge checks:** Confirm behavior for empty input, one item, duplicate values, already-ordered input, reverse-ordered input, and values at the smallest or largest allowed constraints.

### 4. Min stack, monotonic stack, next greater element, daily temperatures, histogram

**Beginner explanation:** This is one of the core ideas for Stacks - LIFO Mastery. Start by saying it in plain language before reaching for code. A beginner should understand what problem this idea solves, what input it expects, and what output it creates.

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

- `DSA JS/src/data-structures/stack/notes.md`
- `DSA JS/src/data-structures/stack/implementation.js`
- `DSA JS/src/data-structures/stack/practice.md`

### Imported Notes: `DSA JS/src/data-structures/stack/notes.md`

# Stack Data Structure

## What It Is

A stack is a linear data structure that follows the `LIFO` rule: `Last In, First Out`.

Examples:

- Browser back navigation
- Undo and redo history
- Function call stack
- Expression parsing
- Monotonic stack problems

Representation:

```text
bottom [10, 20, 30] top
```

---

## Core Operations

| Operation | Purpose | Expected Complexity |
| --- | --- | --- |
| `push(x)` | Insert `x` at the top | `O(1)` |
| `pop()` | Remove and return top element | `O(1)` |
| `peek()` | Return top element without removing it | `O(1)` |
| `isEmpty()` | Check whether stack has no elements | `O(1)` |
| `size()` | Number of elements in stack | `O(1)` |

Interview note:

- `push`, `pop`, and `peek` are only `O(1)` if we operate at one end.
- Using `Array.prototype.shift()` or `unshift()` would make operations `O(n)`, so they should not be used for stack implementations.

---

## Interview Invariants

For a correct stack implementation:

- The newest item must always be the next item removed.
- `peek()` must not modify the stack.
- Underflow should be handled predictably.
- `size()` should always match the number of stored elements.

Good interview explanation:

1. Define the invariant: top element is the most recently inserted unremoved item.
2. Show how each operation preserves that invariant.
3. State time and space complexity.
4. Call out underflow handling.

---

## Implementation 1: Stack Using Array

### When To Use It

Use an array-backed stack when:

- You want a compact implementation
- Random access to the internal backing store is acceptable
- Dynamic resizing from the language runtime is fine

### JavaScript Implementation

```js
class ArrayStack {
  constructor() {
    this.items = []
  }

  push(value) {
    this.items.push(value)
    return this.items.length
  }

  pop() {
    if (this.items.length === 0) {
      return null
    }

    return this.items.pop()
  }

  peek() {
    if (this.items.length === 0) {
      return null
    }

    return this.items[this.items.length - 1]
  }

  isEmpty() {
    return this.items.length === 0
  }

  size() {
    return this.items.length
  }
}
```

### Complexity

- `push`: `O(1)` amortized
- `pop`: `O(1)`
- `peek`: `O(1)`
- `isEmpty`: `O(1)`
- `size`: `O(1)`
- Space: `O(n)`

### Edge Cases

- `pop()` on empty stack
- `peek()` on empty stack
- Repeated push/pop alternating sequences
- Duplicates and falsy values like `0`, `false`, `''`, and `null`

---

## Implementation 2: Stack Using Linked List

### When To Use It

Use a linked-list-backed stack when:

- You want explicit node-level structure
- You want `O(1)` push/pop without relying on array resizing
- You are practicing pointer manipulation for interviews

### JavaScript Implementation

```js
class StackNode {
  constructor(value) {
    this.value = value
    this.next = null
  }
}

class LinkedListStack {
  constructor() {
    this.top = null
    this.length = 0
  }

  push(value) {
    const node = new StackNode(value)
    node.next = this.top
    this.top = node
    this.length += 1
    return this.length
  }

  pop() {
    if (this.top === null) {
      return null
    }

    const removedValue = this.top.value
    this.top = this.top.next
    this.length -= 1
    return removedValue
  }

  peek() {
    return this.top ? this.top.value : null
  }

  isEmpty() {
    return this.length === 0
  }

  size() {
    return this.length
  }
}
```

### Complexity

- `push`: `O(1)`
- `pop`: `O(1)`
- `peek`: `O(1)`
- `isEmpty`: `O(1)`
- `size`: `O(1)`
- Space: `O(n)`

### Trade-Offs vs Array

| Factor | Array Stack | Linked List Stack |
| --- | --- | --- |
| Simplicity | Better | Slightly worse |
| Constant factors | Better in JS | Worse |
| Dynamic growth | Yes | Yes |
| Pointer practice | No | Yes |
| Interview teaching value | Good | Very good |

Important correction:

- Saying an array stack has "fixed memory" is inaccurate in JavaScript because arrays resize dynamically.
- Saying linked lists have "no overflow" is also inaccurate in practical systems. They can still fail due to memory limits.

---

## Pattern: Valid Parentheses

### Problem

Given a string containing only brackets, determine whether every opening bracket is closed in the correct order.

### Why Stack Fits

The most recently opened bracket must be matched first, which is exactly `LIFO`.

### Optimal Approach

1. Push opening brackets.
2. On a closing bracket, pop and verify the type matches.
3. At the end, the stack must be empty.

### Code

```js
function isValidParentheses(sequence) {
  const stack = []
  const closingToOpening = {
    ')': '(',
    ']': '[',
    '}': '{',
  }

  for (const char of sequence) {
    if (char === '(' || char === '[' || char === '{') {
      stack.push(char)
      continue
    }

    if (closingToOpening[char]) {
      if (stack.pop() !== closingToOpening[char]) {
        return false
      }
    }
  }

  return stack.length === 0
}
```

### Complexity

- Time: `O(n)`
- Space: `O(n)` in the worst case

### Interview Discussion Points

- Why this is not a counting problem
- Why order matters, not just frequency
- Why stack is better than trying to match from the start greedily

---

## Pattern: Reverse a String

### Problem

Reverse a string using stack behavior.

### Code

```js
function reverseStringWithStack(value) {
  const stack = []

  for (const char of value) {
    stack.push(char)
  }

  let reversed = ''
  while (stack.length > 0) {
    reversed += stack.pop()
  }

  return reversed
}
```

### Complexity

- Time: `O(n)`
- Space: `O(n)`

Interview note:

- In production JavaScript, `split('').reverse().join('')` is often shorter, but the stack version is useful for teaching the pattern.

---

## Common Stack Patterns

### 1. Parenthesis and Expression Validation

- Valid Parentheses
- Remove Outermost Parentheses
- Minimum Add to Make Parentheses Valid

### 2. Monotonic Stack

Use a stack that is kept increasing or decreasing.

- Next Greater Element
- Daily Temperatures
- Largest Rectangle in Histogram
- Trapping Rain Water

### 3. Simulation Problems

- Baseball Game
- Backspace String Compare
- Decode String

### 4. Stack Transformation

- Implement Queue using Stacks
- Implement Stack using Queues
- Min Stack

---

## FAANG-Level Follow-Up Questions

For stack implementations:

- How would you support `getMin()` in `O(1)`?
- How would you implement a stack using two queues?
- How would you make it generic enough for interview reuse?
- What changes if the stack must be thread-safe?

For stack pattern problems:

- Can you reduce extra space?
- Can you derive the monotonic invariant clearly?
- What happens with duplicate values?
- How do you justify correctness, not just complexity?

---

## Whiteboard Strategy

When presenting a stack problem in an interview:

1. State why `LIFO` matches the problem.
2. Define what is stored in the stack.
3. Walk through one example manually.
4. Identify underflow or empty-stack cases.
5. Give final complexity and trade-offs.

---

## Weak Spots To Fix In The Current Repo

- Canonical stack implementation now lives in [implementation.js](/home/engineer/projects/DSA/DSA%20JS/src/data-structures/stack/implementation.js)
- Automated coverage currently starts with [stack.test.js](/home/engineer/projects/DSA/DSA%20JS/tests/stack.test.js)
- Practice list has been normalized to `practice.md`
- Notes should be standardized by `concept -> invariant -> implementation -> pattern -> practice`

---

## Recommended Practice Set

Easy:

- Valid Parentheses
- Implement Stack using Queues
- Baseball Game

Medium:

- Min Stack
- Daily Temperatures
- Next Greater Element II
- Decode String

Hard:

- Largest Rectangle in Histogram
- Maximal Rectangle
- Basic Calculator II

---

## Final Takeaway

If you can:

- implement a stack from scratch,
- explain why `LIFO` is correct,
- solve bracket validation confidently,
- and recognize monotonic stack patterns,

then your stack fundamentals are interview ready.

### Imported Implementation: `DSA JS/src/data-structures/stack/implementation.js`

```javascript
class ArrayStack {
  constructor() {
    this.items = []
  }

  push(value) {
    this.items.push(value)
    return this.size()
  }

  pop() {
    if (this.isEmpty()) {
      return null
    }

    return this.items.pop()
  }

  peek() {
    if (this.isEmpty()) {
      return null
    }

    return this.items[this.items.length - 1]
  }

  isEmpty() {
    return this.items.length === 0
  }

  size() {
    return this.items.length
  }

  clear() {
    this.items.length = 0
  }

  toArray() {
    return [...this.items]
  }
}

class StackNode {
  constructor(value) {
    this.value = value
    this.next = null
  }
}

class LinkedListStack {
  constructor() {
    this.top = null
    this.length = 0
  }

  push(value) {
    const node = new StackNode(value)
    node.next = this.top
    this.top = node
    this.length += 1
    return this.length
  }

  pop() {
    if (this.isEmpty()) {
      return null
    }

    const removedValue = this.top.value
    this.top = this.top.next
    this.length -= 1
    return removedValue
  }

  peek() {
    return this.top ? this.top.value : null
  }

  isEmpty() {
    return this.length === 0
  }

  size() {
    return this.length
  }

  clear() {
    this.top = null
    this.length = 0
  }

  toArray() {
    const result = []
    let current = this.top

    while (current) {
      result.push(current.value)
      current = current.next
    }

    return result
  }
}

function isValidParentheses(sequence) {
  const stack = new ArrayStack()
  const closingToOpening = {
    ')': '(',
    ']': '[',
    '}': '{',
  }

  for (const char of sequence) {
    if (char === '(' || char === '[' || char === '{') {
      stack.push(char)
      continue
    }

    if (closingToOpening[char]) {
      if (stack.pop() !== closingToOpening[char]) {
        return false
      }
    }
  }

  return stack.isEmpty()
}

function reverseStringWithStack(value) {
  const stack = new ArrayStack()

  for (const char of value) {
    stack.push(char)
  }

  let reversed = ''
  while (!stack.isEmpty()) {
    reversed += stack.pop()
  }

  return reversed
}

module.exports = {
  ArrayStack,
  LinkedListStack,
  StackNode,
  isValidParentheses,
  reverseStringWithStack,
}
```

### Imported Notes: `DSA JS/src/data-structures/stack/practice.md`

# Stack Practice List

## Easy

- Valid Parentheses
- Implement Stack using Queues
- Implement Queue using Stacks
- Baseball Game
- Backspace String Compare

## Medium

- Min Stack
- Next Greater Element I
- Next Greater Element II
- Daily Temperatures
- Online Stock Span
- Remove K Digits
- Decode String

## Hard

- Largest Rectangle in Histogram
- Maximal Rectangle
- Basic Calculator
- Basic Calculator II
- Trapping Rain Water

## Pattern Mapping

- Validation: Valid Parentheses
- Simulation: Baseball Game, Decode String
- Design: Min Stack, Stack Using Queues
- Monotonic Stack: Daily Temperatures, Largest Rectangle in Histogram, Trapping Rain Water

## Interview Order

1. Valid Parentheses
2. Min Stack
3. Daily Temperatures
4. Decode String
5. Largest Rectangle in Histogram
<!-- DSA-JS-MERGE:END -->

---

**Previous:** [Doubly Linked List and Circular Linked List](../Phase-2-Linear-Data-Structures/02-Linked-List-Doubly-Circular.md) | **Next:** [Queues and Deques](../Phase-2-Linear-Data-Structures/04-Queues.md)
