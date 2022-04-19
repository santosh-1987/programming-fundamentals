## Time Complexity

- Imagine a classroom of 100 students in which you gave your pen to one person. Now, you want that pen. Here are some
  ways to find the pen and what the O order is.
    - O(n2): You go and ask the first person of the class, if he has the pen. Also, you ask this person about other 99
      people in the classroom if they have that pen and so on, This is what we call O(n2).
    - O(n): Going and asking each student individually is O(N).
    - O(log n): Now I divide the class into two groups, then ask: “Is it on the left side, or the right side of the
      classroom?” Then I take that group and divide it into two and ask again, and so on. Repeat the process till you
      are left with one student who has your pen. This is what you mean by O(log n).
    - I might need to do the O(n2) search if only one student knows on which student the pen is hidden. I’d use the O(n)
      if one student had the pen and only they knew it. I’d use the O(log n) search if all the students knew, but would
      only tell me if I guessed the right side.

#### Prerequisite

- Understanding of Logarithms

### Logarithms

Logarithm is the way to represent exponential expression as shown in the example .

- a<sup>y</sup> = x is a exponential expression, it can also be written as log<sub>a</sub> x = y
- 2<sup>5</sup> = 32, can be written as log<sub>2</sub>32 = 5
- log<sub>x</sub> N , It means how many time N should be divided by x to make it 1.

### Arithmetic Progression(AP)

An arithmetic progression (AP) is a sequence where the differences between every two consecutive terms are the same.
![arithmetic_progression_example1](../assets/time_complexity/arithmetic_progression_example1.png)
![ap_brief](../assets/time_complexity/ap_brief.png)

**nth term of an AP:**:

- a<sub>n</sub> = a + (n - 1)d

**Sum of N term in AP**
![ap_formulae](../assets/time_complexity/ap_formulae.png)

### Geometric Progression(AP)

![gp_example](../assets/time_complexity/gp_example.png)
![gp_generic](../assets/time_complexity/gp_generic.png)
![gp_detail](../assets/time_complexity/gp_detail.png)

## Problems

- Problem 1
    - ![problem_1](../assets/time_complexity/problem_1.png)
- Problem 2
    - ![problem_2](../assets/time_complexity/problem_2.png)
- Problem 3
    - ![problem_3](../assets/time_complexity/problem_3.png)
- Problem 4
    - ![problem_4](../assets/time_complexity/problem_4.png)
- Problem 5
    - ![problem_5](../assets/time_complexity/problem_5.png)
- Problem 6
    - ![problem_log_6](../assets/time_complexity/problem_log_6.png)
- Problem 7
    - ![problem_7](../assets/time_complexity/problem_7.png)
- Problem 8
    - ![problem_8](../assets/time_complexity/problem_8.png)
- Problem 9
    - ![problem_9](../assets/time_complexity/problem_9.png)
- **Problem 10**
    - ![problem_10](../assets/time_complexity/problem_10.png)
- **Problem 11**
    - ![problem_11](../assets/time_complexity/problem_11.png)

## How to calculate Big O

![big_o_notation](../assets/time_complexity/big_o_notation.png)
![big_o_examples](../assets/time_complexity/big_o_examples.png)

## Tips & Tricks

- [a,b] -> Including a & b. Number of Terms - `b-a+1`
- (a,b) -> Excluding a & b.
- For Big O Notation
    - Ignore all lower order terms
    - Ignore all constant coefficient terms.
    - Draw Table if you are confused with finding Big T.C