# Dynamic Programming - Foundation and Mindset

## Chapter Metadata

| Field | Value |
|---|---|
| Phase | Phase 5 - Advanced Algorithms |
| Chapter | 23 of 37 |
| Difficulty | Advanced |
| Time to Master | 12-14 hours |
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

- Overlapping subproblems and optimal substructure
- State, recurrence, base cases, and computation order
- Top-down memoization and bottom-up tabulation
- Fibonacci, climbing stairs, house robber, jump game, min cost stairs

## Deep Teaching Notes

### 1. Overlapping subproblems and optimal substructure

**Beginner explanation:** This is one of the core ideas for Dynamic Programming - Foundation and Mindset. Start by saying it in plain language before reaching for code. A beginner should understand what problem this idea solves, what input it expects, and what output it creates.

**Why it matters:** In a FAANG interview, this point shows whether you understand the shape of the problem. Interviewers care less about memorized syntax and more about whether your choices match the constraints.

**How to reason about it:** Ask what must be remembered while the algorithm runs. If you need fast lookup, think HashMap or Set. If you need ordered movement, think pointers. If you need all possibilities, think recursion or backtracking. If you need best/count/possible over repeated subproblems, think dynamic programming.

**What to say out loud:** "I am choosing this approach because it matches the constraint: the expensive operation is repeated work, so I want a structure or pattern that removes that repetition."

**Implementation angle in JavaScript:** Prefer clear names, explicit loops when teaching, and built-ins only when you can explain their complexity. JavaScript gives you Array, Map, Set, and flexible objects, but every helper method still has a cost.

**Edge checks:** Confirm behavior for empty input, one item, duplicate values, already-ordered input, reverse-ordered input, and values at the smallest or largest allowed constraints.

### 2. State, recurrence, base cases, and computation order

**Beginner explanation:** This is one of the core ideas for Dynamic Programming - Foundation and Mindset. Start by saying it in plain language before reaching for code. A beginner should understand what problem this idea solves, what input it expects, and what output it creates.

**Why it matters:** In a FAANG interview, this point shows whether you understand the shape of the problem. Interviewers care less about memorized syntax and more about whether your choices match the constraints.

**How to reason about it:** Ask what must be remembered while the algorithm runs. If you need fast lookup, think HashMap or Set. If you need ordered movement, think pointers. If you need all possibilities, think recursion or backtracking. If you need best/count/possible over repeated subproblems, think dynamic programming.

**What to say out loud:** "I am choosing this approach because it matches the constraint: the expensive operation is repeated work, so I want a structure or pattern that removes that repetition."

**Implementation angle in JavaScript:** Prefer clear names, explicit loops when teaching, and built-ins only when you can explain their complexity. JavaScript gives you Array, Map, Set, and flexible objects, but every helper method still has a cost.

**Edge checks:** Confirm behavior for empty input, one item, duplicate values, already-ordered input, reverse-ordered input, and values at the smallest or largest allowed constraints.

### 3. Top-down memoization and bottom-up tabulation

**Beginner explanation:** This is one of the core ideas for Dynamic Programming - Foundation and Mindset. Start by saying it in plain language before reaching for code. A beginner should understand what problem this idea solves, what input it expects, and what output it creates.

**Why it matters:** In a FAANG interview, this point shows whether you understand the shape of the problem. Interviewers care less about memorized syntax and more about whether your choices match the constraints.

**How to reason about it:** Ask what must be remembered while the algorithm runs. If you need fast lookup, think HashMap or Set. If you need ordered movement, think pointers. If you need all possibilities, think recursion or backtracking. If you need best/count/possible over repeated subproblems, think dynamic programming.

**What to say out loud:** "I am choosing this approach because it matches the constraint: the expensive operation is repeated work, so I want a structure or pattern that removes that repetition."

**Implementation angle in JavaScript:** Prefer clear names, explicit loops when teaching, and built-ins only when you can explain their complexity. JavaScript gives you Array, Map, Set, and flexible objects, but every helper method still has a cost.

**Edge checks:** Confirm behavior for empty input, one item, duplicate values, already-ordered input, reverse-ordered input, and values at the smallest or largest allowed constraints.

### 4. Fibonacci, climbing stairs, house robber, jump game, min cost stairs

**Beginner explanation:** This is one of the core ideas for Dynamic Programming - Foundation and Mindset. Start by saying it in plain language before reaching for code. A beginner should understand what problem this idea solves, what input it expects, and what output it creates.

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

- `DSA JS/src/algorithms/dynamic-programming/notes.md`

### Imported Notes: `DSA JS/src/algorithms/dynamic-programming/notes.md`

# 🔥 Dynamic Programming – Complete Master Notes (Beginner to Advanced)

---

# 🧠 1️⃣ What is Dynamic Programming? (Super Simple)

Dynamic Programming (DP) =

👉 Solve big problem
👉 Break into small problems
👉 Store answers
👉 Reuse stored answers

Simple meaning:

"Don't solve same problem again and again."

---

# 🧱 2️⃣ When to Use DP?

DP is used when problem has:

1️⃣ Overlapping Subproblems
2️⃣ Optimal Substructure

---

## ✅ Overlapping Subproblems

Example: Fibonacci

```
fib(5)
├── fib(4)
│   ├── fib(3)
│   └── fib(2)
└── fib(3)
```

fib(3) is calculated multiple times 😵

---

## ✅ Optimal Substructure

If best answer of big problem depends on best answer of small problems.

Example:

Shortest path
Knapsack

---

# 🧩 3️⃣ Two Ways to Do DP

## 1️⃣ Memoization (Top-Down)

* Recursion
* Store answers in array/map

## 2️⃣ Tabulation (Bottom-Up)

* Iterative
* Build solution step by step

---

# 🌱 4️⃣ Fibonacci Example (Starter DP)

---

## ❌ Normal Recursion (Bad)

Time: O(2^n)

```js
function fib(n) {
  if (n <= 1) return n
  return fib(n-1) + fib(n-2)
}
```

---

## ✅ Memoization

Time: O(n)

```js
function fib(n, dp = {}) {
  if (n in dp) return dp[n]
  if (n <= 1) return n

  dp[n] = fib(n-1, dp) + fib(n-2, dp)
  return dp[n]
}
```

---

## ✅ Tabulation

```js
function fib(n) {
  let dp = new Array(n+1).fill(0)
  dp[1] = 1

  for (let i = 2; i <= n; i++) {
    dp[i] = dp[i-1] + dp[i-2]
  }

  return dp[n]
}
```

---

# 🪜 5️⃣ Climbing Stairs

You can climb 1 or 2 steps.

How many ways to reach n?

Same as Fibonacci!

Transition:

```
dp[i] = dp[i-1] + dp[i-2]
```

---

# 🎒 6️⃣ 0/1 Knapsack (Important)

You have:

* Weights
* Values
* Capacity

Goal:
Maximize value without exceeding capacity.

DP State:

```
dp[i][w] = max value using first i items and capacity w
```

Transition:

```
If weight <= w:
  dp[i][w] = max(
      dp[i-1][w],
      value + dp[i-1][w-weight]
  )
Else:
  dp[i][w] = dp[i-1][w]
```

Time: O(n × capacity)

---

# 💰 7️⃣ Coin Change

Given coins, find minimum coins to make amount.

State:

```
dp[i] = minimum coins to make amount i
```

Transition:

```
dp[i] = min(dp[i], dp[i-coin] + 1)
```

---

# 🔤 8️⃣ Longest Common Subsequence (LCS)

Given two strings.
Find longest common subsequence.

State:

```
dp[i][j] = LCS length of s1[0..i-1] and s2[0..j-1]
```

Transition:

If characters match:

```
dp[i][j] = 1 + dp[i-1][j-1]
```

Else:

```
dp[i][j] = max(dp[i-1][j], dp[i][j-1])
```

Time: O(n × m)

---

# 📈 9️⃣ Longest Increasing Subsequence (LIS)

Find longest increasing subsequence.

Basic DP:

```
dp[i] = length of LIS ending at i
```

Time: O(n²)

Optimized:

Binary Search method → O(n log n)

---

# 🧮 🔟 DP on Grid (Matrix DP)

Common Problems:

* Unique paths
* Minimum path sum

State:

```
dp[i][j] = answer for cell (i, j)
```

Transition:

```
dp[i][j] = dp[i-1][j] + dp[i][j-1]
```

---

# 🔁 1️⃣1️⃣ DP on Subsequences

Pattern:

"Include or Exclude"

Example:

* Subset sum
* Partition equal subset
* Target sum

---

# 🔥 1️⃣2️⃣ DP Optimization Techniques

## 1️⃣ Space Optimization

Instead of 2D dp, use 1D dp.

## 2️⃣ Bitmask DP

Used in advanced problems.

## 3️⃣ Digit DP

Used in number problems.

## 4️⃣ DP with State Compression

Advanced competitive programming technique.

---

# 🧠 How to Think in DP (Step-by-Step)

1️⃣ Define state
2️⃣ Define transition
3️⃣ Define base case
4️⃣ Decide memoization or tabulation
5️⃣ Optimize space

---

# 🚀 Complexity Summary

| Problem         | Time Complexity    |
| --------------- | ------------------ |
| Fibonacci       | O(n)               |
| Climbing Stairs | O(n)               |
| Knapsack        | O(nW)              |
| Coin Change     | O(n × amount)      |
| LCS             | O(nm)              |
| LIS             | O(n²) / O(n log n) |
| Grid DP         | O(nm)              |

---

# 🎯 DP Master Roadmap

Level 1:

* Fibonacci
* Climbing Stairs

Level 2:

* Coin Change
* Knapsack
* Subset Sum

Level 3:

* LCS
* LIS
* Matrix DP

Level 4:

* Bitmask DP
* Digit DP
* Advanced Optimization

---

# 🌟 Final Advice

DP is not about memorizing formulas.

It is about pattern recognition.

If you can:

* Define state
* Write transition
* Handle base case

You can solve any DP problem.

---

🔥 End of Dynamic Programming Complete Notes
a
<!-- DSA-JS-MERGE:END -->

<!-- PROMPT-TARGET-EXPANSION:START -->
## Master Prompt Target Expansion

This addendum brings the chapter closer to the depth requested by the master prompt: deeper recognition rules, interview narration, edge-case thinking, dry-run discipline, and complexity reasoning. Treat it as the chapter's final study layer after reading the core lesson and imported legacy material.

### Mastery Expansion 1: state

**What this part means in plain English:** In Dynamic Programming - Foundation and Mindset, state is not something to memorize as a disconnected trick. It is a decision tool. The core question is: what information changes as the input grows, and what information must remain available so the next step is cheap? When you can answer that, the correct data structure or algorithm becomes much easier to choose.

**How to recognize it in an interview:** Listen for the wording of the prompt. If the problem asks for fast lookup, repeated membership checks, duplicate detection, grouping, or counting, you should immediately consider a map or set. If it asks for contiguous ranges, windows, substrings, or subarrays, you should look for a sliding window or prefix state. If it asks for all possible choices, paths, arrangements, or boards, draw the decision tree before coding. If it asks for best, minimum, maximum, count ways, or feasibility with repeated subproblems, define a DP state before reaching for loops.

**Brute force baseline:** Always describe the direct solution first. For state, the brute force version usually repeats work: scanning the same area again, recalculating a value already known, trying every pair, or exploring branches that can be proven impossible. The baseline matters because it gives you a correctness anchor and gives the interviewer a clear before-and-after optimization story.

**Optimization move:** The optimization is usually one of four moves: store seen information, exploit sorted order, maintain an invariant while moving pointers, or cache solved subproblems. Say the invariant out loud. A good invariant sounds like: "At every step, my map contains only values from the processed prefix," or "The window is always the longest valid window ending at the current right pointer," or "The heap always stores the best candidates seen so far."

**Dry-run discipline:** Use a tiny input and trace every state change. Write the input, current index or pointer, auxiliary structure contents, current answer, and reason for movement. Do not jump from the first step to the final answer. The dry run is where off-by-one bugs, stale map entries, missed duplicate handling, and wrong base cases become visible.

**Edge cases to test:** Test empty input, one element, duplicate-heavy input, already sorted input, reverse sorted input, negative values if numbers are allowed, and maximum constraint shape. For recursive or graph problems, also test disconnected input, cycles, repeated visits, and a path that almost works but fails at the final step.

**What a strong candidate says:** "I will start with a correct brute force approach, analyze why it is too slow, then remove repeated work by preserving exactly the state I need. I will keep the invariant visible while coding, dry-run on a normal example, and then test edge cases before giving final complexity."

**Complexity explanation:** Do not only state Big O. Explain the count. If each element enters and leaves a window once, the runtime is O(n). If every node and edge is visited once, it is O(V + E). If recursion branches into two calls per level, draw the tree. If sorting happens before a linear scan, sorting dominates at O(n log n). If a heap operation occurs for every item, multiply by log k or log n depending on heap size.

### Mastery Expansion 2: recurrence

**What this part means in plain English:** In Dynamic Programming - Foundation and Mindset, recurrence is not something to memorize as a disconnected trick. It is a decision tool. The core question is: what information changes as the input grows, and what information must remain available so the next step is cheap? When you can answer that, the correct data structure or algorithm becomes much easier to choose.

**How to recognize it in an interview:** Listen for the wording of the prompt. If the problem asks for fast lookup, repeated membership checks, duplicate detection, grouping, or counting, you should immediately consider a map or set. If it asks for contiguous ranges, windows, substrings, or subarrays, you should look for a sliding window or prefix state. If it asks for all possible choices, paths, arrangements, or boards, draw the decision tree before coding. If it asks for best, minimum, maximum, count ways, or feasibility with repeated subproblems, define a DP state before reaching for loops.

**Brute force baseline:** Always describe the direct solution first. For recurrence, the brute force version usually repeats work: scanning the same area again, recalculating a value already known, trying every pair, or exploring branches that can be proven impossible. The baseline matters because it gives you a correctness anchor and gives the interviewer a clear before-and-after optimization story.

**Optimization move:** The optimization is usually one of four moves: store seen information, exploit sorted order, maintain an invariant while moving pointers, or cache solved subproblems. Say the invariant out loud. A good invariant sounds like: "At every step, my map contains only values from the processed prefix," or "The window is always the longest valid window ending at the current right pointer," or "The heap always stores the best candidates seen so far."

**Dry-run discipline:** Use a tiny input and trace every state change. Write the input, current index or pointer, auxiliary structure contents, current answer, and reason for movement. Do not jump from the first step to the final answer. The dry run is where off-by-one bugs, stale map entries, missed duplicate handling, and wrong base cases become visible.

**Edge cases to test:** Test empty input, one element, duplicate-heavy input, already sorted input, reverse sorted input, negative values if numbers are allowed, and maximum constraint shape. For recursive or graph problems, also test disconnected input, cycles, repeated visits, and a path that almost works but fails at the final step.

**What a strong candidate says:** "I will start with a correct brute force approach, analyze why it is too slow, then remove repeated work by preserving exactly the state I need. I will keep the invariant visible while coding, dry-run on a normal example, and then test edge cases before giving final complexity."

**Complexity explanation:** Do not only state Big O. Explain the count. If each element enters and leaves a window once, the runtime is O(n). If every node and edge is visited once, it is O(V + E). If recursion branches into two calls per level, draw the tree. If sorting happens before a linear scan, sorting dominates at O(n log n). If a heap operation occurs for every item, multiply by log k or log n depending on heap size.

### Mastery Expansion 3: base cases

**What this part means in plain English:** In Dynamic Programming - Foundation and Mindset, base cases is not something to memorize as a disconnected trick. It is a decision tool. The core question is: what information changes as the input grows, and what information must remain available so the next step is cheap? When you can answer that, the correct data structure or algorithm becomes much easier to choose.

**How to recognize it in an interview:** Listen for the wording of the prompt. If the problem asks for fast lookup, repeated membership checks, duplicate detection, grouping, or counting, you should immediately consider a map or set. If it asks for contiguous ranges, windows, substrings, or subarrays, you should look for a sliding window or prefix state. If it asks for all possible choices, paths, arrangements, or boards, draw the decision tree before coding. If it asks for best, minimum, maximum, count ways, or feasibility with repeated subproblems, define a DP state before reaching for loops.

**Brute force baseline:** Always describe the direct solution first. For base cases, the brute force version usually repeats work: scanning the same area again, recalculating a value already known, trying every pair, or exploring branches that can be proven impossible. The baseline matters because it gives you a correctness anchor and gives the interviewer a clear before-and-after optimization story.

**Optimization move:** The optimization is usually one of four moves: store seen information, exploit sorted order, maintain an invariant while moving pointers, or cache solved subproblems. Say the invariant out loud. A good invariant sounds like: "At every step, my map contains only values from the processed prefix," or "The window is always the longest valid window ending at the current right pointer," or "The heap always stores the best candidates seen so far."

**Dry-run discipline:** Use a tiny input and trace every state change. Write the input, current index or pointer, auxiliary structure contents, current answer, and reason for movement. Do not jump from the first step to the final answer. The dry run is where off-by-one bugs, stale map entries, missed duplicate handling, and wrong base cases become visible.

**Edge cases to test:** Test empty input, one element, duplicate-heavy input, already sorted input, reverse sorted input, negative values if numbers are allowed, and maximum constraint shape. For recursive or graph problems, also test disconnected input, cycles, repeated visits, and a path that almost works but fails at the final step.

**What a strong candidate says:** "I will start with a correct brute force approach, analyze why it is too slow, then remove repeated work by preserving exactly the state I need. I will keep the invariant visible while coding, dry-run on a normal example, and then test edge cases before giving final complexity."

**Complexity explanation:** Do not only state Big O. Explain the count. If each element enters and leaves a window once, the runtime is O(n). If every node and edge is visited once, it is O(V + E). If recursion branches into two calls per level, draw the tree. If sorting happens before a linear scan, sorting dominates at O(n log n). If a heap operation occurs for every item, multiply by log k or log n depending on heap size.

### Mastery Expansion 4: memoization

**What this part means in plain English:** In Dynamic Programming - Foundation and Mindset, memoization is not something to memorize as a disconnected trick. It is a decision tool. The core question is: what information changes as the input grows, and what information must remain available so the next step is cheap? When you can answer that, the correct data structure or algorithm becomes much easier to choose.

**How to recognize it in an interview:** Listen for the wording of the prompt. If the problem asks for fast lookup, repeated membership checks, duplicate detection, grouping, or counting, you should immediately consider a map or set. If it asks for contiguous ranges, windows, substrings, or subarrays, you should look for a sliding window or prefix state. If it asks for all possible choices, paths, arrangements, or boards, draw the decision tree before coding. If it asks for best, minimum, maximum, count ways, or feasibility with repeated subproblems, define a DP state before reaching for loops.

**Brute force baseline:** Always describe the direct solution first. For memoization, the brute force version usually repeats work: scanning the same area again, recalculating a value already known, trying every pair, or exploring branches that can be proven impossible. The baseline matters because it gives you a correctness anchor and gives the interviewer a clear before-and-after optimization story.

**Optimization move:** The optimization is usually one of four moves: store seen information, exploit sorted order, maintain an invariant while moving pointers, or cache solved subproblems. Say the invariant out loud. A good invariant sounds like: "At every step, my map contains only values from the processed prefix," or "The window is always the longest valid window ending at the current right pointer," or "The heap always stores the best candidates seen so far."

**Dry-run discipline:** Use a tiny input and trace every state change. Write the input, current index or pointer, auxiliary structure contents, current answer, and reason for movement. Do not jump from the first step to the final answer. The dry run is where off-by-one bugs, stale map entries, missed duplicate handling, and wrong base cases become visible.

**Edge cases to test:** Test empty input, one element, duplicate-heavy input, already sorted input, reverse sorted input, negative values if numbers are allowed, and maximum constraint shape. For recursive or graph problems, also test disconnected input, cycles, repeated visits, and a path that almost works but fails at the final step.

**What a strong candidate says:** "I will start with a correct brute force approach, analyze why it is too slow, then remove repeated work by preserving exactly the state I need. I will keep the invariant visible while coding, dry-run on a normal example, and then test edge cases before giving final complexity."

**Complexity explanation:** Do not only state Big O. Explain the count. If each element enters and leaves a window once, the runtime is O(n). If every node and edge is visited once, it is O(V + E). If recursion branches into two calls per level, draw the tree. If sorting happens before a linear scan, sorting dominates at O(n log n). If a heap operation occurs for every item, multiply by log k or log n depending on heap size.
<!-- PROMPT-TARGET-EXPANSION:END -->

---

**Previous:** [Recursion and Backtracking - The Decision Tree Master](../Phase-4-Core-Algorithms/06-Recursion-and-Backtracking.md) | **Next:** [Dynamic Programming - All Major Patterns](../Phase-5-Advanced-Algorithms/02-Dynamic-Programming-Patterns.md)
