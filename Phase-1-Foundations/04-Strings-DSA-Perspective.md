# Strings - Mastery from a DSA Perspective

## Chapter Metadata

| Field | Value |
|---|---|
| Phase | Phase 1 - Foundations |
| Chapter | 4 of 37 |
| Difficulty | Beginner to Intermediate |
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

A string is a sequence of characters, and most interview string problems are array problems with character rules.

Start simple: the interviewer is not testing whether you can recite textbook language. They are testing whether you can turn a problem into a reliable sequence of choices.

> 🧠 **Mental Model:** First understand what information must be stored, then decide how quickly it must be read, updated, or removed.

## Real-World Analogy

A word is like a train: each character is a carriage, and order matters.

The analogy matters because DSA is usually about trade-offs. A structure that is excellent for fast lookup may be poor for ordered traversal. A recursive solution may be elegant but may use extra call stack memory.

## Visual Representation

```text
s = "code"
index: 0 1 2 3
char:  c o d e
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

- Strings as character arrays and the cost of immutability
- Efficient string building with array join
- Character codes, ASCII math, and frequency arrays
- Anagrams, palindromes, reversal, substring problems, and pattern matching
- Two pointers, HashMap frequency, sliding window, and regular expressions

## Deep Teaching Notes

### 1. Strings as character arrays and the cost of immutability

**Beginner explanation:** This is one of the core ideas for Strings - Mastery from a DSA Perspective. Start by saying it in plain language before reaching for code. A beginner should understand what problem this idea solves, what input it expects, and what output it creates.

**Why it matters:** In a FAANG interview, this point shows whether you understand the shape of the problem. Interviewers care less about memorized syntax and more about whether your choices match the constraints.

**How to reason about it:** Ask what must be remembered while the algorithm runs. If you need fast lookup, think HashMap or Set. If you need ordered movement, think pointers. If you need all possibilities, think recursion or backtracking. If you need best/count/possible over repeated subproblems, think dynamic programming.

**What to say out loud:** "I am choosing this approach because it matches the constraint: the expensive operation is repeated work, so I want a structure or pattern that removes that repetition."

**Implementation angle in JavaScript:** Prefer clear names, explicit loops when teaching, and built-ins only when you can explain their complexity. JavaScript gives you Array, Map, Set, and flexible objects, but every helper method still has a cost.

**Edge checks:** Confirm behavior for empty input, one item, duplicate values, already-ordered input, reverse-ordered input, and values at the smallest or largest allowed constraints.

### 2. Efficient string building with array join

**Beginner explanation:** This is one of the core ideas for Strings - Mastery from a DSA Perspective. Start by saying it in plain language before reaching for code. A beginner should understand what problem this idea solves, what input it expects, and what output it creates.

**Why it matters:** In a FAANG interview, this point shows whether you understand the shape of the problem. Interviewers care less about memorized syntax and more about whether your choices match the constraints.

**How to reason about it:** Ask what must be remembered while the algorithm runs. If you need fast lookup, think HashMap or Set. If you need ordered movement, think pointers. If you need all possibilities, think recursion or backtracking. If you need best/count/possible over repeated subproblems, think dynamic programming.

**What to say out loud:** "I am choosing this approach because it matches the constraint: the expensive operation is repeated work, so I want a structure or pattern that removes that repetition."

**Implementation angle in JavaScript:** Prefer clear names, explicit loops when teaching, and built-ins only when you can explain their complexity. JavaScript gives you Array, Map, Set, and flexible objects, but every helper method still has a cost.

**Edge checks:** Confirm behavior for empty input, one item, duplicate values, already-ordered input, reverse-ordered input, and values at the smallest or largest allowed constraints.

### 3. Character codes, ASCII math, and frequency arrays

**Beginner explanation:** This is one of the core ideas for Strings - Mastery from a DSA Perspective. Start by saying it in plain language before reaching for code. A beginner should understand what problem this idea solves, what input it expects, and what output it creates.

**Why it matters:** In a FAANG interview, this point shows whether you understand the shape of the problem. Interviewers care less about memorized syntax and more about whether your choices match the constraints.

**How to reason about it:** Ask what must be remembered while the algorithm runs. If you need fast lookup, think HashMap or Set. If you need ordered movement, think pointers. If you need all possibilities, think recursion or backtracking. If you need best/count/possible over repeated subproblems, think dynamic programming.

**What to say out loud:** "I am choosing this approach because it matches the constraint: the expensive operation is repeated work, so I want a structure or pattern that removes that repetition."

**Implementation angle in JavaScript:** Prefer clear names, explicit loops when teaching, and built-ins only when you can explain their complexity. JavaScript gives you Array, Map, Set, and flexible objects, but every helper method still has a cost.

**Edge checks:** Confirm behavior for empty input, one item, duplicate values, already-ordered input, reverse-ordered input, and values at the smallest or largest allowed constraints.

### 4. Anagrams, palindromes, reversal, substring problems, and pattern matching

**Beginner explanation:** This is one of the core ideas for Strings - Mastery from a DSA Perspective. Start by saying it in plain language before reaching for code. A beginner should understand what problem this idea solves, what input it expects, and what output it creates.

**Why it matters:** In a FAANG interview, this point shows whether you understand the shape of the problem. Interviewers care less about memorized syntax and more about whether your choices match the constraints.

**How to reason about it:** Ask what must be remembered while the algorithm runs. If you need fast lookup, think HashMap or Set. If you need ordered movement, think pointers. If you need all possibilities, think recursion or backtracking. If you need best/count/possible over repeated subproblems, think dynamic programming.

**What to say out loud:** "I am choosing this approach because it matches the constraint: the expensive operation is repeated work, so I want a structure or pattern that removes that repetition."

**Implementation angle in JavaScript:** Prefer clear names, explicit loops when teaching, and built-ins only when you can explain their complexity. JavaScript gives you Array, Map, Set, and flexible objects, but every helper method still has a cost.

**Edge checks:** Confirm behavior for empty input, one item, duplicate values, already-ordered input, reverse-ordered input, and values at the smallest or largest allowed constraints.

### 5. Two pointers, HashMap frequency, sliding window, and regular expressions

**Beginner explanation:** This is one of the core ideas for Strings - Mastery from a DSA Perspective. Start by saying it in plain language before reaching for code. A beginner should understand what problem this idea solves, what input it expects, and what output it creates.

**Why it matters:** In a FAANG interview, this point shows whether you understand the shape of the problem. Interviewers care less about memorized syntax and more about whether your choices match the constraints.

**How to reason about it:** Ask what must be remembered while the algorithm runs. If you need fast lookup, think HashMap or Set. If you need ordered movement, think pointers. If you need all possibilities, think recursion or backtracking. If you need best/count/possible over repeated subproblems, think dynamic programming.

**What to say out loud:** "I am choosing this approach because it matches the constraint: the expensive operation is repeated work, so I want a structure or pattern that removes that repetition."

**Implementation angle in JavaScript:** Prefer clear names, explicit loops when teaching, and built-ins only when you can explain their complexity. JavaScript gives you Array, Map, Set, and flexible objects, but every helper method still has a cost.

**Edge checks:** Confirm behavior for empty input, one item, duplicate values, already-ordered input, reverse-ordered input, and values at the smallest or largest allowed constraints.


## Complete Implementation

```javascript
/**
 * Checks whether two strings are anagrams.
 * Time: O(n), Space: O(1) for lowercase English letters
 */
function isValidAnagram(firstWord, secondWord) {
  if (firstWord.length !== secondWord.length) return false;

  const counts = new Array(26).fill(0);
  const baseCode = "a".charCodeAt(0);

  for (let index = 0; index < firstWord.length; index += 1) {
    counts[firstWord.charCodeAt(index) - baseCode] += 1;
    counts[secondWord.charCodeAt(index) - baseCode] -= 1;
  }

  return counts.every((count) => count === 0);
}

console.log(isValidAnagram("listen", "silent"));
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

### Problem 1: Valid Anagram

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

### Problem 2: Longest Substring Without Repeating Characters

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

### Problem 3: Valid Palindrome

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

- `DSA JS/src/data-structures/strings/notes.md`
- `DSA JS/src/data-structures/strings/practice.md`

### Imported Notes: `DSA JS/src/data-structures/strings/notes.md`

What is a String?
A string is a sequence of characters (letters, numbers, symbols, or spaces) stored inside quotes. In JavaScript, strings are primitive data types and are immutable (cannot be changed in-place after creation). Any "modification" creates a new string.

Types of Quotes
Single Quotes: 'Umar' – Ideal for simple strings.
Double Quotes: "Janii" – Also for simple strings; useful when including single quotes inside.
Template Literals (Backticks): `Hello ${a}` – Allows interpolation (embedding variables/expressions) and multi-line strings without escape characters.
js

````js
let a = 'Umar';        // Single quotes
let b = "Janii";       // Double quotes
let c = `Hello ${a}`;  // Template literal (interpolation)
console.log(c);        // Output: Hello Umar
Key Point: Strings are immutable. Operations like concatenation or slicing return new strings.

String Indexing
Strings use zero-based indexing, meaning the first character is at index 0. You can access individual characters using bracket notation (str[index]).

js

```js
const str = 'umar';
console.log(str[0]);  // 'u'
console.log(str[1]);  // 'm'
console.log(str[3]);  // 'r'
console.log(str[4]);  // undefined (out of bounds)
Note: Negative indexing (e.g., str[-1]) is not supported natively; use slice() for that.

Length of String
The length property returns the number of characters in the string.

js

```js
const str = 'umar';
console.log(str.length);  // 4
Edge Case: Empty string '' has length 0.

Traversing / Looping a String
Strings can be looped like arrays. Use for...of for simplicity or traditional for for index-based access.

for...of Loop (Modern, Readable)
js

```js
for (const ch of 'Umar') {
  console.log(ch);  // Outputs: U, m, a, r (one per line)
}
Traditional for Loop (Index-Based)
js

```js
const s = 'Hello';
for (let i = 0; i < s.length; i++) {
  console.log(s[i]);  // Outputs: H, e, l, l, o
}
Time Complexity: O(n) for both (linear traversal).

Tip: Prefer for...of for character iteration; use traditional for when you need indices.

Escape Characters
Escape sequences allow special characters in strings. They start with a backslash (\).

Escape Sequence

Meaning

Example Output

\'

Single Quote

'It\'s' → It's

\"

Double Quote

"He said \"Hi\"" → He said "Hi"

\\

Backslash

'Path\\to\\file' → Path\to\file

\n

New Line

'Hello\nWorld' → Hello (newline) World

\t

Tab

'Name\tAge' → Name Age

js

```js
console.log('Hello\nWorld');  // Outputs on two lines
console.log('Tab:\tHere');    // Outputs with tab space
Use Case: Essential for formatting output or handling user input with special chars.

Important String Methods (Core DSA)
These are built-in methods for manipulation. Remember, they return new strings due to immutability.

charAt(index)
Returns the character at a specific index (safer than bracket notation for out-of-bounds).

js

```js
'Janii'.charAt(2);  // 'n'
'Janii'.charAt(10); // '' (empty string, no error)
toUpperCase() / toLowerCase()
Converts case.

js

```js
'hello'.toUpperCase();  // 'HELLO'
'WORLD'.toLowerCase();  // 'world'
Interview Note: Avoid in pure DSA problems; use ASCII for custom logic.

Searching in String
Methods to find substrings or characters.

indexOf(substring, startIndex?)
Returns the first index of the substring (or -1 if not found). Optional start index.

js

```js
'Umar Khan'.indexOf('Khan');     // 5
'Umar Khan'.indexOf('Khan', 6);  // -1 (starts searching from index 6)
lastIndexOf(substring, startIndex?)
Returns the last index of the substring.

js

```js
'hello hello'.lastIndexOf('hello');  // 6
includes(substring)
Checks if the substring exists (returns boolean).

js

```js
'email@gmail.com'.includes('@');  // true
'hello'.includes('x');            // false
startsWith(substring) / endsWith(substring)
Checks prefix/suffix.

js

```js
'Hello World'.startsWith('Hello');  // true
'Hello World'.endsWith('World');    // true
Time Complexity: O(n) for all (worst-case scan).

Search & Match (Interview Use)
For regex-based searching (common in advanced problems).

search(regex)
Returns the index of the first match (or -1).

js

```js
'I love JS'.search('love');  // 2
'I love JS'.search(/love/i); // 2 (case-insensitive with regex)
match(regex)
Returns an array of matches (or null).

js

```js
'Hi Hi'.match(/Hi/g);  // ['Hi', 'Hi'] (global flag for all matches)
'Hi Hi'.match(/Hi/);   // ['Hi'] (first match only)
Tip: Regex is powerful for patterns but can be slow; use for interviews requiring pattern matching.

Slice (Very Important)
Extracts a substring from start to end (exclusive). Supports negative indices (counts from end).

js

```js
const str = 'JavaScript';
str.slice(0, 4);   // 'Java' (indices 0-3)
str.slice(4);      // 'Script' (from 4 to end)
str.slice(-6);     // 'Script' (last 6 chars)
str.slice(2, -2);  // 'vaScri' (from 2 to 2nd last)
Time Complexity: O(n) (creates new string).

DSA Use: Core for substring problems; efficient for extraction.

concat()
Joins strings (alternative to + operator).

js

```js
'Hello'.concat(' ', 'World');  // 'Hello World'
'Hi'.concat(' there', '!');    // 'Hi there!'
Time Complexity: O(n + m) where n and m are string lengths.

charCodeAt() & fromCharCode()
ASCII manipulation (crucial for hashing, encryption, and frequency problems).

charCodeAt(index): Returns ASCII code of char at index.
String.fromCharCode(code): Returns char from ASCII code.
js

```js
'A'.charCodeAt(0);          // 65 (ASCII for 'A')
String.fromCharCode(65);    // 'A'
'abc'.charCodeAt(1);        // 98 ('b')
String.fromCharCode(97, 98, 99);  // 'abc' (multiple codes)
Ranges: A-Z: 65-90, a-z: 97-122, 0-9: 48-57.

DSA Use: Frequency counts, case toggles, cipher problems.

split() → String to Array
Splits string into an array based on a separator.

js

```js
'I love JS'.split(' ');     // ['I', 'love', 'JS']
'hello-world'.split('-');   // ['hello', 'world']
'abc'.split('');            // ['a', 'b', 'c'] (empty separator splits chars)
'a,b,c'.split(',');         // ['a', 'b', 'c']
Time Complexity: O(n).

DSA Use: Convert to array for sorting, reversing, or further processing.

replace(searchValue, replaceValue)
Replaces the first occurrence of a substring (or regex).

js

```js
'Hello World'.replace('World', 'JS');  // 'Hello JS'
'foo foo'.replace('foo', 'bar');       // 'bar foo' (only first)
'foo foo'.replace(/foo/g, 'bar');      // 'bar bar' (global with regex)
Time Complexity: O(n).

Note: For all occurrences, use regex with global flag.

Reverse a String (Classic DSA)
Reverses the string by building a new one.

js

```js
function reverseString(s) {
  let res = '';
  for (let i = s.length - 1; i >= 0; i--) {
    res += s[i];
  }
  return res;
}

console.log(reverseString('hello'));  // 'olleh'
Time: O(n) | Space: O(n) (new string).

Alternative (Cheat): 'hello'.split('').reverse().join('') – but avoid in interviews for manual practice.

Palindrome Check (Two Pointer – Google Favorite)
Checks if a string reads the same forwards and backwards using two pointers.

js

```js
function isPalindrome(s) {
  let i = 0, j = s.length - 1;
  while (i < j) {
    if (s[i] !== s[j]) return false;
    i++;
    j--;
  }
  return true;
}

console.log(isPalindrome('racecar'));  // true
console.log(isPalindrome('hello'));    // false
Time: O(n) | Space: O(1).

Asked in: Google, Amazon, Meta. Handles case-sensitive checks; extend for case-insensitive by converting to lower.

String Immutability (IMPORTANT CONCEPT)
Strings cannot be mutated in-place. Attempts to change fail silently.

js

```js
let s = 'abc';
s[0] = 'z';          // No effect
console.log(s);      // 'abc' (unchanged)
s = s + 'd';         // Creates new string
console.log(s);      // 'abcd'
Why?: JavaScript treats strings as primitives. Always assign to a new variable or use methods that return new strings.

Toggle Character Case & Character Frequency (Google-Level DSA)
Problem 1: Toggle Character Case (Upper ↔ Lower)
Convert uppercase to lowercase and vice versa.

Example: Input: "JaNi" → Output: "jAnI"

Algorithm:

Traverse each char.
Use ASCII: Upper (65-90) → add 32; Lower (97-122) → subtract 32.
Handle non-letters unchanged.
js

```js

function toggleString(str) {
  let result = '';
  for (let i = 0; i < str.length; i++) {
    let ch = str.charCodeAt(i);
    if (ch >= 65 && ch <= 90) {
      result += String.fromCharCode(ch + 32);
    } else if (ch >= 97 && ch <= 122) {
      result += String.fromCharCode(ch - 32);
    } else {
      result += str[i];
    }
  }
  return result;
}

console.log(toggleString('JaNi'));  // 'jAnI'
Time: O(n) | Space: O(n).

Interview Tip: Avoid toUpperCase(); ASCII shows fundamentals.

Problem 2: Character Frequency Counter
Count occurrences of each character.

Example: Input: "google" → Output: g:2, o:2, l:1, e:1

Algorithm:

Use fixed-size array (128 for ASCII) or object.
Increment counts.
Print non-zero.
js

```js
function charCounter(str) {
  const freq = new Array(128).fill(0);
  for (let i = 0; i < str.length; i++) {
    freq[str.charCodeAt(i)]++;
  }
  for (let i = 0; i < freq.length; i++) {
    if (freq[i] > 0) {
      console.log(`${String.fromCharCode(i)} → ${freq[i]}`);
    }
  }
}

charCounter('google');  // g → 2, o → 2, l → 1, e → 1
Time: O(n) | Space: O(1) (fixed array).

Alternative (Object-Based):

js


function frequencyCounter(string) {
  let counter = {}

  for (let i = 0; i < string.length; i++) {
    if (counter[string[i]]) {
      counter[string[i]] += 1
    } else {
      counter[string[i]] = 1
    }
  }

  return counter
}

console.log(frequencyCoun('google'))

```js
function frequencyCount(str) {
  let freq = {};
  for (let char of str) {
    freq[char] = (freq[char] || 0) + 1;
  }
  return freq;  // {g:2, o:2, l:1, e:1}
}
Problem 3: Anagram Check (Using Frequency)
Check if two strings are anagrams (same chars, same counts).

js

```js
function isAnagram(s, t) {
  if (s.length !== t.length) return false;
  let count = {};
  for (let char of s) {
    count[char] = (count[char] || 0) + 1;
  }
  for (let char of t) {
    if (!count[char]) return false;
    count[char]--;
  }
  return true;
}



## Longest Substring Without Repeating

function lengthOfLongestSubstring(s) {

  let maxLength = 0
  let set = new Set()
  let left = 0

  for (let right = 0; right < s.length; right++) {

    while (set.has(s[right])) {
      set.delete(s[left])
      left++
    }

    set.add(s[right])

    maxLength = Math.max(maxLength, right - left + 1)
  }

  return maxLength
}

console.log(lengthOfLongestSubstring("hellhellhell"))




## String Matching


var strStr = function (haystack, needle) {

    for (let i = 0; i <= haystack.length - needle.length; i++) {

        let j = 0

        while (j < needle.length && haystack[i + j] === needle[j]) {
            j++
        }

        if (j === needle.length) {
            return i
        }
    }

    return -1
};



console.log(isAnagram('listen', 'silent'));  // true
Time: O(n) | Space: O(1) (fixed alphabet).

Common DSA String Problems
Reverse String (Manual loop or built-ins).
Palindrome Check (Two Pointers).
Anagram Check (Frequency Map).
Frequency Count (Array or Object).
Longest Substring Without Repeating Characters (Sliding Window).
Valid Parentheses (Stack).
Remove Duplicates (Set or Frequency).
String Compression (Run-Length Encoding, e.g., "aaabb" → "a3b2").
Group Anagrams (Hash Map).
Longest Palindromic Substring (Expand Around Center).
Practice: LeetCode #5, #125, #242, #3, #20.







New string

Interview Tip (VERY IMPORTANT)
💡 Strings behave like arrays but are immutable. Always create new strings for "modifications." Think in terms of Two Pointers (palindromes), Frequency Maps (anagrams/counts), or Sliding Window (substrings). Master ASCII for custom logic. Edge cases: empty strings, mixed case, special chars. Practice on LeetCode for speed.

  Additional Code Examples
  Anagram Check
js

```js
function isAnagram(s, t) {
  if (s.length !== t.length) return false
  const freq = {}
  for (let c of s) freq[c] = (freq[c] || 0) + 1
  for (let c of t) {
    if (!freq[c]) return false
    freq[c]--
  }
  return true
}
Length of Longest Substring Without Repeating Characters


```js
function lengthOfLongestSubstring(s) {
  let set = new Set()
  let maxLen = 0
  let start = 0

  for (let i = 0; i < s.length; i++) {
    while (set.has(s[i])) {
      set.delete(s[start])
      start++
    }

    set.add(s[i])
    maxLen = Math.max(maxLen, i - start + 1)
  }

  return maxLen
}
console.log(lengthOfLongestSubstring('abcabcabcabc'))
````

```js
function str(text, pattern) {
  for (let i = 0; i < text.length - pattern.length; i++) {
    if (text.substring(i, i + pattern.length) === pattern) {
      return i
    }
  }
  return -1
}

console.log(str('hellow', 'll'))
```

<!-- important  problem -->

```js
function isValid(s) {
  let stack = []
  let map = {
    ')': '(',
    '}': '{',
    ']': '[',
  }

  for (let char of s) {
    if (char in map) {
      if (stack.pop() !== map[char]) {
        return false
      }
    } else {
      stack.push(char)
    }
  }

  return stack.length === 0
}
```

### Imported Notes: `DSA JS/src/data-structures/strings/practice.md`

🟢 LEVEL 1: Basics (Foundation – MUST)

Valid Palindrome

Reverse String

Reverse Words in a String

Implement strStr()

Length of Last Word

Valid Anagram

First Unique Character in a String

Isomorphic Strings

Check If Two String Arrays are Equivalent

Longest Common Prefix

🟡 LEVEL 2: Frequency / Hashing

(Google loves map-based logic)

Group Anagrams

Find All Anagrams in a String

Ransom Note

Word Pattern

Sort Characters By Frequency

Minimum Number of Steps to Make Two Strings Anagram

Check if All Characters Have Equal Number of Occurrences

🟡 LEVEL 3: Two Pointers

(VERY important 🔥)

Valid Palindrome II

Longest Palindromic Substring

Palindrome Partitioning

Merge Strings Alternately

Remove Palindromic Subsequences

Compare Version Numbers

🟠 LEVEL 4: Sliding Window

(Google favorite pattern 🚀)

Longest Substring Without Repeating Characters

Longest Repeating Character Replacement

Minimum Window Substring 🔥🔥

Permutation in String

Substring with Concatenation of All Words

Maximum Number of Vowels in a Substring of Given Length

🟠 LEVEL 5: Stack-Based Strings

(Used in parsers, compilers)

Valid Parentheses

Remove All Adjacent Duplicates in String

Remove All Adjacent Duplicates in String II

Decode String

Simplify Path

🔴 LEVEL 6: Advanced / Google Core

(These separate Google from others)

Edit Distance 🔥

Regular Expression Matching 🔥🔥

Wildcard Matching

Longest Happy Prefix

Shortest Palindrome

Reorganize String

🔴 LEVEL 7: String + DP / Greedy

(VERY Google-style)

Longest Common Subsequence

Distinct Subsequences

Interleaving String

Palindrome Partitioning II

Count and Say
<!-- DSA-JS-MERGE:END -->

---

**Previous:** [Arrays - The Foundation of All Data Structures](../Phase-1-Foundations/03-Arrays-Complete-Mastery.md) | **Next:** [Recursion - The Foundation of All Advanced Algorithms](../Phase-1-Foundations/05-Recursion-Complete-Mastery.md)
