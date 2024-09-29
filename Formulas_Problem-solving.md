# Common O(1) Mathematical Formulas for Algorithmic Problems

| **Formula**                     | **What It Solves**                           | **Example**                                          |
|----------------------------------|----------------------------------------------|------------------------------------------------------|
| `n * (n + 1) // 2`               | Sum of first `n` natural numbers             | For `1, 2, 3, 4, 5`: <br> `sum = 5 * (5 + 1) // 2` <br> `sum = 15` |
| `n * (n - 1) // 2`               | Number of ways to choose 2 from `n` elements | For `n = 4` elements: <br> `combinations = 4 * (4 - 1) // 2` <br> `combinations = 6` |
| `(n * (n + 1) * (2n + 1)) // 6`  | Sum of squares of first `n` natural numbers  | For `1, 2, 3`: <br> `sum of squares = (3 * (3 + 1) * (2*3 + 1)) // 6` <br> `sum of squares = 14` |
| `a * b // gcd(a, b)`             | Least common multiple (LCM) of `a` and `b`   | For `a = 6, b = 8`: <br> `LCM = 6 * 8 // gcd(6, 8)` <br> `LCM = 24` |
| `log_b(n)`                       | Logarithm of `n` with base `b`               | For `n = 8, b = 2`: <br> `log_2(8) = 3` |
| `x ^ (x - 1) // x`               | Number of permutations of `x` elements       | For `x = 3`: <br> `permutations = 3! = 3 * 2 * 1` <br> `permutations = 6` |
| `2^n - 1`                        | Total subsets of a set with `n` elements     | For `n = 3`: <br> `subsets = 2^3 - 1` <br> `subsets = 7` |
| `n // d`                         | Number of divisors of `n`                    | For `n = 10, d = 2`: <br> `divisors = 10 // 2` <br> `divisors = 5` |
| `a * (b - 1) // b`               | Sum of geometric series                      | For `a = 5, b = 3`: <br> `sum = 5 * (3 - 1) // 3` <br> `sum = 3` |
| `fib(n) = (Φ^n - (1 - Φ)^n) / √5`| nth Fibonacci number                         | For `n = 5`: <br> `fib(5) = 5` |
