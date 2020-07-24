#### Please add your answers to the **_Analysis of Algorithms_** exercises here.

## Exercise I

a)

O(n)

At first glance I assumed the time complexity would be o(n)^3 but after evaluating the inner statement it becomes obvious that we are
incrementing each iteration by n^2 so the answer has to be n^3 - n^2

b)

O(nlog(n))

The initial for loop obviously has a run time complexity of O(n). the inner loop advances in multiples of 2 which makes me believe
the runtime complexity is log(n)

c)

O(n) or O(bunnies)

there is only one recursion in this function that takes an argument of bunnies decremented by 1. How ever many bunnies you add
as an argument to bunnyEars it will only ever recursed decremented by 1 every time .

## Exercise II

The first thing that comes to mind when evaluating this problem is a binary search. We have a list of floor numbers assuming it starts at 0 to however high the building is - [0, 1, 2, 3, 4, .....] We know that if an egg is dropped at a lower level then our
floor f it will not be broken and if it is dropped above f then it will be broken.

```
pseudocode:
    1. divide total floor numbers // 2 to find the mid point
    2. drop an egg from that floor:
        a. if the egg breaks than that floor becomes the new max value and the search begins again with the lower half
        b. if the egg does not break then the new min value becomes that floor and the search begins with the upper half
        c. enter a base case where if the egg does not break and we are at the last value then we have found f.
    3 return f


the runtime complexity of binary search algorithms is O(log(n))

```
