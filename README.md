# implement List.indexOf

`while`-style and recursive implementations at the top of
OrderedList_inArraySlots.java

[Java API on the `indexOf` method](https://docs.oracle.com/javase/10/docs/api/java/util/List.html#indexOf(java.lang.Object))

based on [solutionsHolmes/5D_genericTypes/OrderedList_inArraySlots_v2/](https://github.com/stuyvesant-cs/solutionsHolmes/tree/master/5D_genericTypes/OrderedList_inArraySlots_v2)
as of 2019-04-10 04:48

#### hw60#2
![logarithm](https://latex.codecogs.com/gif.latex?%24%24y%20%3D%20log_2%20x%24%24) means that y is the power that 2 has to be raised to in order to obtain x. The logarithmic statement is equivalent to ![exponential](https://latex.codecogs.com/gif.latex?%24%24%20x%20%3D%202%5Ey%20%24%24).

#### hw60#3
- Problem: Find a specified element in an ordered list.
- RA (Recursive Abstraction): When I am asked to find a specified element in an ordered list, the recursive abstraction can find the specified element in the proper half of the ordered list.

- Decision: Is the sub-list of size 0?
  - Yes (Base Case): Return -1, the element is not in the list
- Decision: Does the element at the current index match the desired element?
  - Yes (Base Case): Return the current index.
  - No (Recursive Case):
    (Leftover Processing) If the specified element is before the middle element of the list, (RA) find the specified element in the first half of the list using these instructions.
    Else, (RA) find the specified element in the latter half of the list using these instructions.
