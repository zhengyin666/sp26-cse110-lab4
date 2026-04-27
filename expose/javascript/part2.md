# Part 2 Answers

## Q1
Line 12 will print `3`. Since `i` is declared with `var`, it is function-scoped, not block-scoped. After the loop finishes, `i` becomes `3`, so it can still be accessed outside the loop.

## Q2
Line 13 will print `150`. `discountedPrice` is declared with `var`, so it is still available after the loop. The last price is `300`, and with a `0.5` discount, the last discounted price is `150`.

## Q3
Line 14 will print `150`. `finalPrice` is declared before the loop with `var`, so it can be used after the loop. It keeps getting updated each time, and the last value is `150`.

## Q4
The function will return `[50, 100, 150]`. Each price gets multiplied by `1 - 0.5`, so the prices become half of the original values. Those final prices are pushed into the `discounted` array and returned.

## Q5
Line 12 will cause an error because `i` is declared with `let` inside the `for` loop. `let` is block-scoped, so `i` only exists inside the loop and cannot be used after the loop ends.

## Q6
Line 13 will cause an error because `discountedPrice` is declared with `let` inside the loop. That means it only exists inside the loop block, so the code cannot access it outside the loop.

## Q7
Line 14 will print `150`. `finalPrice` is declared with `let` near the top of the function, not inside the loop, so it is still available after the loop. Its last updated value is `150`.

## Q8
The function will return `[50, 100, 150]`. There is no error because the code does not try to access `i` or `discountedPrice` outside their loop scope. The array is updated during the loop and then returned.

## Q9
Line 11 will cause an error because `i` was declared with `let` inside the `for` loop. Since `let` is block-scoped, `i` cannot be accessed outside the loop.

## Q10
Line 12 will print `3`. `length` is declared with `const` inside the function, so it can be used anywhere inside the function after it is declared. Since the array has three items, the value is `3`.

## Q11
The function will return `[50, 100, 150]`. `discounted` is a `const` array, but that only means the variable cannot be reassigned. The array itself can still be changed with `.push()`.

## Q12
A. `student.name`

B. `student["Grad Year"]`

C. `student.greeting()`

D. `student["Favorite Teacher"].name`

E. `student.courseLoad[0]`

## Q13
A. `'3' + 2` gives `"32"` because `+` with a string does string concatenation.

B. `'3' - 2` gives `1` because JavaScript converts the string `"3"` into the number `3`.

C. `3 + null` gives `3` because `null` becomes `0`.

D. `'3' + null` gives `"3null"` because JavaScript treats it as string concatenation.

E. `true + 3` gives `4` because `true` becomes `1`.

F. `false + null` gives `0` because `false` becomes `0` and `null` also becomes `0`.

G. `'3' + undefined` gives `"3undefined"` because it becomes string concatenation.

H. `'3' - undefined` gives `NaN` because `undefined` cannot be converted into a useful number.

## Q14
A. `'2' > 1` gives `true` because JavaScript converts `"2"` into the number `2`.

B. `'2' < '12'` gives `false` because both values are strings, so JavaScript compares them alphabetically. Since `"2"` comes after `"1"`, the result is false.

C. `2 == '2'` gives `true` because `==` allows type conversion, so the string `"2"` becomes the number `2`.

D. `2 === '2'` gives `false` because `===` checks both value and type. One is a number and the other is a string.

E. `true == 2` gives `false` because `true` becomes `1`, and `1` is not equal to `2`.

F. `true === Boolean(2)` gives `true` because `Boolean(2)` becomes `true`, so both sides are boolean `true`.

## Q15
The `==` operator checks if two values are equal, but it can convert the types first. The `===` operator checks both the value and the type, so it is stricter. For example, `2 == "2"` is true, but `2 === "2"` is false.

## Q17
The result will be `[2, 4, 6]`. The `modifyArray` function goes through each number in `[1, 2, 3]` and passes each one into the callback function `doSomething`. Since `doSomething` multiplies the number by `2`, the new array becomes `[2, 4, 6]`.

## Q19
The output will be:

```js
1
4
3
2
```
