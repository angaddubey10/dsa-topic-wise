### List of Questions 
1. Hashing for pair - 1
2. Hashing for pair - 2
3. Linear Probing in Hashing
4. Quadratic Probing in Hashing
5. Separate chaining in Hashing
6. Count Non-Repeated Elements
7. Print Non-Repeated Elements
8. Non Repeating Character
9. Winner of an election
10. First Repeating Element


______

 ## Details of Questions Listed Above

 <details>
<summary>
Hashing for pair - 1
</Summary>

### **Hashing for pair - 1**
**Difficulty Level : Easy** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 

You are given an array of distinct integers and a sum. Check if there's a pair with the given sum in the array.

#### **Example 1:**

    Input:
    N = 10
    arr[] = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10} 
    sum = 14
    Output: 
    1

    Explanation: 
    arr[] = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10} 
    and sum = 14.  There is a pair {4, 10} 
    with sum 14.
#### **Example 2:**

    Input:
    N = 2
    arr[] = {2, 5}
    sum = 10
    Output:
    0

    Explanation: 
    arr[]  = {2, 5} and sum = 10. 
    There is no pair with sum 10.
#### **Your Task:**
You don't need to read input or print anything. Your task is to complete the provided function sumExists () which take the array arr[], its size N, and an integer sum as inputs and returns 1 if there exists a pair with the given sum in the array, else, it returns 0.

**Expected Time Complexity:** O(N).

**Expected Auxiliary Space:** O(N).

**Constraints:** 

1 <= N <= 1000
1 <= arri <= 106
1 <= sum <= 1000


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#{ 
 # Driver Code Starts
#Initial Template for Python 3

# } Driver Code Ends
#User function Template for python3

##Complete this function
#Function to check if there is a pair with the given sum in the array.
def sumExists(arr, N, sum):
    #Your code here

#{ 
 # Driver Code Starts.

def main():
    testcases=int(input())
    while(testcases>0):
        
        N=int(input())
        
        arr=[int(x) for x in input().strip().split()]
        
        sum=int(input())
        
        
        print(sumExists(arr,N,sum))
        
        testcases-=1
        
        

if __name__=="__main__":
    main()
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Hashing for pair - 2
</Summary>

### **Hashing for pair - 2**
**Difficulty Level : Easy** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 

You are given an array of integers and an integer sum. You need to find if two numbers in the array exists that have sum equal to the given sum.

#### **Example 1:**

    Input:
    N = 10
    arr[] = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10}
    sum = 14

    Output: 
    1

    Explanation: 
    there exists a pair which 
    gives sum as 14 example 
    (4,10),(5,9) etc.
#### **Example 2:**

    Input:
    N = 4
    arr[] ={4, 3, 5, 6}
    sum = 12

    Output: 
    0

    Explanation: 
    there does not exist any
    such pair which gives sum as 12.

#### **Your Task:**

You don't need to read input or print anything. You just have to complete the function sumExists() which takes the array arr[], its size N and an integer sum as inputs and returns 1 if there exists a pair with the given sum in the array. Else, it returns 0. 

**Expected Time Complexity:** O(N).

**Expected Auxiliary Space:** O(N).

**Constraints:**

1 <= N <= 1000
1 <= arri <= 106
1 <= sum <= 1000


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#{ 
 # Driver Code Starts
#Initial Template for Python 3

# } Driver Code Ends
#User function Template for python3

#Function to check if two numbers in the array have sum equal to the given sum.
def sumExists(arr, N, sum):
    ##Your code here

#{ 
 # Driver Code Starts.



def main():
    testcases=int(input())
    while(testcases>0):
        
        N=int(input())
        
        arr=[int(x) for x in input().strip().split()]
        
        sum=int(input())
        
        
        print(sumExists(arr,N,sum))
        
        testcases-=1
        
        

if __name__=="__main__":
    main()
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Linear Probing in Hashing
</Summary>

### **Linear Probing in Hashing**
**Difficulty Level : Easy** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 

Linear probing is a collision handling technique in hashing. Linear probing says that whenever a collision occurs, search for the immediate next position.

Given an array of integers and a hash table size. Fill the array elements into a hash table using Linear Probing to handle collisions. Duplicate elements must be mapped to the same position in the hash table while colliding elements must be mapped to the [(value+1)%hashSise] position.

#### **Example 1:**

    Input:
    hashSize = 10
    sizeOfArray = 4 
    Array[] = {4,14,24,44}
    Output:
    -1 -1 -1 -1 4 14 24 44 -1 -1
    Explanation: 4%10=4. So put 4 in 
    hashtable[4].Now, 14%10=4, but 
    hashtable[4] is alreadyfilled so put 
    14 in the next slot and so on.
#### **Example 2:**

    Input:
    hashSize = 10
    sizeOfArray = 4 
    Array[] = {9,99,999,9999}
    Output:
    99 999 9999 -1 -1 -1 -1 -1 -1 9
    Explanation: 9%10=9. So put 9 in 
    hashtable[9]. Now, 99%10=9, but 
    hashtable[9] is already filled so 
    put 99 in the (99+1)%10 =0 slot so
    99 goes into hashtable[0] and so on.
#### **Your Task:**
You don't need to read input or print anything. Your task is to complete the function linearProbing() which takes the hash table size (hashSize), an integers array arr[] and its size N as input parameters and inserts all the elements of the array arr[] into a hash table. The function should return the hash table. 
The empty cells of the hash table are to be given a value of -1.
Also, if there's no more space to insert a new element, just drop that element. 


**Expected Time Complexity:** O(N)

**Expected Auxiliary Space:**O(1)


**Constraints:**

1 <= hashSize <= 1000
1 <= sizeOfArray <= 10000
0 <= Array[] <= 105


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    #Function to fill the array elements into a hash table 
    #using Linear Probing to handle collisions.
    def linearProbing(self,hashSize, arr, sizeOfArray):
        #Your code here



#{ 
 # Driver Code Starts
#Initial Template for Python 3

def main():
    T=int(input())
    
    while(T>0):
        
        hashSize=int(input())
        sizeOfArray=int(input())
        arr=[int(x) for x in input().strip().split()]
        
        obj = Solution()
        hash = obj.linearProbing( hashSize, arr, sizeOfArray)
        
        for i in hash:
            print(i,end=" ")
        print()
        T-=1


if __name__=="__main__":
    main()
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Quadratic Probing in Hashing
</Summary>

#### **Quadratic Probing in Hashing**
**Difficulty Level : Easy** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 

Quadratic probing is a collision handling technique in hashing. Quadratic probing says that whenever a collision occurs, search for i2 position.

Given an array of integers and a Hash table. Fill the elements of the array into the hash table by using Quadratic Probing in case of collisions.

#### **Example 1:**

    Input:
    hashSize = 11
    N = 4
    Array[] = {21,10,32,43}
    Output: 
    10 -1 -1 32 -1 -1 -1 -1 43 -1 21
    Explanation: 21%11=10 so 21 goes into 
    hashTable[10] position. 10%11=10. 
    hashTable[10] is already filled so we try 
    for (10+12)%11=0 position. hashTable[0] 
    is empty so we put 10 there. 32%11=10. 
    hashTable[10] is filled. We try 
    (32+12)%11=0. But hashTable[0] is also 
    already filled. We try (32+22)%11=3. 
    hashTable[3] is empty so we put 32 in 
    hashTable[3] position. 43 uses 
    (43+32)%11=8. We put it in hashTable[8].
#### **Example 2:**

    Input:
    hashSize = 11
    N = 4
    Array[] = {880,995,647,172 }
    Output:
    880 -1 -1 -1 -1 995 -1 172 -1 647 -1 
    Explanation: Using the similar approach 
    as used in above explanation we will get 
    the output like 
    880 -1 -1 -1 -1 995 -1 172 -1 647 -1.
#### **Example 3:**

    Input: 
    hashSize = 11 
    N = 4 
    Array[] = {4,4,4,4} 
    Output: -1 -1 -1 -1 4 -1 -1 -1 -1 -1 -1 
    Your Task:
    You don't need to read input or print anything. Your task is to complete the function QuadraticProbing() which takes the hash table hash[], the hash table size hashSize, an array arr[] and the size of the array N as inputs and inserts all the elements of the array arr[] into the hash table using Quadratic Probing as a collision handling technique.

**Note:** You need to map duplicate elements incase, they have the same hash value even after quadratic probing.

**Expected Time Complexity:** O(N).

**Expected Auxiliary Space:** O(1).

**Constraints:**

2 <= hashSize (prime) <= 97
1 <= N < hashSize*0.5
0 <= Array[] <= 105

**Note:**
All the positions that are unoccupied are denoted by -1 in the hash table.
An empty slot can only be found if load factor < 0.5 and hash table size is a prime number.
The given testcases satisfy the above condition so you can assume that an empty slot is always reachable.


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3
class Solution:
    
    #Function to fill the array elements into a hash table 
    #using Quadratic Probing to handle collisions.
    def QuadraticProbing(self,hash, hashSize, arr, N):
        #Your code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3



def main():
    T=int(input())
    
    while(T>0):
        
        
        hashSize=int(input())
        N=int(input())
        arr=[int(x) for x in input().strip().split()]
        
        hash = [-1]*hashSize
        obj = Solution()
        obj.QuadraticProbing(hash, hashSize, arr, N)
        
        for i in hash:
            print(i,end=" ")
        print()
        T-=1


if __name__=="__main__":
    main()
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Separate chaining in Hashing
</Summary>

### **Separate chaining in Hashing**
**Difficulty Level : Easy** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 

Separate chaining technique in hashing allows to us to use a linked list at each hash slot to handle the problem of collisions. That is, every slot of the hash table is a linked list, so whenever a collision occurs, the element can be appened as a node to the linked list at the slot.

In this question, we'll learn how to fill up the hash table using Separate chaining technique. Given an array (consisting of distinct integers)  and a hashtable size, you have to fill the elements of the array into a hash table of given size. 

#### **Example 1:**

    Input:
    hashSize = 10
    sizeOfArray = 6
    arr[] = {92,4,14,24,44,91}
    Output:
    1->91
    2->92
    4->4->14->24->44
    Explanation: 92%10=2 so 92 goes to slot 2.
    4%10=4 so 4 goes to slot 4. 14%10=4. But 4
    is already occupied so we make a linked
    list at this position and add 14 after 4 
    in slot 4 and so on.
#### **Example 2:**

    Input:
    hashSize = 10
    sizeOfArray = 5
    arr[] = {12,45,36,87,11}
    Output:
    1->11
    2->12
    5->45
    6->36
    7->87
    Explanation: 12%10=2 so 12 goes to slot 2.
    45%10=5 goes to slot 5. 36%10=6 goes to
    slot 6. 87%10=7 goes to slot 7 and finally
    11%10=1 goes to slot 1.
#### **Your Task:**
This is a function problem. You need to complete the function separateChaining that takes hashSize, arr, and sizeOfArr as parameters, inserts elements of arr in the hashTable at positions by using arr[i]%hashSize and then returns the has table. The printing is done automatically by the driver code.

**Expected Time Complexity:** O(N).

**Expected Auxiliary Space:** O(N).

**Constraints:**

2 <= hashSize <= 103
1 <= sizeOfArray <= 103
0 <= arri <= 107



#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    
    #Function to insert elements of array in the hashTable avoiding collisions.
    def separateChaining(self, hashSize, arr, sizeOfArray):
        #Your code here
        #return hashtable


#{ 
 # Driver Code Starts
#Initial Template for Python 3

import math
#Back-end complete function Template for Python 3

def main():
        T=int(input())
        while(T>0):
            
            hashSize=int(input())
            sizeOfArray=int(input())
            arr=input().strip()
            arr=arr.split()
            arr=list(map(int,arr))
            
            obj = Solution()
            hashTable = obj.separateChaining( hashSize, arr, sizeOfArray)
            
            
            for i in range(len(hashTable)):
                if len(hashTable[i])>0:
                    print(str(i)+"->",end="")
                    for j in range(len(hashTable[i])-1):
                        print(str(hashTable[i][j])+"->",end="")
                    print(hashTable[i][len(hashTable[i])-1],end="")
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
Count Non-Repeated Elements

</Summary>

#### **Count Non-Repeated Elements**
**Difficulty Level : Easy** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 

Hashing is very useful to keep track of the frequency of the elements in a list.

You are given an array of integers. You need to print the count of non-repeated elements in the array.

#### **Example 1:**

    Input:
    10
    1 1 2 2 3 3 4 5 6 7

    Output: 
    4

    Explanation: 
    4, 5, 6 and 7 are the 
    elements with frequency 1 and rest 
    elements are repeated so the number 
    of non-repeated elements are 4.
#### **Example 2:**

    Input:
    5
    10 20 30 40 10

    Output: 
    3

    Explanation: 
    20, 30, 40 are the 
    elements with the frequency 1 and 
    10 is the repeated element to 
    number of non-repeated elements 
    are 3.
#### **Your Task:** 
You don't need to read input or print anything. You only need to complete the function countNonRepeated() that takes array arr[] and its size n as parameters and returns the count of non-repeating elements in the array. 

**Expected Time Complexity:** O(n).

**Expected Auxiliary Space:** O(n).

**Constraints:**

1 <= n <= 103
0 <= arri <= 107


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python

#User function Template for python3
class Solution:
    
    #Complete this code
    #Function to return the count of non-repeated elements in the array.
    def countNonRepeated(self,arr,n):
        #Your code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3


def main():
    T=int(input())
    while(T>0):
        
        n=int(input())
        arr=[int(x) for x in input().strip().split()]
        print(Solution().countNonRepeated(arr,n))
        
        
        T-=1

if __name__=="__main__":
    main()
# } Driver Code Ends
```

</details>


</details>


<details>
<summary>
Print Non-Repeated Elements
</Summary>


#### **Print Non-Repeated Elements**
**Difficulty Level : Easy** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 

Hashing is very useful to keep track of the frequency of the elements in a list.

You are given an array of integers. You need to print the non-repeated elements as they appear in the array.

#### **Example 1:**

    Input:
    n = 10
    arr[] = {1,1,2,2,3,3,4,5,6,7}
    Output: 4 5 6 7
    Explanation: 4, 5, 6 and 7 are the only 
    elements which is having only 1 
    frequency and hence, Non-repeating.
#### **Example 2:**

    Input:
    n = 5
    arr[] = {10,20,40,30,10}
    Output: 20 40 30
    Explanation: 20, 40, 30 are the only 
    elements which is having only 1 
    frequency and hence, Non-repeating.
#### **Your Task:**
You don't need to read input or print anything. You only need to complete the function printNonRepeated() that takes arr and n as parameters and return the array which has the distinct elements in same order as they appear in input array. The newline is appended automatically by the driver code.

**Expected Time Complexity:** O(n).

**Expected Auxiliary Space:** O(n).

**Constraints:**

1 <= n <= 103
0 <= arri <= 107

#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3
class Solution:
    
    #Complete this function
    #Function to return non-repeated elements in the array.
    def printNonRepeated(self,arr,n):
        #Your code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3


def main():
    T=int(input())
    while(T>0):
        
        n=int(input())
        arr=[int(x) for x in input().strip().split()]
        l = Solution().printNonRepeated(arr,n)
        print(*l)
        
        T-=1

if __name__=="__main__":
    main()
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Non Repeating Character
</Summary>


#### **Non Repeating Character**
**Difficulty Level : Easy**

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 

Given a string S consisting of lowercase Latin Letters. Return the first non-repeating character in S. If there is no non-repeating character, return '$'.

#### **Example 1:**

    Input:
    S = hello
    Output: h
    Explanation: In the given string, the
    first character which is non-repeating
    is h, as it appears first and there is
    no other 'h' in the string.
#### **Example 2:**

    Input:
    S = zxvczbtxyzvy
    Output: c
    Explanation: In the given string, 'c' is
    the character which is non-repeating. 
#### **Your Task:**
You only need to complete the function nonrepeatingCharacter() that takes string S as a parameter and returns the character. If there is no non-repeating character then return '$' .

**Expected Time Complexity:** O(N)

**Expected Auxiliary Space:**O(Number of distinct characters)

Note: N = |S|

**Constraints:**

1 <= N <= 103

#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    
    #Function to find the first non-repeating character in a string.
    def nonrepeatingCharacter(self,s):
        #code here
    
    


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
    for i in range(t):
        s=str(input())
        obj = Solution()
        ans=obj.nonrepeatingCharacter(s)
        if(ans!='$'):
            print(ans)
        else:
            print(-1)
            
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Winner of an election
</Summary>

**Winner of an election** 
**Difficulty Level : Easy**

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 

Given an array of names (consisting of lowercase characters) of candidates in an election. A candidate name in array represents a vote casted to the candidate. Print the name of candidate that received Max votes. If there is tie, print lexicographically smaller name.

#### **Example 1:**

    Input:
    n = 13
    Votes[] = {john,johnny,jackie,johnny,john 
    jackie,jamie,jamie,john,johnny,jamie,
    johnny,john}
    Output: john 4
    Explanation: john has 4 votes casted for 
    him, but so does johny. john is 
    lexicographically smaller, so we print 
    john and the votes he received.
#### **Example 2:**

    Input:
    n = 3
    Votes[] = {andy,blake,clark}
    Output: andy 1
    Explanation: All the candidates get 1 
    votes each. We print andy as it is 
    lexicographically smaller.
#### **Your Task:**
You only need to complete the function winner() that takes an array of strings arr, and n as parameters and returns the name of the candiate with maximum votes and the number of votes the candidate got as an array of size 2.

**Expected Time Complexity:** O(n)

**Expected Auxiliary Space:** O(n)

**Constraints:**

1 <= n <= 105


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    
    #Complete this function
    
    #Function to return the name of candidate that received maximum votes.
    def winner(self,arr,n):
        # Your code here
        # return the name of the winning candidate and the votes he recieved



#{ 
 # Driver Code Starts
#Initial Template for Python 3

if __name__=="__main__":
    T=int(input())
    for _ in range(T):
        
        n=int(input())
        arr=input().strip().split()
        
        result = Solution().winner(arr,n)
        print(result[0],result[1])
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
First Repeating Element
</Summary>

#### **First Repeating Element**
**Difficulty Level : Easy**

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 

Given an array arr[] of size n, find the first repeating element. The element should occur more than once and the index of its first occurrence should be the smallest.

Note:- The position you return should be according to 1-based indexing. 

#### **Example 1:**

    Input:
    n = 7
    arr[] = {1, 5, 3, 4, 3, 5, 6}
    Output: 2
    Explanation: 
    5 is appearing twice and 
    its first appearence is at index 2 
    which is less than 3 whose first 
    occuring index is 3.

#### **Example 2:**

    Input:
    n = 4
    arr[] = {1, 2, 3, 4}
    Output: -1
    Explanation: 
    All elements appear only once so 
    answer is -1.

#### **Your Task:**
You don't need to read input or print anything. Complete the function firstRepeated() which takes arr and n as input parameters and returns the position of the first repeating element. If there is no such element, return -1.
 

**Expected Time Complexity:** O(n)

**Expected Auxilliary Space:** O(n)

 

**Constraints:**

1 <= n <= 106
0 <= Ai<= 106


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    #Function to return the position of the first repeating element.
    def firstRepeated(self,arr, n):
        
        #arr : given array
        #n : size of the array


#{ 
 # Driver Code Starts
#Initial Template for Python 3

#contributed by RavinderSinghPB
if __name__=='__main__':
    t=int(input())
    for _ in range(t):
        n=int(input())
        
        arr=[int(x) for x in input().strip().split()]
        ob = Solution()
        print(ob.firstRepeated(arr, n))
# } Driver Code Ends
```

</details>


</details>