Problem 2
===
##### Make it Flat

Assume ruby does not have a `flatten` method and you need to flatten an Array. Write a function that would take a nested array and return a single flattened sorted array. To make this more interesting, **do not** use any of the inbuild collection method (merge, concat etc.)

**Input**   
[1, 2, 3, [4, 6, [7, 8]], 5, 9, 10]

**output**   
1, 2, 3, 4, 5, 6, 7, 8, 9, 10

**Example**

```
def make_flat(array)
  # write your code here
end

puts make_flat([1, 2, 3, [4, 6, [7, 8]], 5, 9, 10])

# output : 1, 2, 3, 4, 5, 6, 7, 8, 9, 10

```
