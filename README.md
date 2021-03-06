# searchsort package
A Python Package that contains almost all the Searching and Sorting Algorithms

It is also available in [PyPI](https://pypi.org/project/searchsort/)

## Installation in Python
***Note \: Requires Python Version 3.x***
```bash
pip install searchsort
```

## A Searching Implementation
```python3
from random import shuffle
import searchsort as ss

L1 = [i for i in range(1, 51)]
element = 20

# Shuffling the List
shuffle(L1)

index = ss.BinarySearch(L1, element)

if index:
  print(f"{element} found at :", index)
else:
  print(f"{element} not found")
```
**Note \:-**
- **Some of the Algorithms require a sorted array. It is mentioned in the docstring of the functions so read them carefully.**
- **All the Algorithms return the index of the First Occurence of the element.**
- **If Element is Not Present, False is Returned.**

## A Sorting Implementation
```python3
from random import shuffle
import searchsort as ss

L1 = [i for i in range(1, 51)]

# Shuffling the List
shuffle(L1)
print("List Before Sorting :", L1)

Result = ss.BubbleSort(L1)
print("List After Sorting :", Result)
```
**Note \:-**
- **Some of the Algorithms perform an in-place sorting, which means the structure of the Original List will be changed.**
- **All the Algorithms return the sorted array, so assigning statements are preferred.**

**Besides Searching an Element in an Array and Sorting Arrays, the Package also contains an 'IsSorted' Function that Returns True if an Array is _SORTED_ in either direction; False If NOT.**
## IsSorted Function Implementation
```python3
from random import shuffle
from searchsort import IsSorted

L1 = [i for i in range(1, 51)]
print("Is the List Sorted Now? ", IsSorted(L1))

# Shuffling the List
shuffle(L1)

print("Is the List Sorted Now? ", IsSorted(L1))
```
