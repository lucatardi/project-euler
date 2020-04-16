Even Fibonacci Numbers
Problem

    If we list all the natural numbers below 10 that are multiples of 3 or 5, we get 3, 5, 6 and 9. The sum of these multiples is 23. Find the sum of all the multiples of 3 or 5 below the provided parameter value number.

Algorithm

    create an array with "number" elements.
    filter this array for numbers divisible by 3 or 5.
    sum all the elements in the array.
    return this sum.

Code

function multiplesOf3and5(number) {
  return [...Array(number).keys()]
    .filter(num => num % 3 === 0 || num % 5 === 0)
    .reduce((sum, num) => sum + num)
}

Notes

    When I started to code I realize I could reduce the array instead of doing the sum and return it, so I changed on the flight my algorithm (bad practice).
