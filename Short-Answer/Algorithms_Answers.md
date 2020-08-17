#### Please add your answers to the **_Analysis of Algorithms_** exercises here.

## Exercise I

a) Since the while loop will run exactly n times, the runtime will be O(n).

b) The rate of growth is greater than a linear runtime, so as n increases the increase of the operation is significantly lower than a quadratic runtime. This runtime is O(n log n).

c) O(n) will be the runtime for this function because the function will call itself n times. This is generally the case when a recursive function with only one recursice call and no extra looping.

## Exercise II

1. Since the building is already sorted, we can throw the egg of the middle floor. To find the middle floor, add the first and last floor then divide by 2.

2. If the egg does not break, this means that all the floors under the middle, including the middle are not f. This means the starting postion to middle floor + 1 and keep the head of the pointer at the highest. We can then find the middle again and do it all over to make sure everything is truly not f.

3. If the egg does break, we need to keep account of the floor, because it may be the lowest floor that the egg would break on. To be sure the process will be repeated, looking at the middle floor between the first and the floor below the initial middle. Since the egg will break at floor f and above, we have to be sure that the current is the lowest floor the egg will break on.

4. Continue these steps until our left pointer is greater than our right pointer, while keeping track of the lowest floor the egg breaks from along the way.

This is done using a binary search method and has a runtime of O(log n).
