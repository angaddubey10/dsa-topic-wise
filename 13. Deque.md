## List of Questions
1. Implement Dequeue Using Linked List
2. Deque Implementations
3. Insertion in deque
4. Dequeue Traversal
5. Deque deletion

-----
<details>
<summary>
Implement Dequeue Using Linked List
</Summary>

### **Implement Dequeue Using Linked List**
**Difficulty Level : basic** 

Apply for Mega Job-A-Thon: Fresher Edition | 30+ Opportunities | Avg CTC: 3-15 LPA  

You are given a dequeue and q queries. The queries can be of 4 types:

    ir x: Use insertRear to insert data x in dequeue.
    if x: Use insertFront to insert data x in dequeue.
    df: Use deleteFront to delete the front of dequeue. If dequeue is empty then don't do anything.
    dr: Use deleteRear to delete the rear of dequeue. If dequeue is empty then don't do anything.
#### **Example 1:**

    Input: q = 4, queries[] = {(ir, 5), 
        (if, 7), (df), (if, 22)}
    Output: 22
            5
    Explanation: Here q = 4. First we insert 5 
    at the back. Now we insert 7 in the front. 
    The dequeue is now {7, 5}. Now we remove 
    the front, so dequeue is now {5}. Now, we 
    insert 22 in the front. The dequeue is now
    {22, 5}. So the front is 22 and the rear 
    is 5.

#### **Example 2:**

    Input: q = 1, queries[] = {(ir, 8)} 
    Output: 8
    Explanation: Insert 8 in back, so front 
    and rear elements are same, which is 8.
#### **Your Task:** This is a function problem. You only need to complete the given functions insertFront(),  insertRear(), deleteFront(), deleteRear(). The printing at the end is done by the driver code.

**Expected Time Complexity:** O(1) for all operations.

**Expected Auxilliary Space:** O(N)

**Constraints:**

1 ≤ Number of queries ≤ 105


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

'''
class Node:
    def __init__(self,data):
        self.data=data
        self.next=None
        self.prev=None

class Deque:
    def __init__(self):
        self.front=None
        self.rear=None
        
        
given front and rear of deque in every operation,
return updated front and rear in each operation
'''


def insertFront(front,rear,data):
    # return: (front, rear)
    #code here
    
    
def insertRear(front,rear,data):
    # return: (front,rear)
    #code here
    

def delFront(front,rear):
    # return: (front, rear)
    #code here
    
    
def delRear(front,rear):
    # return: (front, rear)
    #code here


#{ 
 # Driver Code Starts
#contributed by RavinderSinghPB
class Node:
    def __init__(self,data):
        self.data=data
        self.next=None
        self.prev=None

class Deque:
    def __init__(self):
        self.front=None
        self.rear=None





if __name__=='__main__':
    tcs=int(input())

    for _ in range(tcs):
        q=int(input())

        dq=Deque()

        for _ in range(q):

            qry=input().split()

            if qry[0]=='if':
                x=int(qry[1])
                dq.front,dq.rear=insertFront(dq.front,dq.rear,x)

            elif qry[0]=='ir':
                x=int(qry[1])
                dq.front,dq.rear=insertRear(dq.front,dq.rear,x)

            elif qry[0]=='df':
                dq.front,dq.rear=delFront(dq.front,dq.rear)

            else: #dr
                dq.front,dq.rear=delRear(dq.front,dq.rear)


        if dq.front:
            print(dq.front.data)
            print(dq.rear.data)
        else:
            print(-1)
            print(-1)





# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Deque Implementations
</Summary>


### **Deque Implementations**
**Difficulty Level : Easy** 

Apply for Mega Job-A-Thon: Fresher Edition | 30+ Opportunities | Avg CTC: 3-15 LPA  

A deque is a double-ended queue that allows enqueue and dequeue operations from both the ends.

Given a deque and Q queries. The task is to perform some operation on dequeue according to the queries as given below:
1. pb: query to push back the element x.
2. pf: query to push element x(given with query) to the front of the deque.
3. pp_b(): query to delete element from the back of the deque.
4. f: query to return a front element from the deque.

#### **Example 1:**

    Input:
    5
    pf 5
    pf 10
    pb 6
    f
    pp_b
    
    Output: 
    10
    
    Explanation: 
       1. After push front deque will be {5}
       2. After push front deque will be {10, 5}
       3. After push back deque will be {10, 5, 6}
       4. Return front element which is 10
       5. After pop back deque will be {10, 5}

#### **Example 2:**

    Input: 
    2
    pf 5 
    f
    
    Output: 
    5 
    
    Explanation:
       1. After push front deque will be {5}
       2. Return front element which is 5
   #### **Your Task:**
   Your task is to complete the following functions:
   push_back_pb(): Push back the given element and then driver code prints that element.
   push_front_pf(): Push front the given element and then driver code prints that element.
   pop_back_ppb(): Pop the back element (if exists) and then the driver code prints the size of the deque.
   front_dq(): Return the front elements if it exists, else return -1. The driver code prints the return value.

**Expected Time Complexity:** O(1)

**Expected Auxilliary Space:** O(1)

**Constraints:**

1 ≤ Number of queries ≤ 105

*Note: Ouput is also printed after every method call, see the driver code.

#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3


#dq : deque in which element is to be pushed
#x : element to be pushed


#Function to push element x to the front of the deque.
def push_front_pf(dq,x):
    #code here
    

#Function to push element x to the back of the deque.
def push_back_pb(dq,x):
    #code here
    
#Function to return element from front of the deque.
def front_dq(dq):
    #code here
    
#Function to pop element from back of the deque.
def pop_back_ppb(dq):
    #code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

#contributed by RavinderSinghPB
if __name__=='__main__':
    from collections import deque

    tcs=int(input())

    for _ in range(tcs):

        dq=deque()

        n=int(input())

        for _ in range(n):
            qry=input().split()

            if qry[0]=='pf':
                x=int(qry[1])
                push_front_pf(dq,x)
                print(dq[0])

            elif qry[0]=='pb':
                x=int(qry[1])
                push_back_pb(dq,x)
                print(dq[-1])

            elif qry[0]=='pp_b':
                pop_back_ppb(dq)
                print(len(dq))

            else:
                x=front_dq(dq)
                print(x)

# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Insertion in deque
</Summary>

### **Insertion in deque**
**Difficulty Level : Basic** 

Apply for Mega Job-A-Thon: Fresher Edition | 30+ Opportunities | Avg CTC: 3-15 LPA  

Given an array arr[] of size N containing non-negative integers. You need to insert all elements of the array to deque and return it.

#### **Example 1:**

    Input: 
    5
    1 2 3 4 5
    
    Output: 
    1 2 3 4 5
    
    Explanation: 
    After insert in the deque 
    it will look like {1, 2, 3, 4, 5}.
#### **Example 2:**

    Input:
    1
    1
    
    Output: 
    1
    
    Explanation: 
    After insert in the deque 
    it will look like {1}.
#### **Your Task:**
You need to complete the function deque_Init() which takes array arr[] and it's size N as input parameters and should return deque that contains array elements. You don't have to worry about input.

**Expected Time Complexity:** O(N)

**Expected Auxilliary Space:** O(1)

**Constraints:**

1 ≤ N ≤ 105


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    
    #Function to insert all elements of the array in deque.
    def deque_Init(self,arr,n):
        #code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

#contributed by RavinderSinghPB
if __name__ == '__main__':

    from collections import deque

    tcs= int(input())

    for _ in range(tcs):
        n=int(input())
        arr=[int(x) for x in input().split()]
        ob=Solution()
        dq=ob.deque_Init(arr,n)

        for e in dq:
            print(e,end=' ')
        print()
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Dequeue Traversal
</Summary>

#### **Dequeue Traversal**
**Difficulty Level : Basic** 

Apply for Mega Job-A-Thon: Fresher Edition | 30+ Opportunities | Avg CTC: 3-15 LPA  

Given a Deque Deq containing N elements, the task is to traverse the Deq and print its elements of it. 

#### **Example 1:**

    Input: 
    5
    1 2 3 4 5
    
    Output: 
    1 2 3 4 5
    
    Explanation: 
    Dqe will look like 
    {1, 2, 3, 4, 5}.
#### **Example 2:**

    Input:
    1
    1
    
    Output: 
    1
    
    Explanation: 
    Dqe will look like {1}.
#### **Your task:** You don't have to worry about the input. You just have to complete the function printDeque() which takes a Deque as an input parameter and prints all its elements of it.
Note: The output must be printed on different lines for multiple test cases.

**Expected Time Complexity:** O(N)

 **Expected Auxilliary Space:** O(1)

**Constraints:**

1 ≤ N ≤ 105


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3


#Function to traverse the Deque and print the elements of it.
def printDeque(deq):
    #CODE HERE


#{ 
 # Driver Code Starts
#Initial Template for Python 3

#contributed by RavinderSinghPB
if __name__ == '__main__':

    from collections import deque

    tcs= int(input())

    for _ in range(tcs):
        n=int(input())
        arr=[int(x) for x in input().split()]

        deq=deque(arr)

        printDeque(deq)

# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Deque deletion
</Summary>

### **Deque deletion**
**Difficulty Level : Basic** 

Apply for Mega Job-A-Thon: Fresher Edition | 30+ Opportunities | Avg CTC: 3-15 LPA  

Given a Deque dqe of size N containing non-negative integers.

Complete below functions depending type of query as mentioned and provided to you (indexing starts from 0):
1. eraseAt(X): this function should remove the element from specified position X in deque.
2. eraseInRange(start, end): this function should remove the elements in range start (inclusive), end (exclusive) specified in the argument of the function.
Note: If start is equal to end then simply return.
3. eraseAll(): remove all the elements from the deque.

#### **Example 1:**

    Input:
    5
    1 2 4 5 6
    1 2
    
    Output: 
    1 2 5 6 
    
    Explanation: 
    Here the query type is 1 
    and the position is 2. So we remove 
    element at position 2. The element at 
    position 2 is 1 2 4 5 6. So, we remove 
    4 and get 1 2 5 6.
#### **Example 2:**

    Input: 
    4
    1 2 3 4
    2 1 3
    
    Output: 
    1 4 
    
    Explanation: 
    Here the query type is 2 
    and the range is [1, 3). So we need to 
    delete 1 2 3 4. Remember that end is 
    exclusive. So the updated dequeue is 1 4.
#### **Example 3:**

    Input:
    3
    1 2 3
    3
    
    Output: 
    Empty
    
    Explanation: 
    Here the query is of type 3 
    so we remove all the elements of dequeue.
#### **Your Task:**
Complete the functions eraseAt() which takes dequeue and a postion as input parameters, eraseInRange() which takes dequeue, start(inclusive) and end(exclusive) as input parameters and eraseAll() which takes a dequeue as input parameter.

**Expected Time Complexity:** O(N), for all operations

**Expected Auxilliary Space:** O(1)

**Constraints:**

1 ≤ N ≤ 105


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

#Function to erase the element from specified position X in deque.
def eraseAt(deq,x):
    #code here
    
#Function to erase the elements in range start (inclusive), end (exclusive).
def eraseInRange(deq,s,e):
    #code here

#Function to erase all the elements in the deque.   
def eraseAll(deq):
    #code here
    


#{ 
 # Driver Code Starts
#Initial Template for Python 3

#contributed by RavinderSinghPB
if __name__ == '__main__':

    from collections import deque

    tcs= int(input())

    for _ in range(tcs):
        n=int(input())
        arr=[int(x) for x in input().split()]

        qry=input().split()

        deq=deque(arr)

        if int(qry[0])==1:
            
            x=int(qry[1])
            eraseAt(deq,x)

        elif int(qry[0])==2:
            
            start,end=int(qry[1]),int(qry[2])
            eraseInRange(deq,start,end)

        else:
            eraseAll(deq)

        if not deq:
            print('Empty')
        else:
            print(*deq)



# } Driver Code Ends
```

</details>


</details>

