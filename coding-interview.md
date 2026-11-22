# Microsoft Coding Interview

Coding is the largest part of the Microsoft process. Candidates commonly report one coding screen and then two or three coding interviews inside the loop. Each live interview is usually one well-scoped problem at medium difficulty in about an hour.

## The three formats

| Format | Who gets it | Reported shape |
|---|---|---|
| Online assessment (OA) | Students, interns, and new graduates | 2 or 3 problems in 60 to 90 minutes, graded by hidden test cases |
| Technical phone screen | Experienced candidates | 45 to 60 minutes of live coding on a shared editor or Microsoft Teams |
| Loop coding interview | Everyone who reaches the loop | 1 problem in about 60 minutes, with questions about past work at the start |

You can usually choose the language, and the commonly reported options are C++, C#, Java, Python, and JavaScript.

## What is graded

The OA and the live interview reward different skills.

| Skill | Online assessment | Live interview |
|---|---|---|
| Correct output on hidden tests | Decides the score | Expected |
| Efficiency | A solution that times out scores like a wrong one | You state time and space cost aloud |
| Edge cases | Empty input, one element, duplicates, very large values | You raise them before you write |
| Explanation | No credit | Graded throughout |
| Testing | You write your own cases before submitting | You trace a small example at the end |

In a live interview, interviewers are reported to grade more than the final answer. Ask about input size and invalid input before you write, then explain the plan and say when you change it. Write code that would compile, with clear variable names.

## Topics commonly reported

- **Most frequent:** arrays, strings, and hash maps.
- **Next:** linked lists, trees, sorting, and graph traversal.
- **Also reported:** recursion, backtracking, and dynamic programming.

Heavy dynamic programming is reported to be less common in the OA than at some other companies. A typical loop question asks for the values of a binary tree that are visible from the right side. That problem is taught in the lesson [Right View of a Binary Tree](https://www.designgurus.io/course-play/grokking-the-coding-interview/doc/problem-challenge-2-right-view-of-a-binary-tree-easy?utm_source=github&utm_medium=repo&utm_campaign=microsoft-interview-guide&utm_content=coding-interview).

## Patterns worth learning first

A pattern is a reusable approach that solves many problems of the same shape. The table links each pattern to a problem from the Microsoft course or the pattern course.

| Pattern | Example problem | Lesson |
|---|---|---|
| Hash map counting | Find Original Array From Doubled Array | [Problem](https://www.designgurus.io/course-play/grokking-microsoft-coding-interview/doc/find-original-array-from-doubled-array-medium?utm_source=github&utm_medium=repo&utm_campaign=microsoft-interview-guide&utm_content=coding-interview) |
| Two pointers | Reverse Words in a String II | [Problem](https://www.designgurus.io/course-play/grokking-microsoft-coding-interview/doc/reverse-words-in-a-string-ii-medium?utm_source=github&utm_medium=repo&utm_campaign=microsoft-interview-guide&utm_content=coding-interview) |
| Backtracking | Restore IP Addresses | [Problem](https://www.designgurus.io/course-play/grokking-microsoft-coding-interview/doc/restore-ip-addresses-medium?utm_source=github&utm_medium=repo&utm_campaign=microsoft-interview-guide&utm_content=coding-interview) |
| Monotonic stack | Largest Rectangle in Histogram | [Problem](https://www.designgurus.io/course-play/grokking-microsoft-coding-interview/doc/largest-rectangle-in-histogram-hard?utm_source=github&utm_medium=repo&utm_campaign=microsoft-interview-guide&utm_content=coding-interview) |
| Dynamic programming | Longest Arithmetic Subsequence | [Problem](https://www.designgurus.io/course-play/grokking-microsoft-coding-interview/doc/longest-arithmetic-subsequence-medium?utm_source=github&utm_medium=repo&utm_campaign=microsoft-interview-guide&utm_content=coding-interview) |
| Tree breadth-first search | Right View of a Binary Tree | [Pattern introduction](https://www.designgurus.io/course-play/grokking-the-coding-interview/doc/introduction-to-tree-breadth-first-search-pattern?utm_source=github&utm_medium=repo&utm_campaign=microsoft-interview-guide&utm_content=coding-interview) |
| Grid traversal | Number of Islands | [Problem](https://www.designgurus.io/course-play/grokking-the-coding-interview/doc/number-of-islands-easy?utm_source=github&utm_medium=repo&utm_campaign=microsoft-interview-guide&utm_content=coding-interview) |

## How to practice

1. Study patterns, not question counts. Medium questions repeat a small number of shapes.
2. Use a timer and a plain editor. Allow 30 minutes per problem at first, then 20.
3. Write four test cases before each submission: empty input, one element, duplicates, and the largest allowed value.
4. Say your plan aloud for every problem, including the time and space cost.
5. Keep an error log. Record each failed problem and the reason, and review the log in the final week.

The [question bank](question-bank.md) lists 25 coding problems in order of difficulty.

## Go deeper

- [Grokking Microsoft Coding Interview](https://www.designgurus.io/course/grokking-microsoft-coding-interview?utm_source=github&utm_medium=repo&utm_campaign=microsoft-interview-guide&utm_content=coding-interview): 12 problems reported in Microsoft interviews, from easy to hard.
- Lesson: [Sliding Window Maximum](https://www.designgurus.io/course-play/grokking-microsoft-coding-interview/doc/sliding-window-maximum-hard?utm_source=github&utm_medium=repo&utm_campaign=microsoft-interview-guide&utm_content=coding-interview), in Grokking Microsoft Coding Interview
- Lesson: [Introduction to Monotonic Stack](https://www.designgurus.io/course-play/grokking-the-coding-interview/doc/introduction-to-monotonic-stack?utm_source=github&utm_medium=repo&utm_campaign=microsoft-interview-guide&utm_content=coding-interview), in Grokking the Coding Interview
- Free article: [Top 20 coding questions to pass the Microsoft interview](https://www.designgurus.io/blog/top-20-coding-questions-to-pass-microsoft-interview?utm_source=github&utm_medium=repo&utm_campaign=microsoft-interview-guide&utm_content=coding-interview)
- Free answer: [What is the Microsoft online assessment?](https://www.designgurus.io/answers/detail/what-is-microsoft-online-assessment?utm_source=github&utm_medium=repo&utm_campaign=microsoft-interview-guide&utm_content=coding-interview)
- Free guide: [Grokking Coding Interview](https://github.com/design-gurus/grokking-coding-interview) on GitHub
