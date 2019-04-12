# implement List.indexOf

`while`-style and recursive implementations at the top of
OrderedList_inArraySlots.java

[Java API on the `indexOf` method](https://docs.oracle.com/javase/10/docs/api/java/util/List.html#indexOf(java.lang.Object))

based on [solutionsHolmes/5D_genericTypes/OrderedList_inArraySlots_v2/](https://github.com/stuyvesant-cs/solutionsHolmes/tree/master/5D_genericTypes/OrderedList_inArraySlots_v2)
as of 2019-04-10 04:48

# 0. state the problem
Find the index of a given number in an ordered arrayList.

# 1. recursive abstraction
When I'm asked to find the index of a given number in an ordered arrayList, the recursive abstraction can find the index of a given number in half of the original arrayList.

# 2. identify
a. decision of whether to go to b. or c.
	if (low > hi)
b. solution to the base case
	return -1;
c. solutions to the recursive case
	1) combine (N/A)
	2) recursive abstraction
		indexOf_recursive( findMe, low, pageToCheck - 1);
		indexOf_recursive( findMe, pageToCheck + 1, hi);
	3) leftover (N/A)