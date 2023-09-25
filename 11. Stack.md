 ### List of Questions
 1. Insert In Stack
2. Implement Stack Using Array
3. Operations on Stack
4. Implement Stack using Linked List
5. Infix to Postfix
6. Prefix to Infix Conversion
7. Postfix to Infix Conversion
8. Removing consecutive duplicates
9. Removing consecutive duplicates - 2
10. Parenthesis Checker

------
## Details of Questions Listed Above

<details>
<summary>
Insert In Stack
</Summary>


### **Insert In Stack**
**Difficulty Level : Basic**

Apply for Mega Job-A-Thon: Fresher Edition | 30+ Opportunities | Avg CTC: 7 LPA  

You are given an array arr[] of size N, the task is to insert the elements of the array into a stack from left to right

#### **Example 1:**

    Input: N = 5, arr[] = {1, 2, 3, 4, 5}
    Output: 5 4 3 2 1
    Explanation: After insert in the stack 
    it will look like {5, 4, 3, 2, 1}.
#### **Example 2:**

    Input: N = 1, arr[] = {1}
    Output: 1
    Explanation: After insert in the stack 
    it will look like {1}.
#### **Your Task:** You don't need to read any input or print anything. Complete the function insertIntoStack() which takes an array size N and array arr[] as parameters and returns a stack.

**Expected Time Complexity:** O(N)

**Expected Auxilliary Space:** O(N)

**Constraints:**

1 ≤ N ≤ 105

#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    def InsertInStack(self,n,arr):
        #code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

#contributed by RavinderSinghPB
if __name__=='__main__':
    tcs=int(input())

    for _ in range(tcs):
        n=int(input())
        arr=[int(x) for x in input().split()]

        stack=Solution().InsertInStack(n,arr)

        while stack:
            print(stack.pop(),end=' ')
        print()

# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Implement Stack Using Array
</Summary>

#### **Implement Stack Using Array**
**Difficulty Level : Easy**

Apply for Mega Job-A-Thon: Fresher Edition | 30+ Opportunities | Avg CTC: 7 LPA  

Implement stack using array

You are given q queries. The queries can be of 3 types:
Query Type:               Operation
               1 x:               Push x
                  2:               Pop the top element
                  3:               display stack from bottom to top in a single line.

The stack here is implemented by an array stack[], and maxSize of the stack is 100000. If a push operation is performed beyond this size, you must print "Stack Full"(without quotes). Similarly, an unsuccessful pop operation should print "Stack Empty"(without quotes).  If a display operation is performed on an empty stack print -1.

#### **Example 1:**

    Input: q[] = {(1, 4), 3, 2, 2, 3}
    Output: 4
            Stack Empty
            -1
    Explanation: push() --> 4
    display() --> 4 gets printed
    pop() --> Pop 4
    pop() --> stack is empty so print Stack 
              Empty
    display() --> stack is empty so print -1
#### **Example 2:**

    Input: q[] = {(1, 3), 3}
    Output: 3
    Explanation: push() --> 3
    display() --> 3 gets printed
#### **Your Task:**
This is a function problem. The input task is performed by the driver code. You need to complete the provided functions. Complete function push() which takes an element as input parameter and pop(), display() functions.

**Expected Time Complexity:** push: O(1), pop: O(1), display: O(N)

**Expected Auxilliary Space:** O(N)

**Constraints:**

1 ≤ Number of Operations ≤ 103


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#{ 
 # Driver Code Starts
#Initial Template for Python 3



stackMax=100000
stack=[-1]*stackMax
top=-1



# } Driver Code Ends
#User function Template for python3

##Complete these functions
def push(data):
    ##Your code here

def pop():
    ##Your code here

        
def display():
    ##Your code here

#{ 
 # Driver Code Starts.



def main():
    global top
    testcases=int(input())
    while(testcases>0):
        top=-1
        queries=int(input())
        while(queries>0):
            
            queryType=input()
            
            if(queryType[0]=='1'):
                
                x=int(queryType[2])
                push(x)
                
            elif(queryType[0]=='2'):
                pop()
            
            else:
                display()
            
            queries-=1
        
        testcases-=1

if __name__=="__main__":
    main()
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Operations on Stack
</Summary>

#### **Operations on Stack**
**Difficulty Level : Basic**

Apply for Mega Job-A-Thon: Fresher Edition | 30+ Opportunities | Avg CTC: 7 LPA  

Given a stack of integers and Q queries. The task is to perform the operation on stack according to the query.

The queries can be of 4 types:

i x: (adds element x in the stack).

r: (removes the topmost element from the stack).

h: Prints the topmost element.

f y: (check if the element y is present or not in the stack). Print "Yes" if present, else "No".
 

#### **Example 1:**

    Input: 
    Q = 6 
    Queries = {(i, 2), (i, 4), (i, 3),
    (i, 5), (h), (f, 8)}
    Output: 
    5
    No
    Explanation: 
    Inserting 2, 4, 3, and 5 
    onto the stack. Returning top element 
    which is 5. Finding 8 will give No, 
    as 8 is not in the stack.
 

#### **Example 2:**

    Input: 
    Q = 4
    Queries = {(i, 3), (i, 4), (r), (f, 3)}
    Output: 
    Yes
    Explanation: 
    Inserting 3 and 4 onto the 
    stack. Finding 3 will give Yes as output 
    because 3 is available in the stack.
 

#### **Your Task:**
Your task is to complete functions insert(), remove(), headOf_Stack() which takes a stack as input parameter, and find() which takes a stack and value as input parameter, to insert, remove returning top element, and finding the element in stack respectively.

 

**Expected Time Complexity:**
For find(): O(N),
For others: O(1).

**Expected Auxiliary Space:** O(1).

**Constraints:**
1 ≤ Number of queries ≤ 103


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3


#Function to push an element into the stack.
def insert(stack,x):
    # code here

#Function to remove top element from stack.
def remove(stack):
    #code here
    
#Function to print the top element of stack.    
def headOf_Stack(stack):
    #code here
    
#Function to search an element in the stack.
def find(stack,x):
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
        a = list(map(str,input().strip().split()))
        stack = [] # our stack to be implemented
        i = 0 #current index
        while i < len(a):
            if a[i]=='i':
                insert(stack,a[i+1])
                i+=1
            elif a[i] == 'f' :
                if(find(stack,a[i+1])):
                    print("Yes")
                else:
                    print("No")
                i+=1
            elif a[i] == 'r' :
                (remove(stack))
            else:
                print(headOf_Stack(stack))
            i+=1
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Implement Stack using Linked List
</Summary>

**Implement Stack using Linked List**
**Difficulty Level : Basic**

Apply for Mega Job-A-Thon: Fresher Edition | 30+ Opportunities | Avg CTC: 7 LPA  

Let's give it a try! You have a linked list and you have to implement the functionalities push and pop of stack using this given linked list. Your task is to use the class as shown in the comments in the code editor and complete the functions push() and pop() to implement a stack. 

#### **Example 1:**

    Input: 
    push(2)
    push(3)
    pop()
    push(4) 
    pop()
    Output: 3 4
    Explanation: 
    push(2)    the stack will be {2}
    push(3)    the stack will be {2 3}
    pop()      poped element will be 3,
               the stack will be {2}
    push(4)    the stack will be {2 4}
    pop()      poped element will be 4
#### **Example 2:**

    Input: 
    pop()
    push(4)
    push(5)
    pop()
    Output: -1 5
#### **Your Task:** You are required to complete two methods push() and pop(). The push() method takes one argument, an integer 'x' to be pushed into the stack and pop() which returns an integer present at the top and popped out from the stack. If the stack is empty then return -1 from the pop() method.

**Expected Time Complexity:** O(1) for both push() and pop().

**Expected Auxiliary Space:** O(1) for both push() and pop().

**Constraints:**

1 <= Q <= 100
1 <= x <= 100


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
class MyStack:


    # class StackNode:

    # # Constructor to initialize a node
    # def __init__(self, data):
    #     self.data = data
    #     self.next = None
        
    #Function to push an integer into the stack.
    def push(self, data):

        # Add code here


    #Function to remove an item from top of the stack.
    def pop(self):

        # Add code here



#{ 
 # Driver Code Starts


class StackNode:

    # Constructor to initialize a node
    def __init__(self, data):
        self.data = data
        self.next = None


if __name__ == '__main__':
    t = int(input())
    for i in range(t):
        s = MyStack()
        q = int(input())
        q1 = list(map(int, input().split()))
        i = 0
        while(i < len(q1)):
            if(q1[i] == 1):
                s.push(q1[i + 1])
                i = i + 2
            elif(q1[i] == 2):
                print(s.pop(), end=" ")
                i = i + 1
            elif(s.isEmpty()):
                print(-1)
        print()

# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Infix to Postfix
</Summary>

### **Infix to Postfix**
**Difficulty Level : Medium**

Apply for Mega Job-A-Thon: Fresher Edition | 30+ Opportunities | Avg CTC: 7 LPA  

Given an infix expression in the form of string str. Convert this infix expression to postfix expression.

Infix expression: The expression of the form a op b. When an operator is in-between every pair of operands.
Postfix expression: The expression of the form a b op. When an operator is followed for every pair of operands.
Note: The order of precedence is: ^ greater than * equals to / greater than + equals to -. 
#### **Example 1:**

    Input: str = "a+b*(c^d-e)^(f+g*h)-i"
    Output: abcd^e-fgh*+^*+i-
    Explanation:
    After converting the infix expression 
    into postfix expression, the resultant 
    expression will be abcd^e-fgh*+^*+i-
#### **Example 2:**

    Input: str = "A*(B+C)/D"
    Output: ABC+*D/
    Explanation:
    After converting the infix expression 
    into postfix expression, the resultant 
    expression will be ABC+*D/
 
#### **Your Task:**
This is a function problem. You only need to complete the function infixToPostfix() that takes a string(Infix Expression) as a parameter and returns a string(postfix expression). The printing is done automatically by the driver code.

**Expected Time Complexity:** O(|str|).

**Expected Auxiliary Space:** O(|str|).

**Constraints:**

1 ≤ |str| ≤ 105


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3


class Solution:
    
    #Function to convert an infix expression to a postfix expression.
    def InfixtoPostfix(self, exp):
        #code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

import atexit
import io
import sys

# This code is contributed by Nikhil Kumar Singh(nickzuck_007)


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
        exp = str(input())
        ob=Solution()
        print(ob.InfixtoPostfix(exp))
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Prefix to Infix Conversion
</Summary>


### **Prefix to Infix Conversion**
**Difficulty Level : Medium**

Apply for Mega Job-A-Thon: Fresher Edition | 30+ Opportunities | Avg CTC: 7 LPA  

You are given a string S of size N that represents the prefix form of a valid mathematical expression. Convert it to its infix form.

#### **Example 1:**

    Input: 
    *-A/BC-/AKL
    Output: 
    ((A-(B/C))*((A/K)-L))
    Explanation: 
    The above output is its valid infix form.
#### **Your Task:**

Complete the function string preToInfix(string pre_exp), which takes a prefix string as input and return its infix form.

 

**Expected Time Complexity:** O(N).

**Expected Auxiliary Space:** O(N).

**Constraints:**

3<=|S|<=104

#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#{ 
 # Driver Code Starts
#Initial Template for Python 3

# } Driver Code Ends
#User function Template for python3

class Solution:
    def preToInfix(self, pre_exp):
        # Code here

#{ 
 # Driver Code Starts.
if __name__ == '__main__': 
    t = int(input ())
    for _ in range (t):
        prefix = input()
        ob = Solution()
        res = ob.preToInfix(prefix)
        print(res)
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Postfix to Infix Conversion
</Summary>

### **Postfix to Infix Conversion**
**Difficulty Level : Medium**

Apply for Mega Job-A-Thon: Fresher Edition | 30+ Opportunities | Avg CTC: 7 LPA  

You are given a string that represents the postfix form of a valid mathematical expression. Convert it to its infix form.

#### **Example:**

    Input:
    ab*c+ 
    Output: 
    ((a*b)+c)
    Explanation: 
    The above output is its valid infix form.
#### **Your Task:**

Complete the function string postToInfix(string post_exp), which takes a postfix string as input and returns its infix form.

 

**Expected Time Complexity:** O(N).

**Expected Auxiliary Space:** O(N).

**Constraints:**

3<=post_exp.length()<=104



#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#{ 
 # Driver Code Starts
#Initial Template for Python 3

# } Driver Code Ends
#User function Template for python3

class Solution:
    def postToInfix(self, postfix):
        # Code here

#{ 
 # Driver Code Starts.
if __name__ == '__main__': 
    t = int(input ())
    for _ in range (t):
        postfix = input()
        ob = Solution()
        res = ob.postToInfix(postfix)
        print(res)
# } Driver Code Ends
```

</details>


</details>


<details>
<summary>
Removing consecutive duplicates
</Summary>

### **Removing consecutive duplicates**
**Difficulty Level : Easy**

Apply for Mega Job-A-Thon: Fresher Edition | 30+ Opportunities | Avg CTC: 7 LPA  

You are given string str. You need to remove the consecutive duplicates from the given string using a Stack.
 

#### **Example 1:**

    Input: 
    aaaaaabaabccccccc
    
    Output: 
    ababc
    
    Explanation: 
    The order is in the following way 6->a, 1->b, 2->a, 1->b, 7->c. 
    So, only one element from each group will remain and rest all are removed.
    Therefore, final string will be:- ababc.

#### **Example 2:**

    Input: 
    abbccbcd
    
    Output: 
    abcbcd
    
    Explanation: 
    The order is in the following way 1->a, 2->b, 2->c, 1->b, 1->c, 1->d.
    So, only one element from each group will remain and rest all are removed.
    Therefore, final string will be:- abcbcd. 
#### **Your Task:**
This is a function problem. You need to complete the function removeConsecutiveDuplicates() that takes a string as a parameter and returns the modified string. The printing is done automatically by the driver code.

**Expected Time Complexity:** O(N).

**Expected Auxiliary Space:** O(N).

**Constraints:**

1 <= |str| <= 103


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    
    #Function to remove consecutive duplicates from given string using Stack.
    def removeConsecutiveDuplicates(self,s):
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
        obj = Solution()
        print(obj.removeConsecutiveDuplicates(str(input())))
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Removing consecutive duplicates - 2
</Summary>


### **Removing consecutive duplicates - 2**
**Difficulty Level : Easy**

Apply for Mega Job-A-Thon: Fresher Edition | 30+ Opportunities | Avg CTC: 7 LPA  

You are given string str. You need to remove the pair of duplicates.
Note: The pair should be of adjacent elements and after removing a pair the remaining string is joined together. 

#### **Example 1:**

    Input:
    aaabbaaccd
    
    Output: 
    ad
    
    Explanation: 
    Remove (aa)abbaaccd =>abbaaccd
    Remove a(bb)aaccd => aaaccd
    Remove (aa)accd => accd
    Remove a(cc)d => ad
#### **Example 2:**

    Input: 
    aaaa
    
    Output: 
    Empty String
    
    Explanation: 
    Remove (aa)aa => aa
    Again removing pair of duplicates then (aa) 
    will be removed and we will get 'Empty String'.

#### **Your Task:**
This is a function problem. You only need to complete the function removePair() that takes a string as a parameter and returns the modified string. Return an empty string if the whole string is deleted.

**Expected Time Complexity:** O(N).

**Expected Auxiliary Space:** O(N).
N = length of the string.

**Constraints:**

1 <= |str| <= 103

#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python

#User function Template for python3

class Solution:
    
    #Function to remove pair of duplicates from given string using Stack.
    def removePair(self,s):
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
        obj = Solution()
        print(obj.removePair(str(input())))
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Parenthesis Checker
</Summary>

### **Parenthesis Checker**
**Difficulty Level : Easy**

Apply for Mega Job-A-Thon: Fresher Edition | 30+ Opportunities | Avg CTC: 7 LPA  

Given an expression string x. Examine whether the pairs and the orders of {,},(,),[,] are correct in exp.
For example, the function should return 'true' for exp = [()]{}{[()()]()} and 'false' for exp = [(]).

Note: The drive code prints "balanced" if function return true, otherwise it prints "not balanced".

#### **Example 1:**

    Input:
    {([])}
    Output: 
    true
    Explanation: 
    { ( [ ] ) }. Same colored brackets can form 
    balanced pairs, with 0 number of 
    unbalanced bracket.
#### **Example 2:**

    Input: 
    ()
    Output: 
    true
    Explanation: 
    (). Same bracket can form balanced pairs, 
    and here only 1 type of bracket is 
    present and in balanced way.
#### **Example 3:**

    Input: 
    ([]
    Output: 
    false
    Explanation: 
    ([]. Here square bracket is balanced but 
    the small bracket is not balanced and 
    Hence , the output will be unbalanced.
#### **Your Task:**
This is a function problem. You only need to complete the function ispar() that takes a string as a parameter and returns a boolean value true if brackets are balanced else returns false. The printing is done automatically by the driver code.

**Expected Time Complexity:** O(|x|)

**Expected Auixilliary Space:** O(|x|)

**Constraints:**

1 ≤ |x| ≤ 32000


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    
    #Function to check if brackets are balanced or not.
    def ispar(self,x):
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
        #n = int(input())
        #n,k = map(int,imput().strip().split())
        #a = list(map(int,input().strip().split()))
        s = str(input())
        obj = Solution()
        if obj.ispar(s):
            print("balanced")
        else:
            print("not balanced")
# } Driver Code Ends
```

</details>


</details>


