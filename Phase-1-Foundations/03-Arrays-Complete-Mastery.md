# Arrays - The Foundation of All Data Structures

## Chapter Metadata

| Field | Value |
|---|---|
| Phase | Phase 1 - Foundations |
| Chapter | 3 of 37 |
| Difficulty | Beginner to Intermediate |
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

An array stores values in indexed order so each item can be reached by position.

Start simple: the interviewer is not testing whether you can recite textbook language. They are testing whether you can turn a problem into a reliable sequence of choices.

> 🧠 **Mental Model:** First understand what information must be stored, then decide how quickly it must be read, updated, or removed.

## Real-World Analogy

Think of numbered lockers: locker 0, locker 1, locker 2. If you know the locker number, access is instant.

The analogy matters because DSA is usually about trade-offs. A structure that is excellent for fast lookup may be poor for ordered traversal. A recursive solution may be elegant but may use extra call stack memory.

## Visual Representation

```text
Index:  0    1    2    3
Value: [10] [20] [30] [40]
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

- Contiguous memory model, index access, static vs dynamic arrays
- JavaScript arrays, V8 behavior, resizing, and amortized push
- DynamicArray class with push, pop, get, set, insert, delete
- Two pointers, sliding window, prefix sum, Kadane's algorithm, Dutch national flag
- Two Sum, Stock Buy/Sell, Product Except Self, Rotate Array, Merge Sorted Arrays
- 2D arrays, matrix traversal, spiral traversal, and transpose

## Deep Teaching Notes

### 1. Contiguous memory model, index access, static vs dynamic arrays

**Beginner explanation:** This is one of the core ideas for Arrays - The Foundation of All Data Structures. Start by saying it in plain language before reaching for code. A beginner should understand what problem this idea solves, what input it expects, and what output it creates.

**Why it matters:** In a FAANG interview, this point shows whether you understand the shape of the problem. Interviewers care less about memorized syntax and more about whether your choices match the constraints.

**How to reason about it:** Ask what must be remembered while the algorithm runs. If you need fast lookup, think HashMap or Set. If you need ordered movement, think pointers. If you need all possibilities, think recursion or backtracking. If you need best/count/possible over repeated subproblems, think dynamic programming.

**What to say out loud:** "I am choosing this approach because it matches the constraint: the expensive operation is repeated work, so I want a structure or pattern that removes that repetition."

**Implementation angle in JavaScript:** Prefer clear names, explicit loops when teaching, and built-ins only when you can explain their complexity. JavaScript gives you Array, Map, Set, and flexible objects, but every helper method still has a cost.

**Edge checks:** Confirm behavior for empty input, one item, duplicate values, already-ordered input, reverse-ordered input, and values at the smallest or largest allowed constraints.

### 2. JavaScript arrays, V8 behavior, resizing, and amortized push

**Beginner explanation:** This is one of the core ideas for Arrays - The Foundation of All Data Structures. Start by saying it in plain language before reaching for code. A beginner should understand what problem this idea solves, what input it expects, and what output it creates.

**Why it matters:** In a FAANG interview, this point shows whether you understand the shape of the problem. Interviewers care less about memorized syntax and more about whether your choices match the constraints.

**How to reason about it:** Ask what must be remembered while the algorithm runs. If you need fast lookup, think HashMap or Set. If you need ordered movement, think pointers. If you need all possibilities, think recursion or backtracking. If you need best/count/possible over repeated subproblems, think dynamic programming.

**What to say out loud:** "I am choosing this approach because it matches the constraint: the expensive operation is repeated work, so I want a structure or pattern that removes that repetition."

**Implementation angle in JavaScript:** Prefer clear names, explicit loops when teaching, and built-ins only when you can explain their complexity. JavaScript gives you Array, Map, Set, and flexible objects, but every helper method still has a cost.

**Edge checks:** Confirm behavior for empty input, one item, duplicate values, already-ordered input, reverse-ordered input, and values at the smallest or largest allowed constraints.

### 3. DynamicArray class with push, pop, get, set, insert, delete

**Beginner explanation:** This is one of the core ideas for Arrays - The Foundation of All Data Structures. Start by saying it in plain language before reaching for code. A beginner should understand what problem this idea solves, what input it expects, and what output it creates.

**Why it matters:** In a FAANG interview, this point shows whether you understand the shape of the problem. Interviewers care less about memorized syntax and more about whether your choices match the constraints.

**How to reason about it:** Ask what must be remembered while the algorithm runs. If you need fast lookup, think HashMap or Set. If you need ordered movement, think pointers. If you need all possibilities, think recursion or backtracking. If you need best/count/possible over repeated subproblems, think dynamic programming.

**What to say out loud:** "I am choosing this approach because it matches the constraint: the expensive operation is repeated work, so I want a structure or pattern that removes that repetition."

**Implementation angle in JavaScript:** Prefer clear names, explicit loops when teaching, and built-ins only when you can explain their complexity. JavaScript gives you Array, Map, Set, and flexible objects, but every helper method still has a cost.

**Edge checks:** Confirm behavior for empty input, one item, duplicate values, already-ordered input, reverse-ordered input, and values at the smallest or largest allowed constraints.

### 4. Two pointers, sliding window, prefix sum, Kadane's algorithm, Dutch national flag

**Beginner explanation:** This is one of the core ideas for Arrays - The Foundation of All Data Structures. Start by saying it in plain language before reaching for code. A beginner should understand what problem this idea solves, what input it expects, and what output it creates.

**Why it matters:** In a FAANG interview, this point shows whether you understand the shape of the problem. Interviewers care less about memorized syntax and more about whether your choices match the constraints.

**How to reason about it:** Ask what must be remembered while the algorithm runs. If you need fast lookup, think HashMap or Set. If you need ordered movement, think pointers. If you need all possibilities, think recursion or backtracking. If you need best/count/possible over repeated subproblems, think dynamic programming.

**What to say out loud:** "I am choosing this approach because it matches the constraint: the expensive operation is repeated work, so I want a structure or pattern that removes that repetition."

**Implementation angle in JavaScript:** Prefer clear names, explicit loops when teaching, and built-ins only when you can explain their complexity. JavaScript gives you Array, Map, Set, and flexible objects, but every helper method still has a cost.

**Edge checks:** Confirm behavior for empty input, one item, duplicate values, already-ordered input, reverse-ordered input, and values at the smallest or largest allowed constraints.

### 5. Two Sum, Stock Buy/Sell, Product Except Self, Rotate Array, Merge Sorted Arrays

**Beginner explanation:** This is one of the core ideas for Arrays - The Foundation of All Data Structures. Start by saying it in plain language before reaching for code. A beginner should understand what problem this idea solves, what input it expects, and what output it creates.

**Why it matters:** In a FAANG interview, this point shows whether you understand the shape of the problem. Interviewers care less about memorized syntax and more about whether your choices match the constraints.

**How to reason about it:** Ask what must be remembered while the algorithm runs. If you need fast lookup, think HashMap or Set. If you need ordered movement, think pointers. If you need all possibilities, think recursion or backtracking. If you need best/count/possible over repeated subproblems, think dynamic programming.

**What to say out loud:** "I am choosing this approach because it matches the constraint: the expensive operation is repeated work, so I want a structure or pattern that removes that repetition."

**Implementation angle in JavaScript:** Prefer clear names, explicit loops when teaching, and built-ins only when you can explain their complexity. JavaScript gives you Array, Map, Set, and flexible objects, but every helper method still has a cost.

**Edge checks:** Confirm behavior for empty input, one item, duplicate values, already-ordered input, reverse-ordered input, and values at the smallest or largest allowed constraints.

### 6. 2D arrays, matrix traversal, spiral traversal, and transpose

**Beginner explanation:** This is one of the core ideas for Arrays - The Foundation of All Data Structures. Start by saying it in plain language before reaching for code. A beginner should understand what problem this idea solves, what input it expects, and what output it creates.

**Why it matters:** In a FAANG interview, this point shows whether you understand the shape of the problem. Interviewers care less about memorized syntax and more about whether your choices match the constraints.

**How to reason about it:** Ask what must be remembered while the algorithm runs. If you need fast lookup, think HashMap or Set. If you need ordered movement, think pointers. If you need all possibilities, think recursion or backtracking. If you need best/count/possible over repeated subproblems, think dynamic programming.

**What to say out loud:** "I am choosing this approach because it matches the constraint: the expensive operation is repeated work, so I want a structure or pattern that removes that repetition."

**Implementation angle in JavaScript:** Prefer clear names, explicit loops when teaching, and built-ins only when you can explain their complexity. JavaScript gives you Array, Map, Set, and flexible objects, but every helper method still has a cost.

**Edge checks:** Confirm behavior for empty input, one item, duplicate values, already-ordered input, reverse-ordered input, and values at the smallest or largest allowed constraints.


## Complete Implementation

```javascript
/**
 * Returns indices of two numbers that add up to target.
 * Time: O(n), Space: O(n)
 */
function twoSum(numbers, target) {
  const valueToIndex = new Map();

  for (let index = 0; index < numbers.length; index += 1) {
    const currentValue = numbers[index];
    const neededValue = target - currentValue;

    if (valueToIndex.has(neededValue)) {
      return [valueToIndex.get(neededValue), index];
    }

    valueToIndex.set(currentValue, index);
  }

  return [];
}

console.log(twoSum([2, 7, 11, 15], 9));
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

### Problem 1: Two Sum

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

### Problem 2: Product of Array Except Self

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

### Problem 3: Maximum Subarray

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

- `DSA JS/src/data-structures/arrays/notes.md`
- `DSA JS/src/data-structures/arrays/2d-arrays/notes.md`
- `DSA JS/src/data-structures/arrays/2d-arrays/implementation.js`

### Imported Notes: `DSA JS/src/data-structures/arrays/notes.md`

# 📦 JavaScript Arrays — Complete Master Notes (DSA + Interview)

---

# 1️⃣ Definition (Interview Ready)

An **Array** is a linear data structure that stores multiple values in a sequence and allows access using **0-based indexing**.

- Linear → Elements stored one after another
- Indexed → Access using position

```js
const arr = []
arr.push('Hello')
arr.push(1)
arr.pop()
console.log(arr[0])
```

---

# 2️⃣ Important Properties

- Index starts from 0
- Arrays are dynamic in JavaScript
- Can store mixed data types
- Internally arrays are objects
- typeof [] === "object"

```js
const mixed = [1, 'two', true, null]
```

---

# 3️⃣ Sparse Arrays (Avoid in DSA)

```js
const arr = []
arr[5] = 100
console.log(arr)
```

⚠️ This creates empty slots before index 5.

Avoid sparse arrays in interviews.

---

# 4️⃣ Creating Arrays

## Recommended

```js
const a = [1, 2, 3]
```

## Constructor (Be Careful)

```js
const b = new Array(3)
```

⚠️ Creates empty slots, not values.

---

# 5️⃣ Basic Operations

## Sum of Elements

```js
let sum = 0
for (let i = 0; i < arr.length; i++) {
  sum += arr[i]
}
```

Using reduce:

```js
const sum = arr.reduce((acc, curr) => acc + curr, 0)
```

Time: O(n)

---

# 6️⃣ Maximum Element

````js
function maximum(arr) {
  let max = arr[0]
  for (let i = 1; i < arr.length; i++) {
    if (arr[i] > max) max = arr[i]
  }
  return max
}
```z`

Time: O(n) | Space: O(1)

---

# 7️⃣ Minimum Element

```js
let min = arr[0]
for (let i = 1; i < arr.length; i++) {
  if (arr[i] < min) min = arr[i]
}
````

---

# 8️⃣ Second Maximum (Important 🔥)

```js
function secondMax(arr) {
  let max = -Infinity
  let sMax = -Infinity

  for (const num of arr) {
    if (num > max) {
      sMax = max
      max = num
    } else if (num > sMax && num < max) {
      sMax = num
    }
  }
  return sMax
}
```

Time: O(n)

---

# 9️⃣ Reverse Array

## With Extra Space

```js
const rev = []
for (let i = arr.length - 1; i >= 0; i--) {
  rev.push(arr[i])
}
```

## In-place (Best)

```js
let i = 0,
  j = arr.length - 1
while (i < j) {
  ;[arr[i], arr[j]] = [arr[j], arr[i]]
  i++
  j--
}
```

Time: O(n) | Space: O(1)

---

# 🔟 Rotation Problems

## Left Rotate by 1

```js
let first = arr[0]
for (let i = 0; i < arr.length - 1; i++) {
  arr[i] = arr[i + 1]
}
arr[arr.length - 1] = first
```

---

## Right Rotate by 1

```js
let last = arr[arr.length - 1]
for (let i = arr.length - 1; i > 0; i--) {
  arr[i] = arr[i - 1]
}
arr[0] = last
```

---

## Rotate by K (Efficient Extra Space)

```js
let temp = new Array(arr.length)
k = k % arr.length

for (let i = 0; i < arr.length; i++) {
  temp[i] = arr[(i + k) % arr.length]
}
```

````js
// Right rotation
function rotateRight(array, k) {
let n = array.length

let temp = new Array(n)
k = k % n

for (let index = 0; index < n; index++) {
temp[(index + k) % n] = array[index]
}

console.log(temp)
}

## rotateRight([1,2,3,4,5], 3)

# 1️⃣1️⃣ Remove Duplicates (Sorted Array)

Two-pointer pattern.

```js
function removeDuplicates(arr) {
  let j = 0
  for (let i = 1; i < arr.length; i++) {
    if (arr[i] !== arr[j]) {
      j++
      arr[j] = arr[i]
    }
  }
  arr.length = j + 1
  return arr
}
````

Time: O(n) | Space: O(1)

---

# 1️⃣2️⃣ Merge Two Sorted Arrays

```js
function mergeArray(array1, array2) {
  let i = 0
  let j = 0
  let merge = []

  while (i < array1.length && j < array2.length) {
    if (array1[i] < array2[j]) {
      merge.push(array1[i])
      i++
    } else {
      merge.push(array2[j])
      j++
    }
  }

  // remaining elements
  while (i < array1.length) {
    merge.push(array1[i])
    i++
  }

  while (j < array2.length) {
    merge.push(array2[j])
    j++
  }

  return merge
}

console.log(mergeArray([1, 2, 3, 4], [5, 6, 7, 8]))
```

Time: O(n + m)

---

z`

# 1️⃣3️⃣ Kadane’s Algorithm (Maximum Subarray)

````js
function kadane(arr) {
  let currentSum = 0
  let maxSum = -Infinity

  for (let num of arr) {
    currentSum += num

    maxSum = Math.max(maxSum, currentSum)

    if (currentSum < 0) {
      currentSum = 0
    }
  }

  return maxSum
}

console.log(kadane([-2, 3, -1, 4, -5]))```

Time: O(n) | Space: O(1)

---

# 1️⃣4️⃣ Majority Element (Moore’s Voting)

```
````

Time: O(n) | Space: O(1)

---

# 1️⃣5️⃣ Dutch National Flag (Sort 0,1,2)

```jsz
let low = 0,
  mid = 0,
  high = arr.length - 1

while (mid <= high) {
  if (arr[mid] === 0) {
    ;[arr[low], arr[mid]] = [arr[mid], arr[low]]
    low++
    mid++
  } else if (arr[mid] === 2) {
    ;[arr[mid], arr[high]] = [arr[high], arr[mid]]
    high--
  } else {
    mid++
  }
}
```

Time: O(n) | Space: O(1)

---

# 1️⃣6️⃣ Two Sum (Sorted Array - Two Pointer)

```js
function twoSum(nums, target) {
  let map = new Map()

  for (let i = 0; i < nums.length; i++) {
    let needed = target - nums[i]

    if (map.has(needed)) {
      return [map.get(needed), i]
    }

    map.set(nums[i], i)
  }
}
// 2️⃣ Palindrome Number

function Palindram(nums) {
  let origianl = nums
  let reverse = 0

  while (nums > 0) {
    let lastDigit = nums % 10
    reverse = reverse * 10 + lastDigit
    nums = Math.floor(nums / 10)
  }

  return origianl === reverse
}
```

---

# 📊 Complexity Cheat Sheet

| Operation       | Time |
| --------------- | ---- |
| Access          | O(1) |
| Search          | O(n) |
| Insert at End   | O(1) |
| Insert at Start | O(n) |
| Delete          | O(n) |
| Reverse         | O(n) |
| Rotate          | O(n) |

---

# 🧠 Interview Patterns Summary

- Rotation → Modulo logic
- Sorted array → Two pointers
- Subarray sum → Kadane
- Frequency dominance → Moore Voting
- 0/1/2 sorting → Three pointers
- Merge arrays → Two pointers

---

# ✅ Mastery Checklist

✔ Array basics
✔ Two pointer technique
✔ Rotation problems
✔ Subarray problems
✔ Majority element
✔ Sorting patterns

---

🔥 These cover 80% of array interview questions (FAANG level).

End of JavaScript Arrays Master Notes

### Imported Notes: `DSA JS/src/data-structures/arrays/2d-arrays/notes.md`

# 🧮 2D Array (Matrix) – Complete Notes (JavaScript)

A **2D Array (Matrix)** is an array of arrays. It is mainly used to represent **tables, grids, and matrices**.

---

## 📌 Basic Structure

```js
const matrix = [
  [1, 2, 3],
  [4, 5, 6],
]
```

- `matrix.length` → number of rows
- `matrix[i].length` → number of columns in row `i`

---

## 🔁 Traversing a 2D Array

```js
for (let i = 0; i < matrix.length; i++) {
  for (let j = 0; j < matrix[i].length; j++) {
    console.log(matrix[i][j])
  }
}
```

---

## 🔍 Find Maximum Element in 2D Array

```js
const array = [
  [1, 2, 3],
  [4, 5, 6],
]

let maximum = array[0][0]

for (let i = 0; i < array.length; i++) {
  for (let j = 0; j < array[i].length; j++) {
    if (array[i][j] > maximum) {
      maximum = array[i][j]
    }
  }
}

console.log(maximum) // 6
```

---

## ➕ Sum of All Elements

```js
const array = [
  [1, 2, 3],
  [4, 5, 6],
]

let sum = 0

for (let i = 0; i < array.length; i++) {
  for (let j = 0; j < array[i].length; j++) {
    sum += array[i][j]
  }
}

console.log(sum) // 21
```

---

## 🔎 Linear Search in 2D Array

```js
const array = [
  [1, 2, 3],
  [4, 5, 6],
]

let target = 5
let found = false

for (let i = 0; i < array.length; i++) {
  for (let j = 0; j < array[i].length; j++) {
    if (array[i][j] === target) {
      console.log(`Found at row ${i}, column ${j}`)
      found = true
    }
  }
}
```

---

## 🔄 Transpose of a Matrix

> Rows become columns and columns become rows

```js
const array = [
  [1, 2, 3],
  [4, 5, 6],
]

let transpose = []

for (let i = 0; i < array.length; i++) {
  for (let j = 0; j < array[i].length; j++) {
    if (!transpose[j]) transpose[j] = []
    transpose[j][i] = array[i][j]
  }
}

console.log(transpose)
// [[1,4],[2,5],[3,6]]
```

---

## 🔁 Rotate Matrix by 90° Clockwise

### 🧠 Algorithm

1. Transpose the matrix
2. Reverse each row

```js
const matrix = [
  [1, 2, 3],
  [4, 5, 6],
  [7, 8, 9],
]

// STEP 1: Transpose
for (let i = 0; i < matrix.length; i++) {
  for (let j = i; j < matrix.length; j++) {
    let temp = matrix[i][j]
    matrix[i][j] = matrix[j][i]
    matrix[j][i] = temp
  }
}

// STEP 2: Reverse each row
for (let i = 0; i < matrix.length; i++) {
  matrix[i].reverse()
}

console.log(matrix)
```

---

## 🚫 Set Matrix Zeros

> If any cell is 0, set its entire row & column to 0

```js
const Matrix = [
  [1, 1, 1],
  [1, 0, 1],
  [1, 1, 1],
]

let rows = Matrix.length
let cols = Matrix[0].length

let rowZero = new Array(rows).fill(false)
let colZero = new Array(cols).fill(false)

// STEP 1: Mark rows & columns
for (let i = 0; i < rows; i++) {
  for (let j = 0; j < cols; j++) {
    if (Matrix[i][j] === 0) {
      rowZero[i] = true
      colZero[j] = true
    }
  }
}

// STEP 2: Set zeroes
for (let i = 0; i < rows; i++) {
  for (let j = 0; j < cols; j++) {
    if (rowZero[i] || colZero[j]) {
      Matrix[i][j] = 0
    }
  }
}

console.log(Matrix)
```

---

## 🌀 Spiral Traversal of Matrix

### Example

Input:

```js
;[
  [1, 2, 3],
  [4, 5, 6],
  [7, 8, 9],
]
```

Output:

```
[1, 2, 3, 6, 9, 8, 7, 4, 5]
```

### Code

```js
const matrix = [
  [1, 2, 3],
  [4, 5, 6],
  [7, 8, 9],
]

let top = 0
let bottom = matrix.length - 1
let left = 0
let right = matrix[0].length - 1

let result = []

while (top <= bottom && left <= right) {
  // left → right
  for (let i = left; i <= right; i++) {
    result.push(matrix[top][i])
  }
  top++

  // top → bottom
  for (let i = top; i <= bottom; i++) {
    result.push(matrix[i][right])
  }
  right--

  // right → left
  if (top <= bottom) {
    for (let i = right; i >= left; i--) {
      result.push(matrix[bottom][i])
    }
    bottom--
  }

  // bottom → top
  if (left <= right) {
    for (let i = bottom; i >= top; i--) {
      result.push(matrix[i][left])
    }
    left++
  }
}

console.log(result)
```

---

## ✅ Key Points to Remember

- Always use **nested loops** for 2D arrays
- `i` → rows, `j` → columns
- Matrix problems are **very important for interviews**
- Practice transpose, rotation, and traversal

### Imported Implementation: `DSA JS/src/data-structures/arrays/2d-arrays/implementation.js`

```javascript
// ===*Spiral Trasversal*===
```
<!-- DSA-JS-MERGE:END -->

---

**Previous:** [Big O Notation - The Language of Algorithm Efficiency](../Phase-1-Foundations/02-Big-O-Notation-Complete-Guide.md) | **Next:** [Strings - Mastery from a DSA Perspective](../Phase-1-Foundations/04-Strings-DSA-Perspective.md)
