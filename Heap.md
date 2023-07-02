### List of Questions
1. Binary Heap Operations
2. Heap Sort


_____

## Details of Questions Listed Above

<details>
<summary>
Binary Heap Operations
</Summary>

### **Binary Heap Operations**
**Difficulty Level : Medium** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 
A binary heap is a Binary Tree with the following properties:
1) Its a complete tree (All levels are completely filled except possibly the last level and the last level has all keys as left as possible). This property of Binary Heap makes them suitable to be stored in an array.

2) A Binary Heap is either Min Heap or Max Heap. In a Min Binary Heap, the key at the root must be minimum among all keys present in Binary Heap. The same property must be recursively true for all nodes in Binary Tree. Max Binary Heap is similar to MinHeap.

You are given an empty Binary Min Heap and some queries and your task is to implement the three methods insertKey,  deleteKey,  and extractMin on the Binary Min Heap and call them as per the query given below:
1) 1  x  (a query of this type means to insert an element in the min-heap with value x )
2) 2  x  (a query of this type means to remove an element at position x from the min-heap)
3) 3  (a query like this removes the min element from the min-heap and prints it ).

#### **Example 1:**
    
    Input:
    Q = 7
    Queries:
    insertKey(4)
    insertKey(2)
    extractMin()
    insertKey(6)
    deleteKey(0)
    extractMin()
    extractMin()
    Output: 2 6 - 1
    Explanation: In the first test case for
    query 
    insertKey(4) the heap will have  {4}  
    insertKey(2) the heap will be {2 4}
    extractMin() removes min element from 
                 heap ie 2 and prints it
                 now heap is {4} 
    insertKey(6) inserts 6 to heap now heap
                 is {4 6}
    deleteKey(0) delete element at position 0
                 of the heap,now heap is {6}
    extractMin() remove min element from heap
                 ie 6 and prints it  now the
                 heap is empty
    extractMin() since the heap is empty thus
                 no min element exist so -1
                 is printed.
#### **Example 2:**

    Input:
    Q = 5
    Queries:
    insertKey(8)
    insertKey(9)
    deleteKey(1)
    extractMin()
    extractMin()
    Output: 8 -1
#### **Your Task:**
You are required to complete the 3 methods insertKey() which take one argument the value to be inserted, deleteKey() which takes one argument the position from where the element is to be deleted and extractMin() which returns the minimum element in the heap(-1 if the heap is empty)

**Expected Time Complexity:** O(Q*Log(size of Heap) ).

**Expected Auxiliary Space:** O(1).

**Constraints:**

1 <= Q <= 104
1 <= x <= 104


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

'''
heap = [0 for i in range(101)]  # our heap to be used
'''
#Function to insert a value in Heap.
def insertKey (x):
    global curr_size

#Function to delete a key at ith index.
def deleteKey (i):
    global curr_size

#Function to extract minimum value in heap and then to store 
#next minimum value at first index.
def extractMin ():



#{ 
 # Driver Code Starts
#Initial Template for Python 3

import atexit
import io
import sys

# Contributed by : Nagendra Jha

_INPUT_LINES = sys.stdin.read().splitlines()
input = iter(_INPUT_LINES).__next__
_OUTPUT_BUFFER = io.StringIO()
sys.stdout = _OUTPUT_BUFFER

@atexit.register

def write():
    sys.__stdout__.write(_OUTPUT_BUFFER.getvalue())

heap = []  # our heap to be used
curr_size = 0  # current size of heap

if __name__ == '__main__':
    test_cases = int(input())
    for cases in range(test_cases):
        n = int(input())
        a = list(map(int, input().strip().split()))
        # initialize every globals
        curr_size = 0
        heap = [0 for i in range(n)]
        i = 0
        while i < len(a):
            if a[i] == 1:
                insertKey(a[i + 1])
                i += 1
            elif a[i] == 2:
                deleteKey(a[i + 1])
                i += 1
            else:
                print(extractMin (), end=" ")
            i += 1
        # reinitialize every globals
        # curr_size = 0
        # heap = [0 for i in range(101)]
        print()
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Heap Sort
</Summary>

### **Heap Sort**
**Difficulty Level : Medium** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 
Given an array of size N. The task is to sort the array elements by completing functions heapify() and buildHeap() which are used to implement Heap Sort.


#### **Example 1:**

    Input:
    N = 5
    arr[] = {4,1,3,9,7}
    Output:
    1 3 4 7 9
    Explanation:
    After sorting elements
    using heap sort, elements will be
    in order as 1,3,4,7,9.
#### **Example 2:**

    Input:
    N = 10
    arr[] = {10,9,8,7,6,5,4,3,2,1}
    Output:
    1 2 3 4 5 6 7 8 9 10
    Explanation:
    After sorting elements
    using heap sort, elements will be
    in order as 1, 2,3,4,5,6,7,8,9,10.

#### **Your Task :**
You don't have to read input or print anything. Your task is to complete the functions heapify(), buildheap() and heapSort() where heapSort() and buildheap() takes the array and it's size as input and heapify() takes the array, it's size and an index i as input. Complete and use these functions to sort the array using heap sort algorithm.
Note: You don't have to return the sorted list. You need to sort the array "arr" in place.


**Expected Time Complexity:** O(N * Log(N)).

**Expected Auxiliary Space:** O(1).


**Constraints:**

1 ≤ N ≤ 106
1 ≤ arr[i] ≤ 106


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    #Heapify function to maintain heap property.
    def heapify(self,arr, n, i):
        # code here
    
    #Function to build a Heap from array.
    def buildHeap(self,arr,n):
        # code here
    
    #Function to sort an array using Heap Sort.    
    def HeapSort(self, arr, n):
        #code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3
import atexit
import io
import sys

# Contributed by : Mohit Kumara

_INPUT_LINES = sys.stdin.read().splitlines()
input = iter(_INPUT_LINES).__next__
_OUTPUT_BUFFER = io.StringIO()
sys.stdout = _OUTPUT_BUFFER

@atexit.register

def write():
    sys.__stdout__.write(_OUTPUT_BUFFER.getvalue())

if __name__ == '__main__':
    test_cases = int(input())
    for cases in range(test_cases):
        n = int(input())
        arr = list(map(int, input().strip().split()))
        Solution().HeapSort(arr,n)
        print(*arr)

# } Driver Code Ends
```

</details>


</details>