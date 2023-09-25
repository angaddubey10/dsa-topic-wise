### List of Questions
1. Absolute Value
2. Convert Celsius To Fahrenheit
3. Factorial Of Number
4. Digits In Factorial
5. Primality Test
6. Exactly 3 Divisors
7. Quadratic Equation Roots
8. GP Term
9. Addition Under Modulo
10. Multiplication Under Modulo
11. Modular Multiplicative Inverse


----

## Details of Questions Listed Above 

<details>
<summary>
Absolute Value
</Summary>

### **Absolute Value**
**Difficulty Level : Basic** 

Last Week Of Job Fair 2023. Explore Unlimited Opportunities Now!
You are given an interger I, find the absolute value of the interger I.

#### **Example 1:**
    Input:
    I = -32
    Output: 32
    Explanation:  The absolute value of -32 is 32.
 
       
#### **Example 2:**

    Input:
    I = 45
    Output: 45
    Explanation: 
    The absolute value of 45 is 45 itself.
 

#### **Your Task:**
You don't need to read input or print anything. Your task is to complete the function absolute() which takes an integer I as input parameter and return the absolute value of I.

 

**Expected Time Complexity:** O(1)

**Expected Auxiliary Space :** O(1)

 

**Constraints:**
-106 <= I <= 106



#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#{ 
 # Driver Code Starts
# Initial Template for Python 3



# } Driver Code Ends
# User function Template for python3

class Solution:
    def absolute(self,I):
        # code here


#{ 
 # Driver Code Starts.
def main():
    T = int(input()) #Input the number of testcases
    while(T > 0):
        I = int(input()) #input number
        ob=Solution()
        print(ob.absolute(I)) #Call function and print
        T -= 1 #Reduce number of testcases


if __name__ == "__main__":
    main()

# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Convert Celsius To Fahrenheit
</Summary>

### **Convert Celsius To Fahrenheit**
**Difficulty Level : Basic** 

Last Week Of Job Fair 2023. Explore Unlimited Opportunities Now!
Given a temperature in celsius C. You need to convert the given temperature to Fahrenheit.

#### **Example 1:**
    Input:
    C = 32
    Output: 89
    Explanation: Using the conversion 
    formula of celsius to farhenheit , it
    can be calculated that, for 32 degree
    C, the temperature in Fahrenheit = 89.
#### **Example 2:**
    Input:
    50
    Output: 122
    Explanation: Using the conversion 
    formulaof celsius to farhenheit, it
    can be calculated that, for 50 degree
    C, the temperature in Fahrenheit = 122.
#### **Your Task:**
You don't need to read input or print anything. Your task is to complete the function CtoF() that takes C as parameter and returns temperature in fahrenheit( in double). The flooring and printing is automatically done by the driver code.

**Expected Time Complexity:** O(1)

**Expected Auxiliary Space :** O(1)

**Constraints:**

1 <= C <= 104


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python#{ 
 # Driver Code Starts
#Initial Template for Python 3

import math


# } Driver Code Ends
#User function Template for python3

class Solution:
    ##Complete this function
    def cToF(self,C):
        #Your code here


#{ 
 # Driver Code Starts.
def main():
    
    T=int(input())
    
    while(T>0):
        C=int(input())
        ob=Solution()
        print(math.floor(ob.cToF(C)))
        T-=1
    
    




if __name__=="__main__":
    main()
# } Driver Code Ends

```

</details>


</details>

<details>
<summary>
Factorial Of Number
</Summary>

### **Factorial Of Number**
**Difficulty Level : Easy** 

Last Week Of Job Fair 2023. Explore Unlimited Opportunities Now!
Given a positive integer N. The task is to find factorial of N.

#### **Example 1:**
    Input:
    N = 4
    Output: 24
    Explanation: 4! = 4 * 3 * 2 * 1 = 24
#### **Example 2:**
    Input:
    N = 13
    Output: 6227020800
    Explanation: 
    13! = 13 * 12 * .. * 1 = 6227020800
#### **Your Task:**
You don't need to read input or print anything. Your task is to complete the function factorial() that takes N as parameter and returns factorial of N.

**Expected Time Complexity :** O(N)

**Expected Auxilliary Space :** O(1)

**Constraints:**

0 <= N <= 18


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
    #You need to complete this function
    def factorial(self,N):
        #Your code here


#{ 
 # Driver Code Starts.

def main():
    
    T=int(input())
    
    while(T>0):
        N=int(input())
        ob=Solution()
        
        print(ob.factorial(N))
        
        
        T-=1
    
    




if __name__=="__main__":
    main()
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Digits In Factorial
</Summary>

### **Digits In Factorial**
**Difficulty Level : Easy** 

Last Week Of Job Fair 2023. Explore Unlimited Opportunities Now!
Given an integer N. Find the number of digits that appear in its factorial. 
Factorial is defined as, factorial(n) = 1*2*3*4……..*N and factorial(0) = 1.
 

#### **Example 1:**
    Input: N = 5
    Output: 3
    Explanation: Factorial of 5 is 120.
    Number of digits in 120 is 3 (1, 2, and 0)
 

#### **Example 2:**
    Input: N = 120
    Output: 199
    Explanation: The number of digits in
    120! is 199

#### **Your Task:**
You don't need to read input or print anything. Your task is to complete the function digitsInFactorial() that takes N as input parameter and returns number of digits in factorial of N.


**Expected Time Complexity :** O(N)

**Expected Auxilliary Space :** O(1)


**Constraints:**

1 ≤ N ≤ 105


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    def digitsInFactorial(self,N):
        # code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

import math

def main():
    
    T=int(input())
    
    while(T>0):
        N=int(input())
        ob=Solution()
        print(ob.digitsInFactorial(N))
        
        T-=1

if __name__=="__main__":
    main()
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Primality Test
</Summary>

### **Primality Test**
**Difficulty Level : Easy** 

Last Week Of Job Fair 2023. Explore Unlimited Opportunities Now!
A prime number is a number which is only divisible by 1 and itself.
Given number N check if it is prime or not.

 

#### **Example 1:**
    Input:
    N = 5
    Output: Yes
    Explanation: 5 is only divisible by 1 
    and itself. So, 5 is a prime number.
 

#### **Example 2:**
    Input:
    N = 4
    Output: No
    Explanation: 4 is divisible by 2. 
    So, 4 is not a prime number.
 

#### **Your Task:**
You don't need to read input or print anything. Your task is to complete the function isPrime() that takes N as input parameter and returns True if N is prime else returns False. 

 

**Expected Time Complexity :** O(N1/2)

**Expected Auxilliary Space :**  O(1)

 

**Constraints:**

1 <= N <= 109


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
    def isPrime(self,N):
        # code here

#{ 
 # Driver Code Starts.
def main():
    
    T=int(input())
    
    while(T>0):
        
        N=int(input())
        
        ob=Solution()
        if(ob.isPrime(N)):
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
Exactly 3 Divisors
</Summary>

### **Exactly 3 Divisors**
**Difficulty Level : Easy**

Last Week Of Job Fair 2023. Explore Unlimited Opportunities Now!
Given a positive integer value N. The task is to find how many numbers less than or equal to N have numbers of divisors exactly equal to 3.

 

#### **Example 1:**
    Input:
    N = 6
    Output: 1
    Explanation: The only number less than 6 with 
    3 divisors is 4.
#### **Example 2:**

    Input:
    N = 10
    Output: 2
    Explanation: 4 and 9 have 3 divisors.
 

#### **Your Task:**
You don't need to read input or print anything. Your task is to complete the function exactly3Divisors() that takes N as input parameter and returns count of numbers less than or equal to N with exactly 3 divisors.

 

**Expected Time Complexity :** O(N1/2 * N1/4)

**Expected Auxilliary Space :**  O(1)

 

**Constraints :**

1 <= N <= 109


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
    def exactly3Divisors(self,N):
        # code here

#{ 
 # Driver Code Starts.
def main():
    
    T=int(input())
    
    while(T>0):
        
        N=int(input())
        ob=Solution()
        print(ob.exactly3Divisors(N))
        
        T-=1
    

if __name__=="__main__":
    main()
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Quadratic Equation Roots
</Summary>

### **Quadratic Equation Roots**
**Difficulty Level : Basic**

Last Week Of Job Fair 2023. Explore Unlimited Opportunities Now!
Given a quadratic equation in the form ax2 + bx + c. Find its roots.

Note: Return the maximum root followed by the minimum root.

#### **Example 1:**

    Input:
    a = 1
    b = -2
    c = 1
    Output: 1 1
    Explanation:
    Roots of equation x2-2x+1 are 1 and 1.

#### **Example 2:**

    Input:
    a = 1
    b = -7
    c = 12
    Output: 4 3
    Explanation: Roots of equation 
    x2 - 7x + 12 are 4 and 3.
 

#### **Your Task:**
You don't need to read input or print anything. Your task is to complete the function quadraticRoots() which takes a, b, c as input parameters and returns a list of two integers containing the floor value of its roots in decreasing order. If roots are imaginary, the returning list should contain only 1 integer ie -1. Always return the greatest integer smaller than or equal to the result.
Note: If roots are imaginary, the generated output will display "Imaginary".

 

**Expected Time Complexity:** O(1)

**Expected Auxiliary Space :** O(1)

 

**Constraints:**

-103 <= a,b,c <= 103


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3



class Solution:
    def quadraticRoots(self, a, b, c):
        # code here




#{ 
 # Driver Code Starts
#Initial Template for Python 3

if __name__ == '__main__':
    tc = int(input())
    for _ in range(tc):
        abc=[int(x) for x in input().strip().split()]
        a=abc[0]
        b=abc[1]
        c=abc[2]
        ob = Solution()
        ans = ob.quadraticRoots(a,b,c)
        if len(ans)==1 and ans[0]==-1:
            print("Imaginary")
        else:
            for i in range(len(ans)):
                print(ans[i], end=" ")
            print()

# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
GP Term
</Summary>

### **GP Term**
**Difficulty Level : Easy**

Last Week Of Job Fair 2023. Explore Unlimited Opportunities Now!
Given the first 2 terms A and B of a Geometric Series. The task is to find the Nth term of the series.

#### **Example 1:**

    Input:
    A = 2 
    B = 3
    N = 1
    Output: 2
    Explanation: The first term is already
    given in the input as 2
#### **Example 2:**

    Input:
    A = 1
    B = 2
    N = 5
    Output: 16
    Explanation: Common ratio = 2,
    Hence second term is 1*(2)(5-1) = 24 = 16 .
#### **Your Task:**
You don't need to read input or print anything. Your task is to complete the function termOfGP() that takes A, B and N as parameter and returns Nth term of GP. The return value should be double that would be automatically converted to floor by the driver code.

**Expected Time Complexity :** O(logN)

**Expected Auxilliary Space :** O(1)

**Constraints:**

-100 <= A <= 100
-100 <= B <= 100
1 <= N <= 5


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
    #Compelte his function
    def termOfGP(self,A,B,N):
        #Your code here


#{ 
 # Driver Code Starts.
def main():
    
    T=int(input())
    
    while(T>0):
        
        AB=[int(x) for x in input().strip().split()]
        A=AB[0]
        B=AB[1]
        
        N=int(input())
        ob=Solution()
        print(math.floor(ob.termOfGP(A,B,N)))
        
        T-=1
    
    




if __name__=="__main__":
    main()
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Addition Under Modulo
</Summary>

### **Addition Under Modulo**
**Difficulty Level : Basic**

Last Week Of Job Fair 2023. Explore Unlimited Opportunities Now!
Given two numbers a and b, find the sum of a and b. Since the sum can be very large, find the sum modulo 109+7.

 

#### **Example 1:**

    Input:
    a = 9223372036854775807
    b = 9223372036854775807
    Output: 582344006
    Explanation: 
    9223372036854775807 + 9223372036854775807 
    = 18446744073709551614.
    18446744073709551614 mod (109+7)
    = 582344006
 

#### **Example 2:**

    Input:
    a = 1000000007
    b = 1000000007
    Output: 0
    Explanation: 1000000007 + 1000000007 =
    (2000000014) mod (109+7) = 0
 

#### **Your Task:**
You don't need to read input or print anything. Your task is to complete the function sumUnderModulo() that takes a and b as input parameters and returns sum of a and b under modulo 109+7.

 

**Expected Time Complexity :** O(1)

**Expected Auxilliary Space :**  O(1)

 

**Constraints:**

1 <= a,b <= 263-1


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    def sumUnderModulo(self,a,b):
        # code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

import atexit
import io
import sys

if __name__ == '__main__':
    test_cases = int(input())
    for cases in range(test_cases):
        a,b = map(int,input().strip().split())
        ob=Solution()
        print(ob.sumUnderModulo(a,b))

# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Multiplication Under Modulo
</Summary>

### **Multiplication Under Modulo**
**Difficulty Level : Basic**

Last Week Of Job Fair 2023. Explore Unlimited Opportunities Now!
You are given two numbers a and b. You need to find the multiplication of a and b under modulo M (M as 109+7).

#### **Example 1:**

    Input:
    a = 92233720368547758
    b = 92233720368547758
    Output: 484266119
    Explanation: Multiplication of a and b 
    under modulo M will be 484266119.
#### **Example 2:**

    Input:
    a = 1000000007
    b = 1000000007
    Output: 0
    Explanation: Multiplication of a and b
    under modulo M is 0.
#### **Your Task:**
You don't need to read input or print anything. Your task is to complete the function multiplicationUnderModulo() that takes a and b as parameters and returns multiplication of a and b under modulo M.

**Expected Time Complexity :** O(1)

**Expected Auxilliary Space :**  O(1)

**Constraints:**
1 <= a,b <= 263-1


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    def multiplicationUnderModulo(self,a,b):
        '''
        :param a: given value of a
        :param b: given value of b
        :return: Integer , sum under modulo
        '''   
        # code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3
import atexit
import io
import sys

# Contributed by : Nagendra Jha

if __name__ == '__main__':
    test_cases = int(input())
    for cases in range(test_cases):
        a,b = map(int,input().strip().split())
        ob=Solution()
        print(ob.multiplicationUnderModulo(a,b))

# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Modular Multiplicative Inverse
</Summary>

### **Modular Multiplicative Inverse**
**Difficulty Level : Easy**

Last Week Of Job Fair 2023. Explore Unlimited Opportunities Now!
Given two integers ‘a’ and ‘m’. The task is to find the smallest modular multiplicative inverse of ‘a’ under modulo ‘m’.

 

#### **Example 1:**

    Input:
    a = 3
    m = 11
    Output: 4
    Explanation: Since (4*3) mod 11 = 1, 4 
    is modulo inverse of 3. One might think,
    15 also as a valid output as "(15*3)
    mod 11"  is also 1, but 15 is not in 
    ring {0, 1, 2, ... 10}, so not valid.
 

#### **Example 2:**

    Input:
    a = 10
    m = 17
    Output: 12
    Explanation: Since (12*10) mod 17 = 1,
    12 is the modulo inverse of 10.
 

#### **Your Task:**
You don't need to read input or print anything. Your task is to complete the function function modInverse() that takes a and m as input parameters and returns modular multiplicative inverse of ‘a’ under modulo ‘m’. If the modular multiplicative inverse doesn't exist return -1.

 

**Expected Time Complexity :** O(m)

**Expected Auxilliary Space :** O(1)

 

**Constraints:**

1 <= a <= 104
1 <= m <= 104


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
    ##Complete this function
    def modInverse(self,a,m):
        ##Your code here

#{ 
 # Driver Code Starts.
    
    
def main():
    
    T=int(input())
    
    while(T>0):
        
        
        am=[int(x) for x in input().strip().split()]
        a=am[0]
        m=am[1]
        ob=Solution()
        print(ob.modInverse(a,m))
        
        
        T-=1
    
    




if __name__=="__main__":
    main()
# } Driver Code Ends
```

</details>


</details>