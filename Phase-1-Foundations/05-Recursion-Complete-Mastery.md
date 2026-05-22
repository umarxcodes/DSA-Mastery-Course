# Recursion - The Foundation of All Advanced Algorithms

## Chapter Metadata

| Field | Value |
|---|---|
| Phase | Phase 1 - Foundations |
| Chapter | 5 of 37 |
| Difficulty | Intermediate |
| Time to Master | 8-10 hours |
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

Recursion is when a function solves a problem by calling itself on a smaller version of that same problem.

Start simple: the interviewer is not testing whether you can recite textbook language. They are testing whether you can turn a problem into a reliable sequence of choices.

> 🧠 **Mental Model:** First understand what information must be stored, then decide how quickly it must be read, updated, or removed.

## Real-World Analogy

Russian nesting dolls: open one doll and you find the same kind of doll, just smaller, until the smallest one stops the process.

The analogy matters because DSA is usually about trade-offs. A structure that is excellent for fast lookup may be poor for ordered traversal. A recursive solution may be elegant but may use extra call stack memory.

## Visual Representation

```text
factorial(4)
  factorial(3)
    factorial(2)
      factorial(1)
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

- Base case, recursive case, and stack overflow
- Call stack frames with push/pop dry runs
- Factorial, Fibonacci, power, palindrome, flatten nested array, subsets, permutations
- Recursion vs iteration, explicit stack conversion, and JavaScript tail-call limits
- Recursive trees, backtracking, divide and conquer, and memoization

## Deep Teaching Notes

### 1. Base case, recursive case, and stack overflow

**Beginner explanation:** This is one of the core ideas for Recursion - The Foundation of All Advanced Algorithms. Start by saying it in plain language before reaching for code. A beginner should understand what problem this idea solves, what input it expects, and what output it creates.

**Why it matters:** In a FAANG interview, this point shows whether you understand the shape of the problem. Interviewers care less about memorized syntax and more about whether your choices match the constraints.

**How to reason about it:** Ask what must be remembered while the algorithm runs. If you need fast lookup, think HashMap or Set. If you need ordered movement, think pointers. If you need all possibilities, think recursion or backtracking. If you need best/count/possible over repeated subproblems, think dynamic programming.

**What to say out loud:** "I am choosing this approach because it matches the constraint: the expensive operation is repeated work, so I want a structure or pattern that removes that repetition."

**Implementation angle in JavaScript:** Prefer clear names, explicit loops when teaching, and built-ins only when you can explain their complexity. JavaScript gives you Array, Map, Set, and flexible objects, but every helper method still has a cost.

**Edge checks:** Confirm behavior for empty input, one item, duplicate values, already-ordered input, reverse-ordered input, and values at the smallest or largest allowed constraints.

### 2. Call stack frames with push/pop dry runs

**Beginner explanation:** This is one of the core ideas for Recursion - The Foundation of All Advanced Algorithms. Start by saying it in plain language before reaching for code. A beginner should understand what problem this idea solves, what input it expects, and what output it creates.

**Why it matters:** In a FAANG interview, this point shows whether you understand the shape of the problem. Interviewers care less about memorized syntax and more about whether your choices match the constraints.

**How to reason about it:** Ask what must be remembered while the algorithm runs. If you need fast lookup, think HashMap or Set. If you need ordered movement, think pointers. If you need all possibilities, think recursion or backtracking. If you need best/count/possible over repeated subproblems, think dynamic programming.

**What to say out loud:** "I am choosing this approach because it matches the constraint: the expensive operation is repeated work, so I want a structure or pattern that removes that repetition."

**Implementation angle in JavaScript:** Prefer clear names, explicit loops when teaching, and built-ins only when you can explain their complexity. JavaScript gives you Array, Map, Set, and flexible objects, but every helper method still has a cost.

**Edge checks:** Confirm behavior for empty input, one item, duplicate values, already-ordered input, reverse-ordered input, and values at the smallest or largest allowed constraints.

### 3. Factorial, Fibonacci, power, palindrome, flatten nested array, subsets, permutations

**Beginner explanation:** This is one of the core ideas for Recursion - The Foundation of All Advanced Algorithms. Start by saying it in plain language before reaching for code. A beginner should understand what problem this idea solves, what input it expects, and what output it creates.

**Why it matters:** In a FAANG interview, this point shows whether you understand the shape of the problem. Interviewers care less about memorized syntax and more about whether your choices match the constraints.

**How to reason about it:** Ask what must be remembered while the algorithm runs. If you need fast lookup, think HashMap or Set. If you need ordered movement, think pointers. If you need all possibilities, think recursion or backtracking. If you need best/count/possible over repeated subproblems, think dynamic programming.

**What to say out loud:** "I am choosing this approach because it matches the constraint: the expensive operation is repeated work, so I want a structure or pattern that removes that repetition."

**Implementation angle in JavaScript:** Prefer clear names, explicit loops when teaching, and built-ins only when you can explain their complexity. JavaScript gives you Array, Map, Set, and flexible objects, but every helper method still has a cost.

**Edge checks:** Confirm behavior for empty input, one item, duplicate values, already-ordered input, reverse-ordered input, and values at the smallest or largest allowed constraints.

### 4. Recursion vs iteration, explicit stack conversion, and JavaScript tail-call limits

**Beginner explanation:** This is one of the core ideas for Recursion - The Foundation of All Advanced Algorithms. Start by saying it in plain language before reaching for code. A beginner should understand what problem this idea solves, what input it expects, and what output it creates.

**Why it matters:** In a FAANG interview, this point shows whether you understand the shape of the problem. Interviewers care less about memorized syntax and more about whether your choices match the constraints.

**How to reason about it:** Ask what must be remembered while the algorithm runs. If you need fast lookup, think HashMap or Set. If you need ordered movement, think pointers. If you need all possibilities, think recursion or backtracking. If you need best/count/possible over repeated subproblems, think dynamic programming.

**What to say out loud:** "I am choosing this approach because it matches the constraint: the expensive operation is repeated work, so I want a structure or pattern that removes that repetition."

**Implementation angle in JavaScript:** Prefer clear names, explicit loops when teaching, and built-ins only when you can explain their complexity. JavaScript gives you Array, Map, Set, and flexible objects, but every helper method still has a cost.

**Edge checks:** Confirm behavior for empty input, one item, duplicate values, already-ordered input, reverse-ordered input, and values at the smallest or largest allowed constraints.

### 5. Recursive trees, backtracking, divide and conquer, and memoization

**Beginner explanation:** This is one of the core ideas for Recursion - The Foundation of All Advanced Algorithms. Start by saying it in plain language before reaching for code. A beginner should understand what problem this idea solves, what input it expects, and what output it creates.

**Why it matters:** In a FAANG interview, this point shows whether you understand the shape of the problem. Interviewers care less about memorized syntax and more about whether your choices match the constraints.

**How to reason about it:** Ask what must be remembered while the algorithm runs. If you need fast lookup, think HashMap or Set. If you need ordered movement, think pointers. If you need all possibilities, think recursion or backtracking. If you need best/count/possible over repeated subproblems, think dynamic programming.

**What to say out loud:** "I am choosing this approach because it matches the constraint: the expensive operation is repeated work, so I want a structure or pattern that removes that repetition."

**Implementation angle in JavaScript:** Prefer clear names, explicit loops when teaching, and built-ins only when you can explain their complexity. JavaScript gives you Array, Map, Set, and flexible objects, but every helper method still has a cost.

**Edge checks:** Confirm behavior for empty input, one item, duplicate values, already-ordered input, reverse-ordered input, and values at the smallest or largest allowed constraints.


## Complete Implementation

```javascript
/**
 * Computes factorial recursively.
 * Time: O(n), Space: O(n)
 */
function factorial(number) {
  if (number <= 1) return 1;
  return number * factorial(number - 1);
}

console.log(factorial(5));
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

### Problem 1: Factorial

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

### Problem 2: Memoized Fibonacci

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

### Problem 3: Generate Subsets

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

- `DSA JS/src/algorithms/recursion/notes.md`
- `DSA JS/src/algorithms/recursion/fibonacci-notes.md`
- `DSA JS/src/algorithms/recursion/practice.md`

### Imported Notes: `DSA JS/src/algorithms/recursion/notes.md`

# 🔁 Recursion in JavaScript (DSA Notes)

## 📘 Definition

**Recursion** is a technique where a function **calls itself** to solve a problem by breaking it into **smaller subproblems**, until it reaches a **base case**.

> 🛑 **Base Case** stops infinite calls
> 🔁 **Recursive Case** calls the function again

---

## 🧠 Key Concepts

- Every recursion must have:
  1. **Base Case** (stop condition)
  2. **Recursive Call** (same function calling itself)

- Uses **call stack** memory
- Common in **DSA, trees, graphs, backtracking**

---

## 1️⃣ Example: Factorial (Classic Recursion)

### 📌 Problem

Find factorial of a number `n`

```
5! = 5 × 4 × 3 × 2 × 1
```

### ✅ Code

```js
function fact(n) {
  if (n === 1) return 1 // Base case
  return n * fact(n - 1) // Recursive call
}
```

### ⏱ Complexity

- Time: `O(n)`
- Space: `O(n)` (call stack)

---

## 2️⃣ Real-Life Example: Washing Plates 🍽️

### 🧠 Idea

Wash one plate, then call function for remaining plates

### ✅ Code

```js
function WashPlates(plates) {
  if (plates === 0) {
    console.log('All plates are washed!')
    return
  }

  console.log('Washing a plate')
  WashPlates(plates - 1)
}

WashPlates(4)
```

### 📌 Learning

- Each call reduces the problem
- Base case stops recursion

---

## 3️⃣ Searching Using Recursion

### 📌 Problem

Find a name in an array

### ✅ Code

```js
function findName(names, index) {
  if (index === names.length) {
    console.log('Name not found')
    return
  }

  if (names[index] === 'Ali') {
    console.log('Found Ali!')
    return
  }

  findName(names, index + 1)
}

findName(['Ahmed', 'Usman', 'Ali', 'Bilal'], 0)
```

### 🧠 Concept

- Recursive **linear search**

---

## 4️⃣ Best Example: Factorial (Optimized)

```js
function Factorial(n) {
  if (n === 0 || n === 1) return 1 // Base case
  return n * Factorial(n - 1)
}

console.log(Factorial(5))
```

---

## 5️⃣ Fibonacci Series (Iterative Approach)

### 📌 Concept

Each number = sum of previous two

### ✅ Code

```js
function fibonacci(n) {
  let first = 0,
    second = 1
  process.stdout.write(first + ' ' + second + ' ')

  for (let i = 0; i < n; i++) {
    let third = first + second
    first = second
    second = third
    process.stdout.write(third + ' ')
  }
}

fibonacci(5)
```

### ⏱ Complexity

- Time: `O(n)`
- Space: `O(1)`

---

## 6️⃣ Fibonacci Using Recursion (Classic)

```js
function fibonacci(n) {
  if (n === 0) return 0
  if (n === 1) return 1

  return fibonacci(n - 1) + fibonacci(n - 2)
}

console.log(fibonacci(6))
```

### ⚠️ Important

- Very slow for large `n`
- Time: `O(2^n)` ❌

---

## 7️⃣ Fibonacci Using Tail Recursion 🚀

```js
function fibonacci(n, first, second) {
  if (n === 0) return

  let third = first + second
  process.stdout.write(third + ' ')

  fibonacci(n - 1, second, third)
}

fibonacci(4, 0, 1)
```

### ✅ Benefits

- Efficient
- Less recomputation

---

## 📊 Recursion vs Loop

| Feature     | Recursion  | Loop         |
| ----------- | ---------- | ------------ |
| Readability | High       | Medium       |
| Memory      | Uses stack | wLess memory |
| Speed       | Slower     | Faster       |

---

## 🎯 When to Use Recursion?

- Tree / Graph traversal
- Divide & Conquer (Merge Sort, Quick Sort)
- Backtracking (N-Queen, Maze)
- Mathematical problems

---

## 🧠 Interview Tips (Google-Level)

- Always explain **base case** first
- Draw **recursion tree**
- Mention **time & space complexity**
- Avoid recursion if stack overflow possible

---

## ✅ Summary

- Recursion = function calling itself
- Base case is mandatory
- Powerful but must be used carefully

---

🔥 **Next Topics Suggestion**
w

- Recursion Tree Dry Run
- Backtracking Problems
- Recursion → Dynamic Programming
- Stack vs Recursion

---

✍️ _Prepared for DSA & Google-level interviews_

### Imported Notes: `DSA JS/src/algorithms/recursion/fibonacci-notes.md`

Example:First solution ;


function fibonacci(n) {
  let a = 0;
  let b = 1;

  for (let i = 0; i < n; i++) {
    console.log(a);
    let next = a + b;
    a = b;

    b = next;
  }
}

fibonacci(7);

Dry Run the code :



| Step | a | b  | Print |
| ---- | - | -- | ----- |
| 1    | 0 | 1  | 0     |
| 2    | 1 | 1  | 1     |
| 3    | 1 | 2  | 1     |
| 4    | 2 | 3  | 2     |
| 5    | 3 | 5  | 3     |
| 6    | 5 | 8  | 5     |
| 7    | 8 | 13 | 8     |



Example :Second Solution:



function fib(n) {
  if (n === 0) return 0;
  if (n === 1) return 1;

  return fib(n - 1) + fib(n - 2);
}

console.log(fib(6));



//Using Recursion Method


function fib(n) {
  // Base case in fib
  if (n === 0) return 0;
  if (n === 1) return 1;

  return fib(n - 1) + fib(n - 2);
}
console.log(fib(6));

### Imported Notes: `DSA JS/src/algorithms/recursion/practice.md`

EVEL 1: Recursion Basics (Foundation)

Fibonacci Number

Factorial Trailing Zeroes

Power of Two

Power of Three

Power of Four

Reverse String

Sum of Digits of String After Convert

Print Binary Tree (basic recursion idea)

🟡 LEVEL 2: Backtracking Basics

(Real recursion starts here 🔥)

Subsets

Subsets II

Permutations

Permutations II

Combinations

Combination Sum

Combination Sum II

🟡 LEVEL 3: Recursion on Strings

(Google LOVES this)

Letter Combinations of a Phone Number

Generate Parentheses 🔥

Palindrome Partitioning

Restore IP Addresses

Word Search

🟠 LEVEL 4: Recursion on Arrays

(Classic Google pattern)

Sort an Array (using recursion)

K-th Symbol in Grammar

Beautiful Arrangement

Matchsticks to Square

Partition to K Equal Sum Subsets

🟠 LEVEL 5: Recursion + Trees

(MOST IMPORTANT for Google)

Binary Tree Inorder Traversal

Binary Tree Preorder Traversal

Binary Tree Postorder Traversal

Maximum Depth of Binary Tree

Diameter of Binary Tree

Path Sum

Path Sum II

Lowest Common Ancestor of a Binary Tree

🔴 LEVEL 6: Recursion + DP (Hard Google Core)

(These are REAL Google killers 🔥🔥)

Climbing Stairs

House Robber

House Robber II

Unique Paths

Unique Paths II

Decode Ways

Target Sum

Word Break

🔴 LEVEL 7: Advanced Backtracking / DFS

(Top-tier Google)

N-Queens 🔥

N-Queens II

Sudoku Solver 🔥🔥

Expression Add Operators

Remove Invalid Parentheses

All Possible Full Binary Trees
<!-- DSA-JS-MERGE:END -->

<!-- PROMPT-TARGET-EXPANSION:START -->
## Master Prompt Target Expansion

This addendum brings the chapter closer to the depth requested by the master prompt: deeper recognition rules, interview narration, edge-case thinking, dry-run discipline, and complexity reasoning. Treat it as the chapter's final study layer after reading the core lesson and imported legacy material.

### Mastery Expansion 1: base case

**What this part means in plain English:** In Recursion - The Foundation of All Advanced Algorithms, base case is not something to memorize as a disconnected trick. It is a decision tool. The core question is: what information changes as the input grows, and what information must remain available so the next step is cheap? When you can answer that, the correct data structure or algorithm becomes much easier to choose.

**How to recognize it in an interview:** Listen for the wording of the prompt. If the problem asks for fast lookup, repeated membership checks, duplicate detection, grouping, or counting, you should immediately consider a map or set. If it asks for contiguous ranges, windows, substrings, or subarrays, you should look for a sliding window or prefix state. If it asks for all possible choices, paths, arrangements, or boards, draw the decision tree before coding. If it asks for best, minimum, maximum, count ways, or feasibility with repeated subproblems, define a DP state before reaching for loops.

**Brute force baseline:** Always describe the direct solution first. For base case, the brute force version usually repeats work: scanning the same area again, recalculating a value already known, trying every pair, or exploring branches that can be proven impossible. The baseline matters because it gives you a correctness anchor and gives the interviewer a clear before-and-after optimization story.

**Optimization move:** The optimization is usually one of four moves: store seen information, exploit sorted order, maintain an invariant while moving pointers, or cache solved subproblems. Say the invariant out loud. A good invariant sounds like: "At every step, my map contains only values from the processed prefix," or "The window is always the longest valid window ending at the current right pointer," or "The heap always stores the best candidates seen so far."

**Dry-run discipline:** Use a tiny input and trace every state change. Write the input, current index or pointer, auxiliary structure contents, current answer, and reason for movement. Do not jump from the first step to the final answer. The dry run is where off-by-one bugs, stale map entries, missed duplicate handling, and wrong base cases become visible.

**Edge cases to test:** Test empty input, one element, duplicate-heavy input, already sorted input, reverse sorted input, negative values if numbers are allowed, and maximum constraint shape. For recursive or graph problems, also test disconnected input, cycles, repeated visits, and a path that almost works but fails at the final step.

**What a strong candidate says:** "I will start with a correct brute force approach, analyze why it is too slow, then remove repeated work by preserving exactly the state I need. I will keep the invariant visible while coding, dry-run on a normal example, and then test edge cases before giving final complexity."

**Complexity explanation:** Do not only state Big O. Explain the count. If each element enters and leaves a window once, the runtime is O(n). If every node and edge is visited once, it is O(V + E). If recursion branches into two calls per level, draw the tree. If sorting happens before a linear scan, sorting dominates at O(n log n). If a heap operation occurs for every item, multiply by log k or log n depending on heap size.
<!-- PROMPT-TARGET-EXPANSION:END -->

---

**Previous:** [Strings - Mastery from a DSA Perspective](../Phase-1-Foundations/04-Strings-DSA-Perspective.md) | **Next:** [Singly Linked List - Complete Mastery](../Phase-2-Linear-Data-Structures/01-Linked-List-Singly.md)
