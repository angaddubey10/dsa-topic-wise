### list of Queestions 
1. Bubble Sort
2. Insertion Sort
3. Count Inversions
4. Quick Sort
5. Binary Array Sorting



-----


<details>
<summary>
Bubble Sort
</Summary>

### **Bubble Sort**
**Difficulty Level : Easy** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 

Given an Integer N and a list arr. Sort the array using bubble sort algorithm.
#### **Example 1:**

    Input: 
    N = 5
    arr[] = {4, 1, 3, 9, 7}
    Output: 
    1 3 4 7 9
#### **Example 2:**

    Input:
    N = 10 
    arr[] = {10, 9, 8, 7, 6, 5, 4, 3, 2, 1}
    Output: 
    1 2 3 4 5 6 7 8 9 10

#### **Your Task:**
You don't have to read input or print anything. Your task is to complete the function bubblesort() which takes the array and it's size as input and sorts the array using bubble sort algorithm.

**Expected Time Complexity:** O(N^2).

**Expected Auxiliary Space:** O(1).

**Constraints:**

1 <= N <= 103
1 <= arr[i] <= 103


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    #Function to sort the array using bubble sort algorithm.
    def bubbleSort(self,arr, n):
        # code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3



if __name__=='__main__':
    t = int(input())
    for i in range(t):
        n = int(input())
        arr = list(map(int, input().strip().split()))
        ob = Solution()
        ob.bubbleSort(arr, n)
        for i in arr:
            print(i,end=' ')
        print()

# } Driver Code Ends
```

</details>


</details>


<details>
<summary>
Insertion Sort
</Summary>

### **Insertion Sort**
**Difficulty Level : Easy** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 

The task is to complete the insert() function which is used to implement Insertion Sort.


#### **Example 1:**

    Input:
    N = 5
    arr[] = { 4, 1, 3, 9, 7}
    Output:
    1 3 4 7 9
#### **Example 2:**

    Input:
    N = 10
    arr[] = {10, 9, 8, 7, 6, 5, 4, 3, 2, 1}
    Output:
    1 2 3 4 5 6 7 8 9 10

#### **Your Task:**
You don't have to read input or print anything. Your task is to complete the function insert() and insertionSort() where insert() takes the array, it's size and an index i and insertionSort() uses insert function to sort the array in ascending order using insertion sort algorithm. 

**Expected Time Complexity:** O(N*N).

**Expected Auxiliary Space:** O(1).


**Constraints:**

1 <= N <= 1000
1 <= arr[i] <= 1000


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#Sort the array using insertion sort

class Solution:
    def insert(self, alist, index, n):
        #code here
        
    #Function to sort the list using insertion sort algorithm.    
    def insertionSort(self, alist, n):
        #code here


#{ 
 # Driver Code Starts
if __name__=="__main__":
    t=int(input())
    for i in range(t):
        n=int(input())
        arr=list(map(int,input().split()))
    
        Solution().insertionSort(arr,n)
    
        for i in range(n):
            print(arr[i],end=" ")
    
        print()
# } Driver Code Ends
```

</details>


</details>


<details>
<summary>
Count Inversions
</Summary>

### **Count Inversions**
**Difficulty Level : Medium** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 

Given an array of integers. Find the Inversion Count in the array. 

Inversion Count: For an array, inversion count indicates how far (or close) the array is from being sorted. If array is already sorted then the inversion count is 0. If an array is sorted in the reverse order then the inversion count is the maximum. 
Formally, two elements a[i] and a[j] form an inversion if a[i] > a[j] and i < j.
 

#### **Example 1:**

    Input: N = 5, arr[] = {2, 4, 1, 3, 5}
    Output: 3
    Explanation: The sequence 2, 4, 1, 3, 5 
    has three inversions (2, 1), (4, 1), (4, 3).
#### **Example 2:**

    Input: N = 5
    arr[] = {2, 3, 4, 5, 6}
    Output: 0
    Explanation: As the sequence is already 
    sorted so there is no inversion count.
#### **Example 3:**

    Input: N = 3, arr[] = {10, 10, 10}
    Output: 0
    Explanation: As all the elements of array 
    are same, so there is no inversion count.
#### **YOUR TASK**
You don't need to read input or print anything. Your task is to complete the function inversionCount() which takes the array arr[] and the size of the array as inputs and returns the inversion count of the given array.

**Expected Time Complexity:** O(NLogN).

**Expected Auxiliary Space:** O(N).

**Constraints:**

1 ≤ N ≤ 5*105
1 ≤ arr[i] ≤ 1018


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
class Solution:
    #User function Template for python3
    
    # arr[]: Input Array
    # N : Size of the Array arr[]
    #Function to count inversions in the array.
    def inversionCount(self, arr, n):
        # Your Code Here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

import atexit
import io
import sys

_INPUT_LINES = sys.stdin.read().splitlines()
input = iter(_INPUT_LINES).__next__
_OUTPUT_BUFFER = io.StringIO()
sys.stdout = _OUTPUT_BUFFER

@atexit.register

def write():
    sys.__stdout__.write(_OUTPUT_BUFFER.getvalue())

if __name__=='__main__':
    t = int(input())
    for tt in range(t):
        n = int(input())
        a = list(map(int, input().strip().split()))
        obj = Solution()
        print(obj.inversionCount(a,n))
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Quick Sort
</Summary>

### **Quick Sort**
**Difficulty Level : Medium** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 

Quick Sort is a Divide and Conquer algorithm. It picks an element as a pivot and partitions the given array around the picked pivot.
Given an array arr[], its starting position is low (the index of the array) and its ending position is high(the index of the array).

Note: The low and high are inclusive.

Implement the partition() and quickSort() functions to sort the array.


#### **Example 1:**

Input: 
    N = 5 
    arr[] = { 4, 1, 3, 9, 7}
    Output:
    1 3 4 7 9
#### **Example 2:**

    Input: 
    N = 9
    arr[] = { 2, 1, 6, 10, 4, 1, 3, 9, 7}
    Output:
    1 1 2 3 4 6 7 9 10

#### **Your Task:**
You don't need to read input or print anything. Your task is to complete the functions partition()  and quickSort() which takes the array arr[], low and high as input parameters and partitions the array. Consider the last element as the pivot such that all the elements less than(or equal to) the pivot lie before it and the elements greater than it lie after the pivot.


**Expected Time Complexity:** O(N*logN)

**Expected Auxiliary Space:**O(logN)


**Constraints:**

1 <= N <= 103
1 <= arr[i] <= 104


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    #Function to sort a list using quick sort algorithm.
    def quickSort(self,arr,low,high):
        # code here
    
    def partition(self,arr,low,high):
        # code here
    


#{ 
 # Driver Code Starts
#Initial Template for Python 3

if __name__ == "__main__":
    t=int(input())
    for i in range(t):
        n=int(input())
        arr=list(map(int,input().split()))
        Solution().quickSort(arr,0,n-1)
        for i in range(n):
            print(arr[i],end=" ")
        print()

# } Driver Code Ends
```

</details>


</details>


<details>
<summary>
Binary Array Sorting
</Summary>

### **Binary Array Sorting**
**Difficulty Level : Basic**

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 

Given a binary array A[] of size N. The task is to arrange the array in increasing order.
Note: The binary array contains only 0  and 1.
 

#### **Example 1:**

    Input: 
    5
    1 0 1 1 0

    Output: 
    0 0 1 1 1

    Explanation: 
    After arranging the elements in 
    increasing order, elements will be as 
    0 0 1 1 1.
#### **Example 2:**

    Input:
    10
    1 0 1 1 1 1 1 0 0 0

    Output: 
    0 0 0 0 1 1 1 1 1 1

    Explanation: 
    After arranging the elements in 
    increasing order, elements will be 
    0 0 0 0 1 1 1 1 1 1.

#### **Your Task:** 
This is a function problem. You only need to complete the function binSort() that takes the array A[] and it's size N as parameters and sorts the array. The printing is done automatically by the driver code.

**Expected Time Complexity:** O(N)

**Expected Auxilliary Space:**O(1)

**Constraints:**

1 <= N <= 106
0 <= A[i] <= 1


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    
    #Function to sort the binary array.
    def binSort(self, A, N): 
        #Your code here
        #No need to print the array
    


#{ 
 # Driver Code Starts
#Initial Template for Python 3

import math


def main():
        T=int(input())
        while(T>0):
            N=int(input())
            A=list(map(int,input().split()))
            obj = Solution()
            obj.binSort(A,N)
            
            for i in A:
                print(i,end=" ")
            print()
            
            T-=1


if __name__ == "__main__":
    main()
# } Driver Code Ends
```

</details>


</details>
