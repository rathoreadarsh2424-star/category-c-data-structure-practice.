# Part B — Quiz Answer Key

1. **D** — `==` compares object references; `equals()` compares String contents.
2. **B** — `StringBuilder` contains `Java Lab`; reversing all characters gives `baL avaJ`.
3. **B** — `Student(String name)` is the matching one-argument constructor.
4. **D** — `w1` and `w2` refer to the same Wallet object, so both see 700.
5. **C** — Three constructor calls increment the shared static count to 3.
6. **A** — The loop visits indices 0 through `scores.length - 1`, printing all values in order.
7. **B** — `continue` skips printing 3, so output is `1 2 4 5`.
8. **A** — Java passes primitive values by value; changing parameter `n` does not change `x`.
9. **C** — `250 / 3.0` is floating-point division, producing approximately `83.33333333333333`.
10. **B** — 2% of 500 is 10, so the output is `Paid 510.0 by card`.
11. **B** — Strings are immutable; `name` remains `"java"` and `upperName` gets `"JAVA"`.
12. **B** — One pooled literal `"hello"` and one separate object created by `new String(...)`: 2 String objects in the usual conceptual count.
13. **A** — `"Campus"` has length 6 and character at index 2 is `m` (indexing starts at 0).
14. **A** — In `"user@domain.com"`, `@` is at index 4.
15. **B** — The default constructor sets title to `Unknown` and price to `0.0`.
16. **A** — The parameterized constructor stores `"Java Programming"` and `450.0`.
17. **B** — `w1` and `w2` share one object; `w3` creates a second object.
18. **C** — Both references see balance 700 because they refer to the same object.
19. **C** — Only `s1`'s object is updated to `"Anu"`; `s2` remains `"Ravi"`.
20. **C** — Three Visitor objects increment the shared static count to 3.
