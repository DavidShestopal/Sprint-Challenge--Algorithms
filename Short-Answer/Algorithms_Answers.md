#### Please add your answers to the **_Analysis of Algorithms_** exercises here.

## Exercise I

a) The time complexity of this exercise is O(n), which means number of operations scales linearly. So if n = 3, the while loop will run 3 times.

b) I think it's O(n log n) because when the n is bigger the range of the loop is bigger and more operations can be performed but it is not done in a linearl fashion.

c) The time complexity of this exercise is O(n), which means number of operations scales linearly. The running time increases with the size of the input, so as the n gets bigger the operation will last longer and vice versa.

## Exercise II

For this exercise I would use something like a binary search to solve it. I would use it becuase the function would find the middle of our list and so if we throw off an egg and it cracks we know we are on a higher floor then F so then I get the middle of the new list of everything below the previous middle and try again. If the egg does not break, then I get the middle of the new list of everything above the middle. I would repeat this process until the length of the list becomes one which when that is reached we have found out what the element of F is. The runtime complexity would be O(log n).

while f has not been found:

- Drop the egg

- If the egg breaks:

- Move to a middle point between current location and current lower bound (default ground). Set current floor as the upper bound.

- If the egg does not break:

- Move to the middle point between current location and higher bound (default top floor) Set current floor as the lower bound.

- return floor f
