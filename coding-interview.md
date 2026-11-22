# The Apple Coding Interview

Coding appears twice at Apple: once in the technical phone screen and again inside the onsite loop. Each session is commonly reported to last 45 to 60 minutes, and many teams run one to three sessions in the loop. The questions are mostly of medium difficulty, and the interviewer grades the quality of the code as closely as its correctness.

## Format

| Item | Commonly reported |
|---|---|
| Phone screen | 45 to 60 minutes of live coding |
| Editor | CoderPad, a shared browser editor |
| Language | Usually your own choice |
| Sessions in the loop | 1 to 3, each 45 to 60 minutes |
| Difficulty | Mostly medium; unusual algorithms are rare |
| Follow-up | The interviewer changes one constraint and asks you to adapt |

Not every team asks algorithm questions. Some teams ask practical problems from their own work, and others spend the time on language and platform depth. Ask your recruiter which kind of round your team runs.

## What is graded

The interviewer is reported to read your code the way a teammate reads a code review. A code review is the check that one engineer makes on another engineer's change before it is merged.

- **Correctness.** The code runs and handles the empty input and the boundary cases.
- **Readability.** Variables and functions have real names, and the structure is simple.
- **Memory use.** You can state how much memory the solution needs and why.
- **Reasoning.** You state the plan first, write the simple version, and then improve it.
- **Adaptation.** You adjust the solution when a constraint changes, without starting again.

## Topics commonly reported

| Topic | Pattern to practice | Lesson |
|---|---|---|
| Arrays and strings | Sliding window, which moves a fixed or variable range across the input | [Introduction to Sliding Window Pattern](https://www.designgurus.io/course-play/grokking-the-coding-interview/doc/introduction-to-sliding-window-pattern?utm_source=github&utm_medium=repo&utm_campaign=apple-interview-guide&utm_content=coding-interview) |
| Sorted arrays and pairs | Two pointers, which moves two indexes toward each other | [Introduction to Two Pointers Pattern](https://www.designgurus.io/course-play/grokking-the-coding-interview/doc/introduction-to-two-pointers-pattern?utm_source=github&utm_medium=repo&utm_campaign=apple-interview-guide&utm_content=coding-interview) |
| Hash maps | Counting and lookup in constant time | [Introduction to Hash Map Pattern](https://www.designgurus.io/course-play/grokking-the-coding-interview/doc/introduction-to-hash-map-pattern?utm_source=github&utm_medium=repo&utm_campaign=apple-interview-guide&utm_content=coding-interview) |
| Trees | Level-order and depth-first traversal | [Introduction to Tree Depth First Search Pattern](https://www.designgurus.io/course-play/grokking-the-coding-interview/doc/introduction-to-tree-depth-first-search-pattern?utm_source=github&utm_medium=repo&utm_campaign=apple-interview-guide&utm_content=coding-interview) |
| Heaps | Top K elements | [Introduction to Top 'K' Elements Pattern](https://www.designgurus.io/course-play/grokking-the-coding-interview/doc/introduction-to-top-k-elements-pattern?utm_source=github&utm_medium=repo&utm_campaign=apple-interview-guide&utm_content=coding-interview) |
| Binary search | Search in sorted or rotated data | [Introduction to Modified Binary Search Pattern](https://www.designgurus.io/course-play/grokking-the-coding-interview/doc/introduction-to-modified-binary-search-pattern?utm_source=github&utm_medium=repo&utm_campaign=apple-interview-guide&utm_content=coding-interview) |

Linked lists, sorting, graphs, recursion, and simple dynamic programming are also reported. Three problems that candidates name are merging overlapping intervals, detecting a cycle in a linked list, and building an LRU cache. An LRU cache is a cache that removes the least recently used item when it is full.

## Questions tied to the team

Teams also ask about their own work. The reported examples are specific.

- A systems team may ask about concurrency, which is the correct handling of work that runs on several threads at once.
- A client team may ask you to write plain JavaScript.
- One reported question asks for a thread-safe LRU cache with constant-time reads and writes.
- Another asks you to implement a hash map and then explain how it grows.

## How to practice

1. Practice by pattern and not by problem count. Six patterns cover most reported questions.
2. Write every solution as if a teammate will merge it. Use real names and handle the empty input.
3. Say your test cases aloud before you run the code.
4. After each problem, change one constraint yourself and solve it again.

The [Question bank](question-bank.md) lists 32 coding questions with a lesson for each. The [Four-week plan](four-week-plan.md) places them in a schedule.

## Go deeper

- [Grokking the Coding Interview](https://www.designgurus.io/course/grokking-the-coding-interview?utm_source=github&utm_medium=repo&utm_campaign=apple-interview-guide&utm_content=coding-interview) groups coding problems by pattern, which matches how these rounds are built.
- [Grokking 75: Top Coding Interview Questions](https://www.designgurus.io/course/grokking-75-top-coding-interview-questions?utm_source=github&utm_medium=repo&utm_campaign=apple-interview-guide&utm_content=coding-interview) is a shorter list for the final two weeks.
- Lesson: [DSA Patterns Cheat Sheet](https://www.designgurus.io/course-play/grokking-the-coding-interview/doc/coding-patterns-a-cheat-sheet?utm_source=github&utm_medium=repo&utm_campaign=apple-interview-guide&utm_content=coding-interview), in Grokking the Coding Interview
- Lesson: [Introduction to Multi-threaded Pattern](https://www.designgurus.io/course-play/grokking-the-coding-interview/doc/introduction-to-multithreaded-pattern?utm_source=github&utm_medium=repo&utm_campaign=apple-interview-guide&utm_content=coding-interview), in Grokking the Coding Interview
- Free answer: [Does Apple ask LeetCode questions in interviews?](https://www.designgurus.io/answers/detail/does-apple-ask-leetcode-questions-in-interviews?utm_source=github&utm_medium=repo&utm_campaign=apple-interview-guide&utm_content=coding-interview)
- Sibling free guide: [Grokking the Coding Interview patterns on GitHub](https://github.com/design-gurus/grokking-coding-interview)
