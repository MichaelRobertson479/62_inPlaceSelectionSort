# in-place selection sort

Rearrange
an unordered `ArrayList<Integer>`
and use it as the data in an `OrderedList_inArraySlots`.

The re-use is probably contrary to Java's conventions
for its built-in classes. But as a pedagogical tool,
it has the advantage of allowing
the User program to check that the sort
is done in-place.

## count the cost

0. If the number of the elements in the input triples,
the time required to run the reigning champ algorithm
will grow by three times. Has to run through each element
when doing the comparisons to find the smallest.
[Justify, in about 2 sentences.]

0. If the number of the elements in the input triples,
the number of times that the reigning champ algorithm
will be invoked will grow by three times. When sorting the
unordered data, you need to find the smallest element from
index 0 to size()-1, then from 1 to size()-1, and so on.
Therefore, the champ algorithm is invoked size() times.
[Justify, in about 2 sentences.]

0. If the number of the elements in the input triples,
the time required for the selection sort
will grow by roughly 9 times. For an list of size n,
time is n + (n-1) + ... + 1, since you invoke the champ algorithm
n times and each time you're dealing with a smaller number of elements.
This is the same as 1 + 2 ... + n, which is (n^2 + n)/2. For size 3n,
it would be 3n + (3n-1) + ... + 1, or (9n^2 + 3n)/2,
which for large values of n is approximately 9 times greater.
[Justify, in about 2 sentences.]
