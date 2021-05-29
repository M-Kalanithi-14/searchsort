# searchsort
A Python Package that contains almost all the Searching and Sorting Algorithms

It is available in [PyPI](https://pypi.org/project/searchsort/)

## Searching Implementation
```python
from random import shuffle
import searchsort as ss

L1 = [i for i in range(1, 51)]

# Shuffling the List
shuffle(L1)
print("List Before Sorting", L1)

Result = ss.BubbleSort(L1)
print("List After Sorting :", Result)
```
**Note \:-**
- **Some of the Algorithms perform an in-place sorting, which means the structure of the Original List will be changed.**
- **All the Algorithms return the sorted array, so assigning statements are preferred.**
