# Category C — Data Structure Practice (Java)

This repository contains solutions based on the supplied 14-page Category C practice PDF.

## Part A — Coding problems
Ten standalone Java programs are in `src/`:
1. Vowel and Consonant Counter
2. Word Reverser and Palindrome Checker
3. Even and Odd Numbers in a List
4. In-Place Array Reversal
5. Digit Sum and Number Reversal
6. Prime Number Checker
7. Factorial Calculation
8. Student Grade Assignment
9. Leap Year Detector
10. Student Result Card Generator

## Compile and run
Install a JDK, open a terminal in this repository, and compile the program you want. Example:

```bash
javac src/Problem01VowelConsonantCounter.java
java -cp src Problem01VowelConsonantCounter
```

Each program is standalone and uses standard input. For Problem 3 and Problem 4, enter `n` first, followed by `n` integers. For Problem 10, enter each student as `name mark1 mark2 mark3` on its own line; enter EOF to finish.

## Part B and Part C
- `PartB_MCQ_Answers.md`: answer key with brief explanations.
- `PartC_Concept_Answers.md`: concise answers to the ten concept questions.

## Complexity notes
The programs use standard loop-based solutions. In-place reversal takes `O(n)` time and `O(1)` auxiliary space. Prime checking takes `O(sqrt(n))` time. The remaining complexities depend on the input size; the code comments/README can be expanded if your instructor requires per-question complexity statements.

## Important
The source PDF's Problem 10 allows grades other than B and D to be designed by the student. This solution uses C for averages 60–74 and F below 40.
