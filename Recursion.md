# Recursion Problems

#### List of Questions:
1. The Sequence
2. Print 1 To N Without Loop 
3. Print Array Elements Using Recursion  
4. Sum of Digits of a Number
5. Count Total Digits in a Number
6. Fibonacci Using Recursion
7. Factorial Using Recursion 
8. Find nCr
9. Check Palindrome
10. Recursively Sum N Numbers
11. GCD Euclid


---


## Details of Questions Listed Above

<details>
<summary>The Sequence</summary>

### The Sequence - Final Version
**Difficulty Level : Basic**

You are given a number n. You need to recursively find the nth term of the series S that is given by:  S(n) = n+ n*(S(n-1)) and S(0) = 1

#### Example 1:
    Input: n = 2
    Output: 6

#### Example 2:
    Input: n = 3
    Output: 21
      
#### Your Task:

Complete the function theSequence that takes n as parameter and return the answer.

**Expected Time Complexity:** O(N).

**Expected Auxiliary Space:** O(N) (Recursive).

**Constraints:** 1 <= n <= 10

#### Python Code Template

```python
 #User function Template for python3

def theSequence(n):
    pass
    # code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

#contributed by RavinderSinghPB
if __name__=='__main__':
    tcs=int(input())

    for _ in range(tcs):
        n=int(input())

        print(theSequence(n))
# } Driver Code Ends
```
---
 
</details>



<details>
<summary>
 Print 1 To N Without Loop </summary>
      Dificulty Level : Basic
  
 Print numbers from 1 to N without the help of loops.
### Example 1:
Input: N = 10

Output: 1 2 3 4 5 6 7 8 9 10

### Example 2:
Input:N = 5

Output: 1 2 3 4 5
 

### **Your Task:**
**This is a function problem. You only need to complete the function printNos() that takes N as parameter and prints number from 1 to N recursively. Don't print newline, it will be added by the driver code.**

Expected Time Complexity: O(N).

Expected Auxiliary Space: O(N) (Recursive).

Constraints: 1 <= N <= 1000 

```python
 #User function Template for python3

class Solution:    
    #Complete this function
    def printNos(self,N):
      pass
        #Your code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

import math




def main():
    
    T=int(input())
    
    while(T>0):
        
        
        N=int(input())
        
        ob=Solution()
        
        ob.printNos(N)
        print()
        T-=1

if __name__=="__main__":
    main()
# } Driver Code Ends
```
</details>


<details>
<summary> Print Array Elements Using Recursion </summary>

      Dificulty Level : Basic
 You are given an array arr of size n. You need to print the array elements from start to end using given recursive function.


### Example 1:
      
Input: n = 5

arr[] = {1,2,3,4,5}
      
Output: 1 2 3 4 5

### Example 2:

Input: n = 4
      
arr[] = {5,4,2,1}
      
      
Output: 5 4 2 1
 

### Your Task:
      
      
Complete the function printArrayRecursively() that takes array and size n as parameters and prints the array elements recursively. The newline is provided by driver code.
      

      
Expected Time Complexity: O(N).
Expected Auxiliary Space: O(N) (Recursive).
      
Constraints:
1 <= n <= 100
      
```python
      
   #User function Template for python3

class Solution:
    def printArrayRecursively(self,arr,n):
      pass
        #code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

if __name__ == '__main__':
    tcs = int(input())
    
    for _ in range(tcs):
        n=int(input())
        arr=[int(x) for x in input().split()]
        ob=Solution()
        ob.printArrayRecursively(arr,n)
        print()


# } Driver Code Ends
```      

      
</details>

<details>
<summary> Sum of Digits of a Number  </summary>

      Dificulty Level : Basic
You are given a number n. You need to find the sum of digits of n.

### Example 1:

Input: n = 1

Output: 1
      
Explanation: Sum of digit of 1 is 1.

### Example 2:

Input: n = 99999
      
Output: 45
      
Explanation: Sum of digit of 99999 is 45.
      
### Your Task:
      
You don't need to read input or print anything. Your task is to complete the function sumOfDigits() that takes n as parameter and returns the sum of digits of n.
      

Expected Time Complexity: O(Logn).
      
Expected Auxiliary Space: O(Logn) (Recursive).
      

Constraints:
      
1 <= n <= 107

```python
 #User function Template for python3

class Solution:
    def sumOfDigits(self, n):
        '''
        :param n: given number
        :return: sum of digits of n.
        '''
        # code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3
import atexit
import io
import sys

#Contributed by : Nagendra Jha

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
        print(Solution().sumOfDigits(n))
# } Driver Code Ends

```
</details>

<details>
<summary>Count Total Digits in a Number</summary>
      
      Dificulty Level : Basic      
You are given a number n. You need to find the count of digits in n.

### Example 1:

Input: n = 1
      
      
Output: 1
      
Explanation: Number of digit in 1 is 1.
      
### Example 2:
Input:n  = 99999
      
Output: 5
      
Explanation:Number of digit in 99999 is 5
      
### Your Task:
      
You don't need to read input or print anything. Your task is to complete the function countDigits() that takes n as parameter and returns the count of digits in n.
      

Expected Time Complexity: O(Logn).
      
Expected Auxiliary Space: O(Logn).
      

Constraints:  0 <= n <= 107 
      
```python    
#User function Template for python3

class Solution:
    def countDigits(self, n):
        '''
        :param n: given number
        :return: count of digits of n.
        '''
        # code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3
import atexit
import io
import sys

#Contributed by : Nagendra Jha
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
        print(Solution().countDigits(n))
# } Driver Code Ends
```
</details>

<details>
<summary> Fibonacci Using Recursion </summary>
      
      Dificulty Level : Basic
 You are given a number n. You need to find nth Fibonacci number.
      
F(n)=F(n-1)+F(n-2); where F(1)=1 and F(2)=1

Example 1:

Input:n = 1
      
Output: 1
      
Explanation: The first fibonacci number is 1
      
### Example 2:

Input:n = 20
      
Output:6765
      
Explanation: The 20th fibonacci number is 6765
      
### Your Task:
      
You don't need to read input or print anything. You only need to complete the function fibonacci that takes n as parameters and returns the n-th fibonacci number.
      

Expected Time Complexity: O(2n).
      
Expected Auxiliary Space: O(N).
      

Constraints: 1 <= n <= 20

```python

 #User function Template for python3

class Solution:
    def fibonacci(self,n):
      pass
        #code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3
import atexit
import io
import sys

#Contributed by : Nagendra Jha

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
        ob=Solution()
        print(ob.fibonacci(n))
# } Driver Code Ends
```
      
</details>

<details>
<summary> Factorial Using Recursion </summary>
      
       Dificulty Level : Basic
You are given a number n. You need to recursively find the factorial of n and return it.

### Example 1:

Input: n = 5
      
Output: 120
      
### Example 2:

Input: n = 0
      
Output: 1
      
### Your Task:
      

Complete the function factorial that takes n as parameter and returns the factorial.
      

Expected Time Complexity: O(N).
      
Expected Auxiliary Space: O(N) (Recursive).
      

Constraints: 0 <= n <= 10
      
```python
      
 #User function Template for python3

class Solution:
    def factorial(self,n):
      pass
        #code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

#contributed by RavinderSinghPB
if __name__ =='__main__':
    tcs=int(input())
    
    for _ in range(tcs):
        n=int(input())
        ob=Solution()
        print(ob.factorial(n))
# } Driver Code Ends
      
```
</details>


<details>
<summary> Find nCr  </summary>
      
      Dificulty Level : Basic
You are given two numbers n and r. You need to find nCr.
nCr = (n!) / ((n-r)!*(r!))
      
In recursive way, we can write nCr as nCr = (n-1)C(r-1) + (n-1)Cr

### Example 1:

Input: n = 5, r = 2
      
Output: 10
      
### Example 2:

Input:n = 4, r = 1
      
Output: 4
      
### Your Task:
      
You only need to complete the function nCr that takes n and r as parameters and returns the nCr.
      

Expected Time Complexity: O(2N).
      
Expected Auxiliary Space: O(2N) (Recursive).
      

Constraints: 1 <= r <= n <= 30
     
```python
       
      #User function Template for python3

def nCr(n,r):
  pass
    #code here
    


#{ 
 # Driver Code Starts
#Initial Template for Python 3

#contributed by RavinderSinghPB
if __name__ == '__main__':
    tcs=int(input())
    
    for _ in range(tcs):
        n,r=[int(x) for x in input().split()]
        
        print(nCr(n,r))
# } Driver Code Ends
```
                
                
</details>


<details>
<summary> Check Palindrome  </summary>
      
      Dificulty Level : Basic
You are given a number n. You need to see if the number is a palindrome or not (recursively)

### Example 1:

Input: n = 100
      
Output: 0
      
### Example 2:

Input:n = 101
      
Output: 1
      
### Your Task:
      

Complete the function isPalin that takes n as parameter and returns true or false . (In case of true, 1 will be printed by the driver code, otherwise 0)
      

Expected Time Complexity: O(Log(N)).
      
Expected Auxiliary Space: O(Log(N)) (Recursive).
      

Constraints: 1 <= n <= 108
      
      
      
```python
      
      #User function Template for python3

class Solution:
    def isPalin(self,N):
      pass
        #code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

#contributed by RavinderSinghPB
if __name__ == '__main__':
    tcs=int(input())
    
    for _ in range(tcs):
        n=int(input())
        obj = Solution()
        print(int(obj.isPalin(n)))
# } Driver Code Ends
```
      
</details>



<details>
<summary> Recursively Sum N Numbers  </summary>
      
      Dificulty Level : Basic
You are given a number n. You need to recursively sum the numbers from 1 to n and return the sum.

### Example 1:

Input: n = 5
      
Output: 15
      
### Example 2:

Input: n = 4
      
Output: 10
      
### Your Task:
      

Complete the function recursiveSum that takes n as paramenter and return the sum.
      

Expected Time Complexity: O(N).
      
Expected Auxiliary Space: O(N) (Recursive).
      

Constraints: 0 <= n <= 100
      
      
      
```python
      
 #User function Template for python3

class Solution:
    def recursiveSum(self,n):
      pass
        #code here
        
        


#{ 
 # Driver Code Starts
#Initial Template for Python 3

#contributed by RavinderSinghPB
if __name__ =='__main__':
    tcs=int(input())
    
    for _ in range(tcs):
        n=int(input())
        ob=Solution()
        print(ob.recursiveSum(n))
# } Driver Code Ends
```
      
</details>


<details>
<summary> GCD Euclid  </summary>
      
      Dificulty Level : Basic
You are given a two numbers a and b. Find their GCD using recursion.

### Example 1:

Input: a = 7, b = 8
      
Output: 1
      
### Example 2:

Input: a = 2, b = 4
      
Output: 2
      
### Your Task:
      

Complete the function GCD that takes a and b as parameters and returns the GCD.
      

Expected Time Complexity: O(Log(N)).
      
Expected Auxiliary Space: O(Log(N)) (Recursive).
      

Constraints: 1 <= a, b <= 100
      
      
```python
      
 #User function Template for python3

class Solution:
    def GCD(self,a,b):
      pass
        #code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

if __name__ =='__main__':
    tcs= int(input())
    
    for _ in range(tcs):
        a,b=[int(x) for x in input().split()]
        ob=Solution()
        print(ob.GCD(a,b))
# } Driver Code Ends
 ```     
 
</details>
