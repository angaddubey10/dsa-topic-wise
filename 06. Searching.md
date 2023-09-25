### List of Questions
1. Searching an element in a sorted array
2. Left Index
3. Peak element
4. Count 1's in binary array
5. Floor in a Sorted Array
6. Search an Element in an array



____


## Details of Questions Listed Above


<details>
<summary>
Searching an element in a sorted array
</Summary>

### **Searching an element in a sorted array**
**Difficulty Level : Basic** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 

Given an array arr[] sorted in ascending order of size N and an integer K. Check if K is present in the array or not.


#### **Example 1:**

    Input:
    N = 5, K = 6
    arr[] = {1,2,3,4,6}
    Output: 1
    Exlpanation: Since, 6 is present in 
    the array at index 4 (0-based indexing),
    output is 1.
    

#### **Example 2:**

    Input:
    N = 5, K = 2
    arr[] = {1,3,4,5,6}
    Output: -1
    Exlpanation: Since, 2 is not present 
    in the array, output is -1.
 

#### **Your Task:**
You don't need to read input or print anything. Complete the function searchInSorted() which takes the sorted array arr[], its size N and the element K as input parameters and returns 1 if K is present in the array, else it returns -1. 


**Expected Time Complexity:** O(Log N)

**Expected Auxiliary Space:** O(1)

 

**Constraints:**

1 <= N <= 106
1 <= K <= 106
1 <= arr[i] <= 106


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    ##Complete this function
    def searchInSorted(self,arr, N, K):
        #Your code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

import math
if __name__ == '__main__': 
    t = int(input())
    for _ in range(t):
        NK = input().strip().split()
        N = int(NK[0])
        K = int(NK[1])
        A = [ int(x) for x in input().strip().split() ]
        ob=Solution()
        print(ob.searchInSorted(A,N,K))

# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Left Index
</Summary>

### **Left Index**
**Difficulty Level : Easy** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 

Given a sorted array of integers of size N and a number X. Find the leftmost index of X in the array arr[].

#### **Example 1:**

    Input:
    N = 10
    arr[] = {1, 1, 2, 2, 3, 4, 5, 5, 6, 7}
    X = 1
    Output: 0 
    Explanation: Because the element 1   
    appears twice and its left most 
    occurrence is at index 0.

#### **Example 2:**

    Input:
    N = 5
    arr[] = {2, 2, 3, 3, 4}
    X = 4
    Output: 4
    Explanation: Because element 4 appears 
    only once at index 4.

#### **Your Task:**
You don't need to read input or print anything. Your task is to complete the function leftIndex() which takes the array arr[], its size N and an integer X as input parameters and returns the leftmost occurrence of X in arr[]. If X is not present in the array, return -1.

**Expected Time Complexity:** O(LogN)

**Expected Auxiliary Space:** O(1)

**Constraints:**

1 <= N <= 106
-105 <= arr[i] <= 105
Array may contain duplicate elements. 


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    def leftIndex (self, N, arr, X):
        # code here 
        
        


#{ 
 # Driver Code Starts
#Initial Template for Python 3

if __name__ == '__main__': 
    t = int (input ())
    for _ in range (t):
        N = int(input())
        arr = input().split()
        for itr in range(N):
            arr[itr] = int(arr[itr])
        X = int(input())

        ob = Solution()
        print(ob.leftIndex(N, arr, X))

# } Driver Code Ends
```

</details>


</details>


<details>
<summary>
Peak element
</Summary>

### **Peak element**
**Difficulty Level : Easy** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 

An element is called a peak element if its value is not smaller than the value of its adjacent elements(if they exists).
Given an array arr[] of size N, Return the index of any one of its peak elements.
Note: The generated output will always be 1 if the index that you return is correct. Otherwise output will be 0. 


#### **Example 1:**

    Input: 
    N = 3
    arr[] = {1,2,3}
    Possible Answer: 2
    Generated Output: 1
    Explanation: index 2 is 3.
    It is the peak element as it is 
    greater than its neighbour 2.
    If 2 is returned then the generated output will be 1 else 0.
#### **Example 2:**

    Input:
    N = 3
    arr[] = {3,4,2}
    Possible Answer: 1
    Output: 1
    Explanation: 4 (at index 1) is the 
    peak element as it is greater than 
    it's neighbor elements 3 and 2.
    If 1 is returned then the generated output will be 1 else 0.
 

#### **Your Task:**
You don't have to read input or print anything. Complete the function peakElement() which takes the array arr[] and its size N as input parameters and return the index of any one of its peak elements.

Can you solve the problem in expected time complexity?

 

**Expected Time Complexity:** O(log N)

**Expected Auxiliary Space:**O(1)


**Constraints:**

1 ≤ N ≤ 105
1 ≤ A[] ≤ 106



#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
# your task is to complete this function
# function should return index to the any valid peak element
class Solution:   
    def peakElement(self,arr, n):
        # Code here



#{ 
 # Driver Code Starts
if __name__=='__main__':
    t = int(input())
    for i in range(t):
        n = int(input())
        arr = list(map(int, input().strip().split()))
        index = Solution().peakElement(arr.copy(), n)
        flag = False
        if index<0 or index>=n:
            flag = False
        else:
            if index == 0 and n==1:
                flag = True
            elif index==0 and arr[index]>=arr[index+1]:
                flag = True
            elif index==n-1 and arr[index]>=arr[index-1]:
                flag = True
            elif arr[index-1] <= arr[index] and arr[index] >= arr[index+1]:
                flag = True
            else:
                flag = False

        if flag:
            print(1)
        else:
            print(0)
# Contributed by: Harshit Sidhwa

# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Count 1's in binary array
</Summary>

### **Count 1's in binary array**
**Difficulty Level : Easy** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 

Given a binary sorted non-increasing array of 1s and 0s. You need to print the count of 1s in the binary array.

#### **Example 1:**

    Input:
    N = 8
    arr[] = {1,1,1,1,1,0,0,0}
    Output: 5
    Explanation: Number of 1's in given 
    binary array : 1 1 1 1 1 0 0 0 is 5.
#### **Example 2:**

    Input:
    N = 8
    arr[] = {1,1,0,0,0,0,0,0}
    Output: 2
    Explanation: Number of 1's in given 
    binary array : 1 1 0 0 0 0 0 0 is 2.
#### **Your Task:**
The task is to complete the function countOne() which takes the array arr[] and its size N as inputs and returns the count of 1s in the input array.

**Expected Time Complexity:** O(LogN).

**Expected Auxiliary Space:**O(1).

**Constraint:**

1 <= N <= 5*106
arr[i] = 0,1




#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    ##Complete this code
    def countOnes(self,arr, N):
        #Your code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

import math


def main():
        T=int(input())
        while(T>0):
            
            N=int(input())

            A=[int(x) for x in input().strip().split()]
            
            
            ob=Solution()
            print(ob.countOnes(A,N))
            
            T-=1


if __name__ == "__main__":
    main()
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Floor in a Sorted Array
</Summary>

### **Floor in a Sorted Array**
**Difficulty Level : Easy** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 

Given a sorted array arr[] of size N without duplicates, and given a value x. Floor of x is defined as the largest element K in arr[] such that K is smaller than or equal to x. Find the index of K(0-based indexing).

#### **Example 1:**

    Input:
    N = 7, x = 0 
    arr[] = {1,2,8,10,11,12,19}
    Output: -1
    Explanation: No element less 
    than 0 is found. So output 
    is "-1".
#### **Example 2:**

    Input:
    N = 7, x = 5 
    arr[] = {1,2,8,10,11,12,19}
    Output: 1
    Explanation: Largest Number less than 5 is
    2 (i.e K = 2), whose index is 1(0-based 
    indexing).
#### **Your Task:**
The task is to complete the function findFloor() which returns an integer denoting the index value of K or return -1 if there isn't any such number.

**Expected Time Complexity:**O(log N).

**Expected Auxiliary Space:** O(1).

**Constraints:**

1 ≤ N ≤ 107
1 ≤ arr[i] ≤ 1018
0 ≤ X ≤ arr[n-1]


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
class Solution:
    #User function Template for python3
    
    #Complete this function
    def findFloor(self,A,N,X):
        #Your code here
        


#{ 
 # Driver Code Starts
#Initial Template for Python 3


import math


def main():
        T=int(input())
        while(T>0):
            
            NX=[int(x) for x in input().strip().split()]
            N=NX[0]
            X=NX[1]

            A=[int(x) for x in input().strip().split()]
            
            obj = Solution()
            print(obj.findFloor(A,N,X))
            
            T-=1


if __name__ == "__main__":
    main()
# } Driver Code Ends
```

</details>


</details>


<details>
<summary>
Search an Element in an array
</Summary>

### **Search an Element in an array**
**Difficulty Level : Basic** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 

Given an integer array and another integer element. The task is to find if the given element is present in array or not.

#### **Example 1:**

    Input:
    n = 4
    arr[] = {1,2,3,4}
    x = 3
    Output: 2
    Explanation: There is one test case 
    with array as {1, 2, 3 4} and element 
    to be searched as 3.  Since 3 is 
    present at index 2, output is 2.
#### **Example 2:**

    Input:
    n = 5
    arr[] = {1,2,3,4,5}
    x = 5
    Output: 4
    Explanation: For array elements 
    {1,2,3,4,5} element to be searched 
    is 5 and it is at index 4. So, the 
    output is 4.
#### **Your Task:**
The task is to complete the function search() which takes the array arr[], its size N and the element X as inputs and returns the index of first occurrence of X in the given array. If the element X does not exist in the array, the function should return -1.

**Expected Time Complexity:**O(n).

**Expected Auxiliary Space:**O(1). 

**Constraints:**

1 <= n <= 106
0 <= arr[i] <= 106
0 <= x <= 105


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    #Complete the below function
    def search(self,arr, N, X):
        #Your code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3


import math



    
def main():
        T=int(input())
        while(T>0):
            
            N=int(input())
            
            A=[int(x) for x in input().strip().split()]
            
            x=int(input())
            ob=Solution()
            print(ob.search(A,N,x))
            
            T-=1


if __name__ == "__main__":
    main()
# } Driver Code Ends
```

</details>


</details>