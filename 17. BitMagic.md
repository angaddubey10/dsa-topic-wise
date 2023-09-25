## List of Questions
1. Find first set bit
2. Rightmost different bit
3. Check whether K-th bit is set or not
4. Count total set bits
5. Bit Difference
6. Longest Consecutive 1's
7. Power of 2
8. Swap all odd and even bits
9. Maximum AND Value
10. Number is sparse or not
11. Binary To Gray Code equivalent
12. Gray to Binary equivalent

______

## Details of Questions Listed Above

<details>
<summary>
Find first set bit
</Summary>

### **Find first set bit**
**Difficulty Level : Easy** 

Sharpen up your programming skills, participate in coding contests & explore high-paying jobs

Given an integer N. The task is to return the position of first set bit found from the right side in the binary representation of the number.
Note: If there is no set bit in the integer N, then return 0 from the function.  

#### **Example 1:**

    Input: N = 18
    Output: 2
    Explanation: Binary representation of 
    18 is 010010,the first set bit from the 
    right side is at position 2.
#### **Example 2:**

    Input: N = 12 
    Output: 3 
    Explanation: Binary representation 
    of  12 is 1100, the first set bit 
    from the right side is at position 3.
#### **Your Task:**
The task is to complete the function getFirstSetBit() that takes an integer n as a parameter and returns the position of first set bit.

**Expected Time Complexity:** O(log N).

**Expected Auxiliary Space:** O(1).

#### **Constraints:**
0 <= N <= 108




#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#{ 
 # Driver Code Starts
#Initial Template for Python 3

import math



# } Driver Code Ends
#User function Template for python3

class Solution:
    
    #Function to find position of first set bit in the given number.
    def getFirstSetBit(self,n):
        #Your code here

#{ 
 # Driver Code Starts.
    
    
def main():
    
    T=int(input())
    
    while(T>0):
        
        
        n=int(input())
        ob=Solution()
        
        print(ob.getFirstSetBit(n))
        
        
        T-=1
    
    




if __name__=="__main__":
    main()
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Rightmost different bit
</Summary>


### **Rightmost different bit**
**Difficulty Level : Easy** 

Sharpen up your programming skills, participate in coding contests & explore high-paying jobs

Given two numbers M and N. The task is to find the position of the rightmost different bit in the binary representation of numbers.

#### **Example 1:** 
    
    Input: M = 11, N = 9
    Output: 2
    Explanation: Binary representation of the given 
    numbers are: 1011 and 1001, 
    2nd bit from right is different.
#### **Example 2:**
    
    Input: M = 52, N = 4
    Output: 5
    Explanation: Binary representation of the given 
    numbers are: 110100 and 0100, 
    5th-bit from right is different.
#### **User Task:**
The task is to complete the function posOfRightMostDiffBit() which takes two arguments m and n and returns the position of first different bits in m and n. If both m and n are the same then return -1 in this case.

**Expected Time Complexity:** O(max(log m, log n)).

**Expected Auxiliary Space:** O(1).

**Constraints:**

0 <= M <= 109
0 <= N <= 109

#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#{ 
 # Driver Code Starts
#Initial Template for Python 3

import math




    
# } Driver Code Ends
#User function Template for python3

class Solution:
    
    #Function to find the first position with different bits.
    def posOfRightMostDiffBit(self,m,n):
        #Your code here

#{ 
 # Driver Code Starts.
    
def main():
    
    T=int(input())
    
    while(T>0):
        
        
        mn=[int(x) for x in input().strip().split()]
        m=mn[0]
        n=mn[1]
        ob=Solution()
        print(math.floor(ob.posOfRightMostDiffBit(m,n)))
        
        
        
        
        T-=1
    
    




if __name__=="__main__":
    main()
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Check whether K-th bit is set or not
</Summary>

### **Check whether K-th bit is set or not**
**Difficulty Level : Easy** 

Sharpen up your programming skills, participate in coding contests & explore high-paying jobs

Given a number N and a bit number K, check if Kth index bit of N is set or not. A bit is called set if it is 1. Position of set bit '1' should be indexed starting with 0 from LSB side in binary representation of the number.
Note: Index is starting from 0.
#### **Example 1:**

    Input: N = 4, K = 0
    Output: No
    Explanation: Binary representation of 4 is 100, 
    in which 0th index bit from LSB is not set. 
    So, return false.
#### **Example 2:**

    Input: N = 4, K = 2
    Output: Yes
    Explanation: Binary representation of 4 is 100, 
    in which 2nd index bit from LSB is set. 
    So, return true.
#### **Example 3:**

    Input: N = 500, K = 3
    Output: No
    Explanation: Binary representation of 500 is 
    111110100, in which 3rd index bit from LSB is not set. 
    So, return false.

#### **Your task:**
You don't have to read input or print anything. Your task is to complete the function checkKthbit that takes n and k as parameters and returns either true (if kth bit is set) or false(if kth bit is not set).

**Expected Time Complexity:** O(1).

**Expected Auxiliary Space:** O(1).

**Constraints:**

1 ≤ N ≤ 109
0 ≤ K ≤ floor(log2(N) + 1)


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#{ 
 # Driver Code Starts
#Initial Template for Python 3

import math


# } Driver Code Ends
#User function Template for python3


class Solution:
    
    #Function to check if Kth bit is set or not.
    def checkKthBit(self, n,k):
        #Your code here

#{ 
 # Driver Code Starts.


    
def main():
    
    T=int(input())
    
    while(T>0):
        
        
        n=int(input())
        k=int(input())
        obj = Solution()
        if obj.checkKthBit(n,k):
            print("Yes")
        else:
            print("No")
        
        T-=1

if __name__=="__main__":
    main()
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Count total set bits
</Summary>

### **Count total set bits**
**Difficulty Level : Medium** 

Sharpen up your programming skills, participate in coding contests & explore high-paying jobs

You are given a number N. Find the total count of set bits for all numbers from 1 to N(both inclusive).

#### **Example 1:**

    Input: N = 4
    Output: 5
    Explanation:
    For numbers from 1 to 4.
    For 1: 0 0 1 = 1 set bits
    For 2: 0 1 0 = 1 set bits
    For 3: 0 1 1 = 2 set bits
    For 4: 1 0 0 = 1 set bits
    Therefore, the total set bits is 5.
#### **Example 2:**

    Input: N = 17
    Output: 35
    Explanation: From numbers 1 to 17(both inclusive), 
    the total number of set bits is 35.

#### **Your Task:**
The task is to complete the function countSetBits() that takes n as a parameter and returns the count of all bits.

**Expected Time Complexity:** O(log N).

**Expected Auxiliary Space:** O(1).

**Constraints:**

1 ≤ N ≤ 108



#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    #Function to return sum of count of set bits in the integers from 1 to n.
    def countSetBits(self,n):
        # code here
        # return the count


#{ 
 # Driver Code Starts
#Initial Template for Python 3

if __name__=="__main__":
    for _ in range(int(input())):
        ob=Solution()
        print(ob.countSetBits(int(input())))
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Bit Difference
</Summary>

### **Bit Difference**
**Difficulty Level : Basic** 

Sharpen up your programming skills, participate in coding contests & explore high-paying jobs

You are given two numbers A and B. The task is to count the number of bits needed to be flipped to convert A to B.

#### **Example 1:**

    Input: A = 10, B = 20
    Output: 4
    Explanation:
    A  = 01010
    B  = 10100
    As we can see, the bits of A that need 
    to be flipped are 01010. If we flip 
    these bits, we get 10100, which is B.
#### **Example 2:**

    Input: A = 20, B = 25
    Output: 3
    Explanation:
    A  = 10100
    B  = 11001
    As we can see, the bits of A that need 
    to be flipped are 10100. If we flip 
    these bits, we get 11001, which is B.

#### **Your Task:** 
The task is to complete the function countBitsFlip() that takes A and B as parameters and returns the count of the number of bits to be flipped to convert A to B.

**Expected Time Complexity:** O(log N).

**Expected Auxiliary Space:** O(1).

**Constraints:**

1 ≤ A, B ≤ 106


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    ##Complete this function
    # Function to find number of bits needed to be flipped to convert A to B
    def countBitsFlip(self,a,b):
        ##Your code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3


import math



def main():
    
    T=int(input())
    
    while(T>0):
        
        
        ab=[int(x) for x in input().strip().split()]
        a=ab[0]
        b=ab[1]
        ob=Solution()
        print(ob.countBitsFlip(a,b))
        T-=1

if __name__=="__main__":
    main()
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Longest Consecutive 1's
</Summary>

### **Longest Consecutive 1's**
**Difficulty Level : Easy** 

Sharpen up your programming skills, participate in coding contests & explore high-paying jobs

Given a number N. Find the length of the longest consecutive 1s in its binary representation.

#### **Example 1:**

    Input: N = 14
    Output: 3
    Explanation: 
    Binary representation of 14 is 
    1110, in which 111 is the longest 
    consecutive set bits of length is 3.
#### **Example 2:**
    
    Input: N = 222
    Output: 4
    Explanation: 
    Binary representation of 222 is 
    11011110, in which 1111 is the 
    longest consecutive set bits of length 4. 

#### **Your Task:** 
You don't need to read input or print anything. Your task is to complete the function maxConsecutiveOnes() which returns the length of the longest consecutive 1s in the binary representation of given N.

**Expected Time Complexity:** O(log N).

**Expected Auxiliary Space:** O(1).

**Constraints:**

1 <= N <= 106



#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3


class Solution:
    ##Complete this function
    # Function to calculate the longest consecutive ones
    def maxConsecutiveOnes(self, N):
        ##Your code here





#{ 
 # Driver Code Starts
#Initial Template for Python 3

import math





def main():
    
    T=int(input())
    
    while(T>0):
        
        
        n=int(input())
        obj = Solution()
        print(obj.maxConsecutiveOnes(n))
        T-=1

if __name__=="__main__":
    main()
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Power of 2
</Summary>

### **Power of 2**
**Difficulty Level : Basic** 

Sharpen up your programming skills, participate in coding contests & explore high-paying jobs

Given a non-negative integer N. The task is to check if N is a power of 2. More formally, check if N can be expressed as 2x for some x.

#### **Example 1:**

    Input: N = 1
    Output: YES
    Explanation:1 is equal to 2 
    raised to 0 (20 = 1).
#### **Example 2:**
    
    Input: N = 98
    Output: NO
    Explanation: 98 cannot be obtained
    by any power of 2.

#### **Your Task:**
Your task is to complete the function isPowerofTwo() which takes n as a parameter and returns true or false by checking if the given number can be represented as a power of two or not.

**Expected Time Complexity:** O(log N).

**Expected Auxiliary Space:** O(1).

**Constraints:**

0 ≤N ≤1018


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    ##Complete this function
    # Function to check if given number n is a power of two.
    def isPowerofTwo(self,n):
        ##Your code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

import math


def main():
    
    T=int(input())
    
    while(T>0):
        
        
        n=int(input())
        ob=Solution()
        if ob.isPowerofTwo(n):
            print("YES")
        else:
            print("NO")
        
        T-=1

if __name__=="__main__":
    main()
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Swap all odd and even bits
</Summary>

### **Swap all odd and even bits**
**Difficulty Level : Easy** 

Sharpen up your programming skills, participate in coding contests & explore high-paying jobs

Given an unsigned integer N. The task is to swap all odd bits with even bits. For example, if the given number is 23 (00010111), it should be converted to 43(00101011). Here, every even position bit is swapped with an adjacent bit on the right side(even position bits are highlighted in the binary representation of 23), and every odd position bit is swapped with an adjacent on the left side.

#### **Example 1:**
    
    Input: N = 23
    Output: 43
    Explanation: 
    Binary representation of the given number 
    is 00010111 after swapping 
    00101011 = 43 in decimal.
#### **Example 2:**
    
    Input: N = 2
    Output: 1
    Explanation: 
    Binary representation of the given number 
    is 10 after swapping 01 = 1 in decimal.

#### **Your Task:**
Your task is to complete the function swapBits() which takes an integer and returns an integer with all the odd and even bits swapped.


**Expected Time Complexity:** O(1).

**Expected Auxiliary Space:** O(1).

**Constraints:**

1 ≤ N ≤ 109




#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    
    ##Complete this function
    #Function to swap odd and even bits.
    def swapBits(self,n):
        #Your code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

import math



def main():
    
    T=int(input())
    
    while(T>0):
        
        
        n=int(input())
        ob=Solution()
        print(ob.swapBits(n))
        T-=1

if __name__=="__main__":
    main()
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Maximum AND Value
</Summary>

### **Maximum AND Value**
**Difficulty Level : Medium** 

Sharpen up your programming skills, participate in coding contests & explore high-paying jobs

Given an array arr[] of N positive elements. The task is to find the Maximum AND Value generated by any pair(arri, arrj) from the array such that i != j.
Note: AND is bitwise '&' operator.


#### **Example 1:**
    
    Input: 
    N = 4
    arr[] = {4, 8, 12, 16}
    Output: 8
    Explanation:
    Pair (8,12) has the Maximum AND Value 8.
#### **Example 2:**
    
    Input:
    N = 4
    arr[] = {4, 8, 16, 2}
    Output: 0
    Explanation: Any two pairs of the array has 
    Maximum AND Value 0.

#### **Your Task:** 
You don't need to read input or print anything. Your task is to complete the function maxAND() which takes the array elements and N (size of the array) as input parameters and returns the maximum AND value generated by any pair in the array. 

**Expected Time Complexity:** O(N * log M), where M is the maximum element of the array.

**Expected Auxiliary Space:** O(1).

#### **Constraints:**
1 <= N <= 105
1 <= arr[i] <= 105


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    #Complete this function
    # Function for finding maximum AND value.
    def maxAND(self, arr,N):
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
        obj = Solution()
        print(obj.maxAND(arr,n))
        T-=1

if __name__=="__main__":
    main()
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Number is sparse or not
</Summary>

### **Number is sparse or not**
**Difficulty Level : Basic** 

Sharpen up your programming skills, participate in coding contests & explore high-paying jobs

Given a number N. The task is to check whether it is sparse or not. A number is said to be a sparse number if no two or more consecutive bits are set in the binary representation.

#### **Example 1:**
    
    Input: N = 2
    Output: 1
    Explanation: Binary Representation of 2 is 10, 
    which is not having consecutive set bits. 
    So, it is sparse number.
#### **Example 2:**

    Input: N = 3
    Output: 0
    Explanation: Binary Representation of 3 is 11, 
    which is having consecutive set bits in it. 
    So, it is not a sparse number.

#### **Your Task:** 
The task is to complete the function checkSparse() that takes n as a parameter and returns 1 if the number is sparse else returns 0.


**Expected Time Complexity:** O(1).

**Expected Auxiliary Space:** O(1).

**Constraints:**

1 <= N <= 106


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    
    #Function to check if the number is sparse or not.
    def isSparse(self,n):
        #Your code here 



#{ 
 # Driver Code Starts
#Initial Template for Python 3

import math



def main():
    
    T=int(input())
    
    while(T>0):
        
        
        n=int(input())
        ob=Solution()
        if ob.isSparse(n):
            print("1")
        else:
            print("0")
        T-=1

if __name__=="__main__":
    main()
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Binary To Gray Code equivalent
</Summary>

### **Binary To Gray Code equivalent**
**Difficulty Level : Basic** 

Sharpen up your programming skills, participate in coding contests & explore high-paying jobs

You are given a decimal number N. You need to find the gray code of the number N and convert it into decimal.
To see how it's done, refer here.

#### **Example 1:**

    Input: N = 7
    Output: 4
    Explanation: 7 is represented as 111 in 
    binary form. The gray code of 111 is 100, 
    in the binary form whose decimal equivalent 
    is 4.
#### **Example 2:**
    
    Input: N = 10
    Output: 15
    Explanation: 10 is represented as 1010 in 
    binary form. The gray code of 1010 is 1111, 
    in the binary form whose decimal equivalent 
    is 15.
#### **Example 3:**

    Input: N = 0
    Output: 0
    Explanation: Zero is represented as zero 
    in binary, gray, and decimal.

#### **Your Task:** 
The task is to complete the function greyConverter() which takes n as a parameter and returns it's equivalent gray code.

**Expected Time Complexity:** O(1).

**Expected Auxiliary Space:** O(1).

**Constraints:**

0 <= N <= 109




#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    ##Complete this fcuntion
    # Function to find the gray code of given number n
    def greyConverter(self,n):
        ##Your code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

import math




def main():
    
    T=int(input())
    
    while(T>0):
        
        
        n=int(input())
        ob=Solution()
        print(ob.greyConverter(n))
        T-=1

if __name__=="__main__":
    main()
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Gray to Binary equivalent
</Summary>

### **Gray to Binary equivalent**
**Difficulty Level : Basic** 

Sharpen up your programming skills, participate in coding contests & explore high-paying jobs

Given N in Gray Code, find its binary equivalent. Return the decimal representation of the binary equivalent.



#### **Example 1:**

    Input: N = 4
    Output: 7
    Explanation:
    Given 4 representing gray code 110.
    Binary equivalent of gray code 110 is 100.
    Return 7 representing gray code 100.
#### **Example 2:**
    
    Input: N = 15
    Output: 10
    Explanation:
    Given 15 representing gray code 1000.
    Binary equivalent of gray code 1000 is 1111.
    Return 10 representing gray code 1111 
    ie binary 1010.
#### **Example 3:**

    Input: N = 0
    Output: 0
    Explanation: 
    Zero remains the same in all systems.

#### **Your Task:** 
You don't need to read input or print anything. Your task is to complete the function grayToBinary() which accepts an integer n as an input parameter and returns decimal of the binary equivalent of the given gray code. 

**Expected Time Complexity:** O(log N)

**Expected Auxiliary Space:** O(1)

**Constraints:**

0 <= N <= 108


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:    
    ##Complete this function
    # function to convert a given Gray equivalent n to Binary equivalent.
    def grayToBinary(self,n):
        ##Your code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

import math


def main():
    
    T=int(input())
    
    while(T>0):
        
        
        n=int(input())
        ob=Solution()
        print(ob.grayToBinary(n))
        T-=1

if __name__=="__main__":
    main()
# } Driver Code Ends
```

</details>


</details>