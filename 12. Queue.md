## List of Questions
1. Implement Queue using array
2. Implement Queue using Linked List
3. Operations on Queue

----

<details>
<summary>
Implement Queue using array
</Summary>

### **Implement Queue using array**
**Difficulty Level : basic** 

Apply for Mega Job-A-Thon: Fresher Edition | 30+ Opportunities | Avg CTC: 3-15 LPA  

Implement a Queue using an Array. Queries in the Queue are of the following type:
(i) 1 x   (a query of this type means  pushing 'x' into the queue)
(ii) 2     (a query of this type means to pop element from queue and print the poped element)

#### **Example 1:**

    Input:
    Q = 5
    Queries = 1 2 1 3 2 1 4 2
    Output: 2 3
    Explanation:
    In the first test case for query 
    1 2 the queue will be {2}
    1 3 the queue will be {2 3}
    2   poped element will be 2 the 
        queue will be {3}
    1 4 the queue will be {3 4}
    2   poped element will be 3 
#### **Example 2:**

    Input:
    Q = 4
    Queries = 1 3 2 2 1 4   
    Output: 3 -1
    Explanation:
    In the second testcase for query 
    1 3 the queue will be {3}
    2   poped element will be 3 the
        queue will be empty
    2   there is no element in the
        queue and hence -1
    1 4 the queue will be {4}. 
#### **Your Task :**
You are required to complete the two methods push() which take one argument an integer 'x' to be pushed into the queue and pop() which returns a integer poped out from othe queue. If the queue is empty, it should return -1 on a pop operation. 

**Expected Time Complexity:** O(1) for both push() and pop().

**Expected Auxiliary Space:** O(1) for both push() and pop().

**Constraints:**

1 ≤ Q ≤ 105
1 ≤ x ≤ 105


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class MyQueue:
    
    #Function to push an element x in a queue.
    def push(self, x):
         
         #add code here
     
    #Function to pop an element from queue and return that element.
    def pop(self): 
         
         # add code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

if __name__=='__main__':
    t=int(input())
    for i in range(t):
        s=MyQueue()
        q=int(input())
        q1=list(map(int,input().split()))
        i=0
        while(i<len(q1)):
            if(q1[i]==1):
                s.push(q1[i+1])
                i=i+2
            elif(q1[i]==2):
                print(s.pop(),end=" ")
                i=i+1
            elif(s.isEmpty()):
                print(-1)
                i=i+1
        print()   

# } Driver Code Ends
```

</details>

</details>

<details>
<summary>
Implement Queue using Linked List
</Summary>


### **Implement Queue using Linked List**
**Difficulty Level : basic** 

Apply for Mega Job-A-Thon: Fresher Edition | 30+ Opportunities | Avg CTC: 3-15 LPA  

Implement a Queue using Linked List. 
A Query Q is of 2 Types
(i) 1 x   (a query of this type means  pushing 'x' into the queue)
(ii) 2     (a query of this type means to pop an element from the queue and print the poped element)

#### **Example 1:**

    Input:
    Q = 5
    Queries = 1 2 1 3 2 1 4 2
    Output: 2 3
    Explanation: n the first testcase
    1 2 the queue will be {2}
    1 3 the queue will be {2 3}
    2   poped element will be 2 the
        queue will be {3}
    1 4 the queue will be {3 4}
    2   poped element will be 3.

#### **Example 2:**

    Input:
    Q = 4
    Queries = 1 2 2 2 1 3 
    Output: 2 -1
    Explanation: In the second testcase 
    1 2 the queue will be {2}
    2   poped element will be {2} then
        the queue will be empty. 
    2   the queue is empty and hence -1
    1 3 the queue will be {3}.
#### **Your Task:**
Complete the function push() which takes an integer as input parameter and pop() which will remove and return an element(-1 if queue is empty).

**Expected Time Complexity:** O(1).

**Expected Auxiliary Space:** O(1).

**Constraints:**

1 <= Q <= 100
1 <= x <= 100

#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
# A linked list (LL) node 
# to store a queue entry 
'''class Node: 
      
    def __init__(self, data): 
        self.data = data 
        self.next = None'''
        
class MyQueue:
    
    #Function to push an element into the queue.
    def push(self, item): 
         
         #Add code here
    
    #Function to pop front element from the queue.
    def pop(self):
         
         #add code here


#{ 
 # Driver Code Starts
if __name__=='__main__':
    t=int(input())
    for i in range(t):
        s=MyQueue()
        q=int(input())
        q1=list(map(int,input().split()))
        i=0
        while(i<len(q1)):
            if(q1[i]==1):
                s.push(q1[i+1])
                i=i+2
            elif(q1[i]==2):
                print(s.pop(),end=" ")
                i=i+1
            elif(s.isEmpty()):
                print(-1)
                i=i+1
        print()   
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Operations on Queue
</Summary>

### **Operations on Queue**
**Difficulty Level : basic** 

Apply for Mega Job-A-Thon: Fresher Edition | 30+ Opportunities | Avg CTC: 3-15 LPA  

Given a queue of integers and Q queries. The task is to perform operations on queue according to the query. 

Queries are as:

i x : (adds element x in the queue from rear).

r : (Removes the front element of queue).

h : (Returns the front element).

f y : (check if the element y is present or not in the queue). Return "Yes" if present, else "No".

#### **Example 1:**

    Input:
    Q = 6
    Queries = i 2 i 4 i 3 i 5 h f 8
    Output:
    2
    No
    Explanation: Inserting 2, 4, 3, and 5
    onto the queue: 2 4 3 5. h means front
    So front is 2. f is find. 8 is not in
    queue so No.
#### **Example 2:**

    Input:
    Q = 4
    Queries = i 3 i 4 r f 3
    Output: No
    Explanation: Inserting 3 and 4 . When
    we return and remove 3 and then when
    we find 3 , it will return NO as
    output as 3 is not present in the
    queue.
#### **Your Task:**
Your task is to complete functions enqueue(), dequeue(), front() and find() which performs the operations described above in the problem description.

**Expected Time Complexity:** O(1) for enqueue(), dequeue() and front(); O(N) for find().

**Expected Auxiliary Space:** O(1) for all the 4 functions. 

**Constraints:**

1 <= Q <= 103




#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    '''
    Function Arguments :
    		@param  : q (given list on which queue is implemented)
    		@param  : x (value to be used accordingly)
    		@return : None
    '''
    
    #Function to push an element in queue.
    def enqueue(self,q, x):
        # code here
    
    #Function to remove front element from queue.
    def dequeue(self,q):
        # code here
    
    #Function to find the front element of queue.
    def front(self,q):
        # code here
    
    #Function to find an element in the queue.
    def find(self,q, x):
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
        a = list(map(str,input().strip().split()))
        queue = [] # our queue to be implemented
        ob=Solution()
        i = 0 #current index
        while i < len(a):
            if a[i]=='i':
                ob.enqueue(queue,a[i+1])
                i+=1
            elif a[i] == 'f' :
                if(ob.find(queue,a[i+1])):
                    print("Yes")
                else:
                    print("No")
                i+=1
            elif a[i] == 'r' :
                (ob.dequeue(queue))
            else:
                print(ob.front(queue))
            i+=1
# } Driver Code Ends
```

</details>


</details>

