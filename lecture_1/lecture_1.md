# lecture_1

URL: https://youtu.be/ZA-tUyM_y7s?list=PLUl4u3cNGP63EdVPNLG3ToM6LaEUuStEY

Goals:

- Solve Computational Problems
- Prove correctness
- Argue Efficiency
- Communicating Solution to others

### What is a computational problem?

- In terms of computational problems: suppose there are some Inputs and Outputs defined by a binary relation. The problem could be stated as or thought of in terms of whether an output is correct for a specified input defined by the relation

### What is Algorithm?

- An algorithm is a function that maps a correct output to an input f :I->O
  - Example Birthday Problem
  - Interview students in some order
  - Check if birthday in record
    - if so return pair
  - add new student to the record
  - return none

### Correctness?

- how do we argue that our algorithm is correct?
- Induction:
- we need a base case, and
- Inductive hypothesis:

  - If first k students contain match
  - Algo returns a match before interviewing student k + 1
  - Base Case: k = 0

- Assume the Inductive Hypothesis true for k = k'
  - if k' contain match -> already returned by Induction
  - else if k'+ 1 contain match the algorithm checks against all possibilities.

### Efficiency?

- By efficiency we mean not only how fast an algorithm runs but also compare with other possible ways
- We don't measure time, instead count fundamental operations (OPS)
- expect performance to depend on size of input
- Big (O) and Omega (Ω) and Theta (ϴ) notations
- example O(1), O(n), O(n^2), O(n^c)(polynomial), 2^n (Exponential = bad)

- MODEL of COMPUTATION
- Word RAM
- Operations:(constant amount of time)
- Integer Arithmetic
- logical ops
- bitwise ops
