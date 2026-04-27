# Part 1 Answers

## Q1

Line 9 prints `values added: 20` because `add` is true, so the code runs inside the `if` block and adds `10 + 10`.

## Q2

Line 13 prints `final result: 20` because `result` uses `var`, so it can still be used outside the `if` block.

## Q3

We should not use `var` because it can be confusing. A variable made with `var` inside a block can still be used outside that block, so it is easier to make mistakes. `let` and `const` are safer and clearer.

## Q4

Line 9 prints `values added: 20` because `result` is created with `let` inside the `if` block and then changed to `20`.

## Q5

Line 13 gives an error because `result` was made with `let` inside the `if` block, so it only exists inside that block.

## Q6

Line 9 gives an error because `result` is made with `const`, but the code tries to change its value. `const` cannot be reassigned.

## Q7

Line 13 does not print anything because the program already stops from the `const` error before it gets there.
