### List of Questions
1. Check if array is sorted and rotated
2. Maximum Index
3. Stock buy and sell
4. Trapping Rain Water
5. Kadane's Algorithm
6. Longest Subarray Of Evens And Odds
7. Max Circular Subarray Sum
8. Rearrange an array with O(1) extra space
9. Game of Chocolates
10. Smallest Positive missing number
11. Divide and Subtract Game


______

 ## Details of Questions Listed Above

<details>
<summary>
Check if array is sorted and rotated
</Summary>

### **Check if array is sorted and rotated**
**Difficulty Level : Medium** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 
Given an array arr[] of N distinct integers, check if this array is Sorted (non-increasing or non-decreasing) and Rotated counter-clockwise. Note that input array may be sorted in either increasing or decreasing order, then rotated.
A sorted array is not considered as sorted and rotated, i.e., there should be at least one rotation.

#### *Example 1:**
    
    Input:
    N = 4
    arr[] = {3,4,1,2}
    Output: Yes
    Explanation: The array is sorted 
    (1, 2, 3, 4) and rotated twice 
    (3, 4, 1, 2).
#### **Example 2:**

    Input:
    N = 3
    arr[] = {1,2,3}
    Output: No
    Explanation: The array is sorted 
    (1, 2, 3) is not rotated.
#### **Your Task:**
The task is to complete the function checkRotatedAndSorted() which returns true if an array is sorted and rotated clockwise otherwise false.

**Expected Time Complexity:** O(N).

**Expected Auxiliary Space:** O(1).

**Constraints:**

1 <= N <= 106
1 <= A[i] <= 106


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    ##Complete this function
    #Function to check if array is sorted and rotated.
    def checkRotatedAndSorted(self,arr,n):
        #code here    


#{ 
 # Driver Code Starts
import atexit

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

if __name__ == '__main__':
    test_cases = int(input())
    for cases in range(test_cases) :
        n = int(input())
        a = list(map(int,input().strip().split()))
        ob=Solution()
        if ob.checkRotatedAndSorted(a,n) or ob.checkRotatedAndSorted(a[::-1],n):
            print("Yes")
        else:
            print("No")

# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Maximum Index
</Summary>

### **Maximum Index**
**Difficulty Level : Medium** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 
Given an array A[] of N positive integers. The task is to find the maximum of j - i subjected to the constraint of A[i] < A[j] and i < j.
 

#### **Example 1:**

    Input:
    N = 2
    A[] = {1, 10}
    Output:
    1
    Explanation:
    A[0]<A[1] so (j-i) is 1-0 = 1.
#### **Example 2:**

    Input:
    N = 9
    A[] = {34, 8, 10, 3, 2, 80, 30, 33, 1}
    Output:
    6
    Explanation:
    In the given array A[1] < A[7]
    satisfying the required 
    condition(A[i] < A[j]) thus giving 
    the maximum difference of j - i 
    which is 6(7-1).
 

#### **Your Task:**
The task is to complete the function maxIndexDiff() which finds and returns maximum index difference. Printing the output will be handled by driver code. Return 0 in case no such index is found.

**Expected Time Complexity:** O(N)

**Expected Auxiliary Space:** O(N)

**Constraints:**

1 ≤ N ≤ 107
0 ≤ A[i] ≤ 109


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    #Complete this function
    # Function to find the maximum index difference.
    def maxIndexDiff(self,A, N): 
        ##Your code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

import math

def main():
        T=int(input())
        while(T>0):
            
            n=int(input())
            
            arr=[int(x) for x in input().strip().split()]
            ob=Solution()
            print(ob.maxIndexDiff(arr,n))
            
            
            T-=1


if __name__ == "__main__":
    main()
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Stock buy and sell
</Summary>

#### **Stock buy and sell**
**Difficulty Level : Easy** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 
The cost of stock on each day is given in an array A[] of size N. Find all the segments of days on which you buy and sell the stock so that in between those days for which profit can be generated.
Note: Since there can be multiple solutions, the driver code will print 1 if your answer is correct, otherwise, it will return 0. In case there's no profit the driver code will print the string "No Profit" for a correct solution.

#### **Example 1:**

    Input:
    N = 7
    A[] = {100,180,260,310,40,535,695}
    Output:
    1
    Explanation:
    One possible solution is (0 3) (4 6)
    We can buy stock on day 0,
    and sell it on 3rd day, which will 
    give us maximum profit. Now, we buy 
    stock on day 4 and sell it on day 6.
#### **Example 2:**

    Input:
    N = 5
    A[] = {4,2,2,2,4}
    Output:
    1
    Explanation:
    There are multiple possible solutions.
    one of them is (3 4)
    We can buy stock on day 3,
    and sell it on 4th day, which will 
    give us maximum profit.

#### **Your Task:**
The task is to complete the function stockBuySell() which takes an array of A[] and N as input parameters and finds the days of buying and selling stock. The function must return a 2D list of integers containing all the buy-sell pairs i.e. the first value of the pair will represent the day on which you buy the stock and the second value represent the day on which you sell that stock. If there is No Profit, return an empty list.


**Expected Time Complexity:** O(N)

**Expected Auxiliary Space:** O(N)


**Constraints:**

2 ≤ N ≤ 106
0 ≤ A[i] ≤ 106


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function template for Python

class Solution:
    #Function to find the days of buying and selling stock for max profit.
	def stockBuySell(self, A, n):
		#code here


#{ 
 # Driver Code Starts
#Initial template for Python

def check(ans,A,p):
    c = 0
    for i in range(len(ans)):
        c += A[ans[i][1]]-A[ans[i][0]]
    if(c==p):
        return 1 
    else:
        return 0

if __name__=='__main__':
	t = int(input())
	while(t>0):
		n = int(input())
		A = [int(x) for x in input().strip().split()]
		ob = Solution()
		ans = ob.stockBuySell(A,n)
		p=0
		for i in range(n-1):
		    p += max(0,A[i+1]-A[i])
		if(len(ans) == 0):
			print("No Profit",end="")
		else:
			print(check(ans,A,p),end="")
		print()
		t-=1
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Trapping Rain Water
</Summary>

### **Trapping Rain Water**
**Difficulty Level : Medium** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 
Given an array arr[] of N non-negative integers representing the height of blocks. If width of each block is 1, compute how much water can be trapped between the blocks during the rainy season. 
 

#### **Example 1:**

    Input:
    N = 6
    arr[] = {3,0,0,2,0,4}
    Output:
    10
    Explanation: 

#### **Example 2:**

    Input:
    N = 4
    arr[] = {7,4,0,9}
    Output:
    10
    Explanation:
    Water trapped by above 
    block of height 4 is 3 units and above 
    block of height 0 is 7 units. So, the 
    total unit of water trapped is 10 units.
#### **Example 3:**

    Input:
    N = 3
    arr[] = {6,9,9}
    Output:
    0
    Explanation:
    No water will be trapped.

#### **Your Task:**
You don't need to read input or print anything. The task is to complete the function trappingWater() which takes arr[] and N as input parameters and returns the total amount of water that can be trapped.


**Expected Time Complexity:** O(N)

**Expected Auxiliary Space:** O(N)


**Constraints:**

3 < N < 106
0 < Ai < 108


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python

class Solution:
    def trappingWater(self, arr,n):
        #Code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

import math



def main():
        T=int(input())
        while(T>0):
            
            n=int(input())
            
            arr=[int(x) for x in input().strip().split()]
            obj = Solution()
            print(obj.trappingWater(arr,n))
            
            
            T-=1


if __name__ == "__main__":
    main()



# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Kadane's Algorithm
</Summary>

### **Kadane's Algorithm**
**Difficulty Level : Medium** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 
Given an array Arr[] of N integers. Find the contiguous sub-array(containing at least one number) which has the maximum sum and return its sum.


#### **Example 1:**

    Input:
    N = 5
    Arr[] = {1,2,3,-2,5}
    Output:
    9
    Explanation:
    Max subarray sum is 9
    of elements (1, 2, 3, -2, 5) which 
    is a contiguous subarray.
#### **Example 2:**

    Input:
    N = 4
    Arr[] = {-1,-2,-3,-4}
    Output:
    -1
    Explanation:
    Max subarray sum is -1 
    of element (-1)

#### **Your Task:**
You don't need to read input or print anything. The task is to complete the function maxSubarraySum() which takes Arr[] and N as input parameters and returns the sum of subarray with maximum sum.


**Expected Time Complexity:** O(N)

**Expected Auxiliary Space:** O(1)


**Constraints:**

1 ≤ N ≤ 106
-107 ≤ A[i] ≤ 107


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    ##Complete this function
    #Function to find the sum of contiguous subarray with maximum sum.
    def maxSubArraySum(self,arr,N):
        ##Your code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

import math

 
def main():
        T=int(input())
        while(T>0):
            
            n=int(input())
            
            arr=[int(x) for x in input().strip().split()]
            
            ob=Solution()
            
            print(ob.maxSubArraySum(arr,n))
            
            T-=1


if __name__ == "__main__":
    main()
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Longest Subarray Of Evens And Odds
</Summary>

### **Longest Subarray Of Evens And Odds**
**Difficulty Level : Medium** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 
You are given an array of size n. Find the maximum possible length of a subarray such that its elements are arranged alternately either as even and odd or odd and even .

#### **Example 1:**
    
    Input:
    n = 5
    a[] = {10,12,14,7,8}
    Output: 3
    Explanation: The max length of subarray
    is 3 and the subarray is {14 7 8}. Here 
    the array starts as an even element and 
    has odd and even elements alternately.
#### **Example 2:**

    Input:
    n = 2
    a[] = {4,6}
    Output: 1
    Explanation: The array contains {4 6}. 
    So, we can only choose 1 element as 
    that will be the max length subarray.
#### **Your Task:**
 You don't need to take any input. Just complete the function maxEvenOdd() that returns the maximum length.

**Expected Time Complexity:** O(N).

**Expected Auxiliary Space:** O(1).

**Constraints:**

1 <= n <= 106
1 <= Ai <= 103


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    #Function to find the length of longest subarray of even and odd numbers.
    def maxEvenOdd(self,arr,n):
        
        #returns: the maximum length
        
        #code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

#contributed by RavinderSinghPB
if __name__=='__main__':
    t=int(input())
    for i in range(t):
        n=int(input())
        arr = list(map(int,input().strip().split()))
        ob=Solution()
        print(ob.maxEvenOdd(arr,n))
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Max Circular Subarray Sum
</Summary>

### **Max Circular Subarray Sum**
**Difficulty Level : Hard** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 
Given an array arr[] of N integers arranged in a circular fashion. Your task is to find the maximum contiguous subarray sum.


#### **Example 1:**

    Input:
    N = 7
    arr[] = {8,-8,9,-9,10,-11,12}
    Output:
    22
    Explanation:
    Starting from the last element
    of the array, i.e, 12, and 
    moving in a circular fashion, we 
    have max subarray as 12, 8, -8, 9, 
    -9, 10, which gives maximum sum 
    as 22.
#### **Example 2:**
    
    Input:
    N = 8
    arr[] = {10,-3,-4,7,6,5,-4,-1}
    Output:
    23
    Explanation: Sum of the circular 
    subarray with maximum sum is 23

#### **Your Task:**
The task is to complete the function circularSubarraySum() which returns a sum of the circular subarray with maximum sum.


**Expected Time Complexity:** O(N).

**Expected Auxiliary Space:** O(1).


**Constraints:**

1 <= N <= 106
-106 <= Arr[i] <= 106


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

#Complete this function
#Function to find maximum circular subarray sum.
def circularSubarraySum(arr,n):
    ##Your code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3


import math
import sys

    
    

if __name__ == "__main__":
    T=int(input())
    while(T>0):
            
        n=int(input())
        
        arr=[int(x) for x in input().strip().split()]
            
        print(circularSubarraySum(arr,n))
        
        T-=1
    
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Rearrange an array with O(1) extra space
</Summary>

### **Rearrange an array with O(1) extra space**
**Difficulty Level : Medium** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 
Given an array arr[] of size N where every element is in the range from 0 to n-1. Rearrange the given array so that the transformed array arrT[i] becomes arr[arr[i]].

NOTE: arr and arrT are both same variables, representing the array before and after transformation respectively.

#### **Example 1:**

    Input:
    N = 2
    arr[] = {1,0}
    Output: 0 1
    Explanation: 
    arr[arr[0]] = arr[1] = 0
    arr[arr[1]] = arr[0] = 1
    So, arrT becomes {0, 1}
#### **Example 2:**
    
    Input:
    N = 5
    arr[] = {4,0,2,1,3}
    Output: 3 4 2 0 1
    Explanation: 
    arr[arr[0]] = arr[4] = 3
    arr[arr[1]] = arr[0] = 4
    arr[arr[2]] = arr[2] = 2
    arr[arr[3]] = arr[1] = 0
    arr[arr[4]] = arr[3] = 1
    and so on
    So, arrT becomes {3, 4, 2, 0, 1}
#### **Your Task:**
You don't need to read input or print anything. The task is to complete the function arrange() which takes arr and N as input parameters and rearranges the elements in the array in-place. 

**Expected Time Complexity:** O(N)

**Expected Auxiliary Space:** O(1)

**Constraints:**

1 <= N <= 105
0 <= Arr[i] < N


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

##Complete this code

class Solution:
    #Function to rearrange an array so that arr[i] becomes arr[arr[i]]
    #with O(1) extra space.
    def arrange(self,arr, n): 
        #Your code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3


import math



def main():
        T=int(input())
        while(T>0):
            
            n=int(input())
            
            arr=[int(x) for x in input().strip().split()]
            
            ob=Solution()
            ob.arrange(arr,n)
            
            for i in arr:
                print(i,end=" ")
            
            print()
            
            T-=1


if __name__ == "__main__":
    main()
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Game of Chocolates
</Summary>

### **Game of Chocolates**
**Difficulty Level : Medium** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 
Bunty and Dolly are playing a game, described as follows.
Game Description: -
There are two boxes having A and B number of chocolates respectively. Both can eat L (L ≥ 1) chocolates from any one box or L chocolates from both the boxes in one move. They play the game alternatively and the last one to eat the chocolate will be the winner.
As Bunty wants to impress Dolly, he wants to make Dolly the winner. You have to help Bunty in deciding who should play first. Assume that both the players play optimally.

#### **Example 1:**
    
    Input:
    A = 1 and B = 2
    Output: Bunty
    Explanation:
    If Bunty starts first, all the next possible state
    (0,2), (1,1), (1,0) are wining state for Dolly
#### **Example 2:**
    
    Input:
    A = 1 and B = 3
    Output: Dolly
#### **Your Task:**  
You don't need to read input or print anything. Your task is to complete the function game() which takes the integer A and B as input parameters and returns false if Bunty should play first else returns true.

**Expected Time Complexity:** O(1)

**Expected Auxiliary Space:** O(1)

**Constraints:**

0 ≤ a, b ≤ 106


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3


class Solution:
    def game (self, A, B):
        # code here
        pass



#{ 
 # Driver Code Starts
#Initial Template for Python 3





if __name__ == '__main__': 
    ob = Solution()
    t = int (input ())
    for _ in range (t):
        N, K = map(int, input().split())
        ans = ob.game(N, K);
        if(ans):
            print("Dolly")
        else:
            print("Bunty")


# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Smallest Positive missing number
</Summary>

### **Smallest Positive missing number**
**Difficulty Level : Medium** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 
You are given an array arr[] of N integers including 0. The task is to find the smallest positive number missing from the array.

#### **Example 1:**

    Input:
    N = 5
    arr[] = {1,2,3,4,5}
    Output: 6
    Explanation: Smallest positive missing 
    number is 6.
#### **Example 2:**

    Input:
    N = 5
    arr[] = {0,-10,1,3,-20}
    Output: 2
    Explanation: Smallest positive missing 
    number is 2.
#### **Your Task:**
The task is to complete the function missingNumber() which returns the smallest positive missing number in the array.

**Expected Time Complexity:** O(N).

**Expected Auxiliary Space:** O(1).

**Constraints:**

1 <= N <= 106
-106 <= arr[i] <= 106


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    
    #Function to find the smallest positive number missing from the array.
    def missingNumber(self,arr,n):
        #Your code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3


import math


def main():
        T=int(input())
        while(T>0):
            
            n=int(input())
            
            arr=[int(x) for x in input().strip().split()]
            
            ob=Solution()
            print(ob.missingNumber(arr,n))
            
            T-=1


if __name__ == "__main__":
    main()
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Divide and Subtract Game
</Summary>


### **Divide and Subtract Game**
**Difficulty Level : Medium** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 
Jon and Arya are playing a game. Rules of game as follows:
  They have a single number N initially.
   Both will play an alternate move. Jon starts first.
   Both will play each move optimally.
   In each move, they can perform only one of these operation
          1. Divide that number by 2, 3, 4 or 5 and take floor of result.
          2. Subtract that number by 2, 3, 4 or 5.
   If after making a move the number becomes 1, the player who made the move automatically loses the game.
   When number becomes zero, the game will stop and the player who can't make a move loses the game.

 

#### **Example 1:**

    Input:
    N = 3
    Output:
    Jon
    Explanation:
    Jon will just subtract 3 from initial
    number and win the game.
#### **Example 2:**
    
    Input:
    N = 6
    Output:
    Arya
    Explanation:
    Jon will divide by 3 and then in next step
    Arya will subtract by 2 and win the game.
 

#### **Your Task:**
You don't need to read input or print anything. Your task is to complete the function divAndSub() which takes an Integer N as input and returns a string denoting who won the game.

 

**Expected Time Complexity:** O(N)

**Expected Auxiliary Space:** O(N)

 

**Constraints:**

1 <= N <= 105

#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    def divAndSub(self, N):
        # code here 


#{ 
 # Driver Code Starts
#Initial Template for Python 3

if __name__ == '__main__': 
    t = int (input ())
    for _ in range (t):
        N=int(input())
        
        ob = Solution()
        print(ob.divAndSub(N))
# } Driver Code Ends
```

</details>


</details>



