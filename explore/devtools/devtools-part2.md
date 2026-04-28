# DevTools Part 2

## Q1

The bug was that the input values were strings instead of numbers. When I typed `2` and `3`, the code joined them together and showed `23` instead of adding them to get `5`.

## Q2

I would fix it by converting the input values to numbers before adding them. I changed the calculation to use `Number(num1) + Number(num2)`.
