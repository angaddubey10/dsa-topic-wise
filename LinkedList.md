### List of Questions
1. Display Linked List
2. Count nodes of linked list |--| [GFG](https://practice.geeksforgeeks.org/problems/count-nodes-of-linked-list/1)
3. Sum The Nodes of Linked List
4. Search In Linked List
5. Linked List Insertion
6. Linked List Insertion At Position
7. Delete Head of Linked List
8. Delete Tail of Linked List
9. Linked List Delete at Position
10. Insert In Sorted Linked List
11. Insert in Middle of Linked List
12. Is Linked List Sorted
13. Nth node from end of linked list
14. Join Two Linked Lists
15. Remove duplicate element from sorted Linked List
16. Reverse a linked list[LeetCode](https://leetcode.com/problems/reverse-linked-list/)
17. Maximum And Minimum In Linked List
18. Identical Linked Lists


-----

## Details of Questions Listed Above

<details>
<summary>1.Display Linked List</summary>

### **Display Linked List**
**Difficulty Level : Basic** 

Given a singly linked list of integers.the task is to dispLay the linked list

#### **Example 1:**
     Input:
     linkedlist 1->2->3->4->5
     Output: 1 2 3 4 5

**Constraints:**

1 <= Number of nodes <= 100

0 <= value of nodes<= 103

#### **Your Task:**
your task is to complete the given function displayList(), which takes head reference as argument and return the linkedlist as an array.

**Expected Time Complexity:** O(N).

**Expected Auxiliary Space:** O(1).

#### **Python Code Template**

<details>
<summary>Python Code Template</summary>

```python
#User function Template for python3

'''
class Node:
    def __init__(self,data):
        self.data=data
        self.next=None
'''
def displayList(head):
    #code here
    


#{ 
 # Driver Code Starts
#Initial Template for Python 3

import io
import sys

    
# Node class
class Node:
    def __init__(self,data):
        self.data=data
        self.next=None
#Linked list class
class LinkedList:
    def __init__(self):
        self.head=None
        self.tail=None

    # append at the end of the list
    def append(self,new_node):
        if self.head is None:
            self.head=new_node
            self.tail=new_node
            return
        self.tail.next=new_node
        self.tail = self.tail.next

if __name__ == '__main__':
    t=int(input())
    for cases in range(t):
        n=int(input())
        a=LinkedList()
        nodes=list(map(int,input().strip().split())) #list containing nodes
        for x in nodes:
            node=Node(x) # create a new node
            a.append(node)
        l = displayList (a.head)
        for x in l:
            print(x,end=' ')
        print () 
# } Driver Code Ends


```
</details>


</details>


<details>
<summary>2.Count nodes of linked list</summary>

### **Count nodes of linked list**
**Difficulty Level : Basic** 

Given a singly linked list. The task is to find the length of the linked list, where length is defined as the number of nodes in the linked list.

#### **Example 1**
    Input:
    linkedlist 1->2->3->4->5
    Output:5
    Explanation: Count of nodes in the linkedlist is 5, which is its length
        

#### **Example 2**
    Input: 
    linkedlist 2->4->6->7->5->1->0
    output:7
    Explanation: Count of nodes in the linked list is 7. Hence, the output is 7

#### **Your task:**
Your task is to complete the given function getCount(), which takes a head reference as an argument and should return the length of the linked list.
 

**Expected Time Complexity : O(N)**

**Expected Auxilliary Space : O(1)**

**Constraints:**

1 <= N <= 105


1 <= value <= 103

</details>



<details>
<summary>3.Sum The Nodes of Linked List</summary>


### **Sum The Nodes of Linked List**
**Difficulty Level : Basic** 



Given a singly linked list of size N. The task is to sum the elements of the linked list.

#### **Example 1**
    Input:
    linkedlist 1->2->3->4->5
    output:15

#### **Example 2**
     Input:
     linkedlist 2->4->6->7->1->0
     output: 25

#### **Your Task**
Your task is to complete the given function sumOfElements(), which takes head reference as argument and should return the sum of all the nodes in the Linked List. 

#### **Constraints:**
1 <= n <= 100

1 <= value <= 103

**Expected Time Complexity: O(N).**

**Expected Auxiliary Space: O(1).**

#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

'''
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None
'''

def sumOfElements(head):
    #code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

import io
import sys

    
# Node class
class Node:
    def __init__(self,data):
        self.data=data
        self.next=None
#Linked list class
class LinkedList:
    def __init__(self):
        self.head=None
        self.tail=None

    # append at the end of the list
    def append(self,new_node):
        if self.head is None:
            self.head=new_node
            self.tail=new_node
            return
        self.tail.next=new_node
        self.tail = self.tail.next

if __name__ == '__main__':
    t=int(input())
    for cases in range(t):
        n=int(input())
        a=LinkedList()
        nodes=list(map(int,input().strip().split())) #list containing nodes
        for x in nodes:
            node=Node(x) # create a new node
            a.append(node)
        print(sumOfElements(a.head))
# } Driver Code Ends
```

</details>


</details>


<details>
<summary>
4.Search In Linked List
</Summary>

### Search In Linked List
**Difficulty Level : Basic**

Done with this problem? Now use these skills to apply for a job in Job-A-Thon 20!
You are given a singly linked list of N elements, and also an element x. You need to find if x is present in the linked list or not.

#### **Example 1:**
    Input:
    LinkedList: 1->2->3->4->5
    x = 4
    Output: 1

#### **Example 2:**
    Input:
    LinkedList: 2->4->6->7->5->1->0
    x = 10
    Output: 0

#### **Your Task:**
Your task is to complete the given function searchLinkedList() which takes head reference and x as arguments and returns true if x is present else returns false. (1 is printed by the driver code if the returned value is true, otherwise 0)

**Constraints:**

1 <= n <= 100

1 <= x, value <= 103

**Expected Time Complexity:** O(N).

**Expected Auxiliary Space:** O(1).


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python

#User function Template for python3

'''
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None
'''
def searchLinkedList(head,x):
    #code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

# contributed by RavinderSinghPB
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None


class Llist:
    def __init__(self):
        self.head = None

    def insert(self, data, tail):
        node = Node(data)

        if not self.head:
            self.head = node
            return node

        tail.next = node
        return node


if __name__ == '__main__':
    t = int(input())

    for tcs in range(t):

        n = int(input())
        arr = [int(x) for x in input().split()]
        x=int(input())

        ll = Llist()
        tail = None

        for nodeData in arr:
            tail = ll.insert(nodeData, tail)

        res=searchLinkedList(ll.head,x)
        print(res)
# } Driver Code Ends

```

</details>


</details>


<details>
<summary>
5. Linked List Insertion
</Summary>

### **Linked List Insertio**n
**Difficulty Level : Basic**


Create a link list of size N according to the given input literals. Each integer input is accompanied by an indicator which can either be 0 or 1. If it is 0, insert the integer in the beginning of the link list. If it is 1, insert the integer at the end of the link list. 

**Hint**: When inserting at the end, make sure that you handle NULL explicitly.

#### **Example 1:**
    Input:
    LinkedList: 9->0->5->1->6->1->2->0->5->0
    Output: 5 2 9 5 6

**Explanation**:
    Length of Link List = N = 5
    9 0 indicated that 9 should be
    inserted in the beginning. Modified
    Link List = 9.
    5 1 indicated that 5 should be
    inserted in the end. Modified Link
    List = 9,5.
    6 1 indicated that 6 should be
    inserted in the end. Modified Link
    List = 9,5,6.
    2 0 indicated that 2 should be
    inserted in the beginning. Modified
    Link List = 2,9,5,6.
    5 0 indicated that 5 should be
    inserted in the beginning. Modified
    Link List = 5,2,9,5,6. 
    Final linked list = 5, 2, 9, 5, 6.

#### **Example 2:**
    Input:
    LinkedList: 5->1->6->1->9->1
    Output: 5 6 9

**Your Task:**

You only need to complete the functions insertAtBeginning() and insertAtEnd() that takes the head of link list and integer value of the data to be inserted as inputs and returns the head of the modified link list. 

**Expected Time Complexity:** O(1) for insertAtBeginning() and O(N) for insertAtEnd().

**Expected Auxiliary Space:** O(1) for both.

**Constraints:**

1 <= N <= 104


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
'''    
class Node:
    def __init__(self,data):
        self.data=data
        self.next=None
'''
class Solution:
    #Function to insert a node at the beginning of the linked list.
    def insertAtBegining(self,head,x):
        # code here 
    
    #Function to insert a node at the end of the linked list.
    def insertAtEnd(self,head,x):
        # code here 




#{ 
 # Driver Code Starts
class Node:
    def __init__(self,data):
        self.data=data
        self.next=None

class LinkedList:
    def __init__(self):
        self.head=None

def printList(head):
    while head:
        print(head.data,end=' ')
        head=head.next
    print()

if __name__ == '__main__':
    t=int(input())
    for cases in range(t):
        n=int(input())
        a=LinkedList()
        
        nodes_info=list(map(int,input().split()))
        for i in range(0,len(nodes_info)-1,2):
            if(nodes_info[i+1]==0):
                a.head = Solution().insertAtBegining(a.head,nodes_info[i])
            else:
                a.head = Solution().insertAtEnd(a.head,nodes_info[i])
        printList(a.head)

 
# } Driver Code Ends
```

</details>


</details>


<details>
<summary>
6.Linked List Insertion At Position
</Summary>

### **Linked List Insertion At Position**
**Difficulty Level : Basic**

Done with this problem? Now use these skills to apply for a job in Job-A-Thon 20!
You are given a linked list of size n. You need to insert an element data just after the given position pos.
The position of first element is 1. If the given position is greater than n, then don't insert anything as it is not possible.

#### **Example 1:**
    Input:
    LinkedList: 1->2->3->4->5
    position = 6, data = 10
    Output: 1 2 3 4 5
**Explanation:** The given linked list is
1 2 3 4 5. The data 10 is to be inserted
after position 6. However, the linked
list only contains 5 elements so we
cannot insert the data.

**Example 2:**

    Input:
    LinkedList: 2->4->6->7->5->1->0
    position = 7, data = 99
    Output: 2 4 6 7 5 1 0 99
#### **Your Task:**
This is a function problem. You only need to complete the function insertAtPosition that takes head, pos, and data as parameters.  The printing is done automatically by the driver code.

**Expected Time Complexity:** O(N).

**Expected Auxiliary Space:** O(1).

**Constraints:**

1 <= n, pos <= 103



#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

'''
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None
'''
def insertAtPosition(head,pos,data):
    #code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

# contributed by RavinderSinghPB
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None


class Llist:
    def __init__(self):
        self.head = None

    def insert(self, data, tail):
        node = Node(data)

        if not self.head:
            self.head = node
            return node

        tail.next = node
        return node


def printList(head):
    while head:
        print(head.data,end=' ')
        head=head.next


if __name__ == '__main__':
    t = int(input())

    for tcs in range(t):

        n = int(input())
        arr = [int(x) for x in input().split()]
        pos,data=[int(x) for x in input().split()]

        ll = Llist()
        tail = None

        for nodeData in arr:
            tail = ll.insert(nodeData, tail)

        insertAtPosition(ll.head,pos,data)
        printList(ll.head)
        print()
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
7.Delete Head of Linked List
</Summary>

### **Delete Head of Linked List**
**Difficulty Level : EASSY**

Done with this problem? Now use these skills to apply for a job in Job-A-Thon 20!
Given a linked list of size n, you have to delete the head of the linked list and return the new head.
Note: Please also set the next of the original head to null.

#### **Example 1:**
    Input:
    LinkedList: 1->2
    Output: 2
#### **Example 2:**
    Input:
    LinkedList: 2->5->7->8->99->100
    Output: 5 7 8 99 100
#### **Your Task:**
The task is to complete the function deleteHead() which takes head referenceand returns reference to the new head node, which is then used to display the list. The printing is done automatically by the driver code.

 **Expected Time Complexity:** O(1).

**Expected Auxiliary Space:** O(1).

**Constraints:**

2 <= number of nodes <= 103





#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

'''
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None
'''

def deleteHead(head):
    #code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

# contributed by RavinderSinghPB
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None


class Llist:
    def __init__(self):
        self.head = None

    def insert(self, data, tail):
        node = Node(data)

        if not self.head:
            self.head = node
            return node

        tail.next = node
        return node

def printList(head):
    while head:
        print(head.data,end=' ')
        head=head.next


if __name__ == '__main__':
    t = int(input())

    for tcs in range(t):

        n = int(input())
        arr = [int(x) for x in input().split()]

        ll = Llist()
        tail = None

        for nodeData in arr:
            tail = ll.insert(nodeData, tail)

        res=deleteHead(ll.head)
        
        if ll.head.next:
            print(' please set head of next to None')
        
        ll.head=res
        printList(ll.head)
        print()
        
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
8.Delete Tail of Linked List
</Summary>

### **Delete Tail of Linked List**
**Difficulty Level : EASSY**

Done with this problem? Now use these skills to apply for a job in Job-A-Thon 20!
Given a linked list of size n, you have to delete the tail (last element) in the linked list.

#### **Example 1:**

    Input:
    LinkedList: 1->2
    Output: 1
#### **Example 2:**

    Input:
    LinkedList: 2->5->7->8->99->100
    Output: 2 5 7 8 99
#### **Your Task:**
The task is to complete the function deleteTail() which takes head reference and returns reference to the head node, which is then used to display the list. The printing is done automatically by the driver code.

**Expected Time Complexity:**O(N).

**Expected Auxiliary Space:**O(1).

**Constraints:**

2 <= number of nodes <= 103





#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

def deleteTail(head):
    #code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

# contributed by RavinderSinghPB
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None


class Llist:
    def __init__(self):
        self.head = None

    def insert(self, data, tail):
        node = Node(data)

        if not self.head:
            self.head = node
            return node

        tail.next = node
        return node

def printList(head):
    while head:
        print(head.data,end=' ')
        head=head.next


if __name__ == '__main__':
    t = int(input())

    for tcs in range(t):

        n = int(input())
        arr = [int(x) for x in input().split()]

        ll = Llist()
        tail = None

        for nodeData in arr:
            tail = ll.insert(nodeData, tail)

        res=deleteTail(ll.head)
        printList(res)
        print()
# } Driver Code Ends
```

</details>


</details>


<details>
<summary>9.Linked List Delete at Position</summary>

**Linked List Delete at Position**
**Difficulty Level : Easy**

Done with this problem? Now use these skills to apply for a job in Job-A-Thon 20!
Given a linked list of size n, you have to delete the node at position pos of the linked list and return the new head. The position of initial node is 1.

#### **Example 1:**
    Input:
    LinkedList: 1->2->3->4->5
    pos = 4
    Output: 1 2 3 5
#### **Example 2:**
    Input:
    LinkedList: 2->5->7->8->99->100
    pos = 6
    Output: 2 5 7 8 99
#### **Your Task:**
The task is to complete the function deleteAtPosition() which takes head reference and pos as argument and returns reference to the new head node, which is then used to display the list. The printing is done automatically by the driver code.

**Expected Time Complexity:**O(pos).

**Expected Auxiliary Space:**O(1).

**Constraints:**

2 <= number of nodes <= 103
1 <= pos <= n






#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

'''
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None
'''
def deleteAtPosition(head, pos):
    #code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

#contributed by RavinderSinghPB
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None


class Llist:
    def __init__(self):
        self.head = None

    def insert(self, data, tail):
        node = Node(data)

        if not self.head:
            self.head = node
            return node

        tail.next = node
        return node
    
def printList(head):
    tmp = head
    while tmp != None:
        print(tmp.data, end=" ")
        tmp=tmp.next
    print()
        


if __name__ == '__main__':
    t = int(input())

    for tcs in range(t):

        n = int(input())
        arr = [int(x) for x in input().split()]
        x=int(input())

        ll = Llist()
        tail = None

        for nodeData in arr:
            tail = ll.insert(nodeData, tail)

        res=deleteAtPosition(ll.head,x)
        printList(res)
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
10.Insert In Sorted Linked List
</Summary>

### **Insert In Sorted Linked List**
**Difficulty Level : Easy**

Apply for Mega Job-A-Thon: Fresher Edition | 30+ Opportunities | Avg CTC: 7 LPA  

Given a sorted (non decreasing) linked list of size n, you have to insert the given data at appropriate position in the linked list.

#### **Example 1:**

    Input:
    LinkedList: 1->2->3->4->5
    data = 10
    Output: 1 2 3 4 5 10
#### **Example 2:**

    Input:
    LinkedList: 2->5->7->8->99->100
    data = 100
    Output: 2 5 7 8 99 100 100
#### **Your Task:**
The task is to complete the function insertInSorted() which takes head reference and data to be inserted as the arguments. The function returns reference to the head node, which is then used to display the list.

**Expected Time Complexity:** O(N).

**Expected Auxiliary Space:** O(1).

**Constraints:**

1 <= number of nodes <= 103


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

'''
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None
'''

def  insertInSorted(head,data):
    #code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

# contributed by RavinderSinghPB
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None


class Llist:
    def __init__(self):
        self.head = None

    def insert(self, data, tail):
        node = Node(data)

        if not self.head:
            self.head = node
            return node

        tail.next = node
        return node


def printList(head):
    while head:
        print(head.data,end=' ')
        head=head.next


if __name__ == '__main__':
    t = int(input())

    for tcs in range(t):

        n = int(input())
        arr = [int(x) for x in input().split()]
        data=int(input())
        ll = Llist()
        tail = None

        for nodeData in arr:
            tail = ll.insert(nodeData, tail)

        res=insertInSorted(ll.head,data)
        printList(res)
        print()
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
11.Insert in Middle of Linked List
</Summary>

### **Insert in Middle of Linked List**
**Difficulty Level : Bacic**

Apply for Mega Job-A-Thon: Fresher Edition | 30+ Opportunities | Avg CTC: 7 LPA  

Given a linked list of size N and a key. The task is to insert the key in the middle of the linked list.

#### **Example 1:**

    Input:
    LinkedList = 1->2->4
    key = 3
    Output: 1 2 3 4
    Explanation: The new element is inserted
    after the current middle element in the
    linked list.
#### **Example 2:**

    Input:
    LinkedList = 10->20->40->50
    key = 30
    Output: 10 20 30 40 50
    Explanation: The new element is inserted
    after the current middle element in the
    linked list and Hence, the output is
    10 20 30 40 50.
 

#### **Your Task:**
The task is to complete the function insertInMiddle() which takes head reference and element to be inserted as the arguments. The printing is done automatically by the driver code.

**Expected Time Complexity :** O(N)

**Expected Auxilliary Space :** O(1)

**Constraints:**

1 <= N <= 104


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3
'''
    Your task is to insert a new node in 
	the middle of the linked list with
	the given value.
	
	{
		# Node Class
		class Node:
		    def __init__(self, data):   # data -> value stored in node
		        self.data = data
		        self.next = None
	}
	
	Function Arguments: head (head of linked list), node 
	(node to be inserted in middle)
	Return Type: None, just insert the new node at mid.
'''
#Function to insert a node in the middle of the linked list.
def insertInMid(head,node):
    #code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3
#Contributed by : Nagendra Jha

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
    
# Node Class
class Node:
    def __init__(self, data):   # data -> value stored in node
        self.data = data
        self.next = None
        
# Linked List Class
class LinkedList:
    def __init__(self):
        self.head = None
        self.tail = None
    
    # creates a new node with given value and appends it at the end of the 
    #linked list
    def append(self, new_value):
        new_node = Node(new_value)
        if self.head is None:
            self.head = new_node
            self.tail = new_node
            return
        self.tail.next = new_node
        self.tail = new_node
        return
    
    # prints the elements of linked list starting with head
    def printList(self):
        if self.head is None:
            print(' ')
            return
        curr_node = self.head
        while curr_node:
            print(curr_node.data,end=" ")
            curr_node=curr_node.next
        print('')

if __name__ == '__main__':
    t=int(input())
    for cases in range(t):
        n = int(input())
        a = LinkedList()
        nodes = list(map(int, input().strip().split()))
        for x in nodes:
            a.append(x)
        mid_elem = int(input())
        insertInMid(a.head, Node(mid_elem) )
        a.printList()
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
12.Is Linked List Sorted
</Summary>

### **Is Linked List Sorted**
**Difficulty Level : Easy**

Apply for Mega Job-A-Thon: Fresher Edition | 30+ Opportunities | Avg CTC: 7 LPA  

Given a linked list of size n, you have to find whether the given linked list is sorted or not.
The sorting can either be non-increasing or non-decreasing.

#### **Example 1:**

    Input:
    LinkedList: 5->5->6->7->8
    Output: 1
#### **Example 2:**

    Input:
    LinkedList: 2->5->7->8->99->7
    Output: 0
#### **Your Task:**
The task is to complete the function isSorted() which takes head reference as argument. The function returns true if the LL is sorted, else it returns false. (The driver code prints 1 when the returned value is true, otherwise 0)

**Expected Time Complexity:** O(N).

**Expected Auxiliary Space:** O(1).

**Constraints:**

1 <= number of nodes <= 103


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

'''
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None
'''
def isSorted(head):
    #code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

#contributed by RavinderSinghPB
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None


class Llist:
    def __init__(self):
        self.head = None

    def insert(self, data, tail):
        node = Node(data)

        if not self.head:
            self.head = node
            return node

        tail.next = node
        return node


if __name__ == '__main__':
    t = int(input())

    for tcs in range(t):

        n = int(input())
        arr = [int(x) for x in input().split()]

        ll = Llist()
        tail = None

        for nodeData in arr:
            tail = ll.insert(nodeData, tail)

        res=isSorted(ll.head)
        print(res)
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
13.Nth node from end of linked list
</Summary>

### **Nth node from end of linked list**
**Difficulty Level : Easy**

Apply for Mega Job-A-Thon: Fresher Edition | 30+ Opportunities | Avg CTC: 7 LPA  

Given a linked list consisting of L nodes and given a number N. The task is to find the Nth node from the end of the linked list.

#### **Example 1:**

    Input:
    N = 2
    LinkedList: 1->2->3->4->5->6->7->8->9
    Output: 8
    Explanation: In the first example, there
    are 9 nodes in linked list and we need
    to find 2nd node from end. 2nd node
    from end is 8.  
#### **Example 2:**

    Input:
    N = 5
    LinkedList: 10->5->100->5
    Output: -1
    Explanation: In the second example, there
    are 4 nodes in the linked list and we
    need to find 5th from the end. Since 'n'
    is more than the number of nodes in the
    linked list, the output is -1.
#### **Your Task:**
The task is to complete the function getNthFromLast() which takes two arguments: reference to head and N and you need to return Nth from the end or -1 in case node doesn't exist.

Note:
Try to solve in a single traversal.

**Expected Time Complexity:** O(N).

**Expected Auxiliary Space:** O(1).

**Constraints:**

1 <= L <= 106
1 <= N <= 106


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3
'''
	Your task is to return the data stored in
	the nth node from end of linked list.
	
	Function Arguments: head (reference to head of the list), n (pos of node from end)
	Return Type: Integer or -1 if no such node exits.

	{
		# Node Class
		class Node:
		    def __init__(self, data):   # data -> value stored in node
		        self.data = data
		        self.next = None
	}
'''
#Function to find the data of nth node from the end of a linked list
def getNthFromLast(head,n):
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
    
# Node Class
class Node:
    def __init__(self, data):   # data -> value stored in node
        self.data = data
        self.next = None

# Linked List Class
class LinkedList:
    def __init__(self):
        self.head = None
        self.tail = None

    # creates a new node with given value and appends it at the end of the linked list
    def append(self, new_value):
        new_node = Node(new_value)
        if self.head is None:
            self.head = new_node
            self.tail = new_node
            return
        self.tail.next = new_node
        self.tail = new_node

if __name__ == '__main__':
    t=int(input())
    for cases in range(t):
        n,nth_node = map(int, input().strip().split())
        a = LinkedList() # create a new linked list 'a'.
        nodes_a = list(map(int, input().strip().split()))
        for x in nodes_a:
            a.append(x)  # add to the end of the list
        print(getNthFromLast(a.head,nth_node))
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
14.Join Two Linked Lists
</Summary>

### **Join Two Linked Lists**
**Difficulty Level : Easy**

Apply for Mega Job-A-Thon: Fresher Edition | 30+ Opportunities | Avg CTC: 7 LPA  

Given two linked lists of size n1 and n2 respectively, you have to join the head of second list to the tail of first so that we can traverse both the lists using head of 1st list.

#### **Example 1:**

    Input:
    LinkedList1: 5
    LinkedList2: 1->2
    Output: 5 1 2
#### **Example 2:**

    Input:
    LinkedList1: 1->2->9->6->5->7
    LinkedList2: 99->8->4
    Output: 1 2 9 6 5 7 99 8 4
#### **Your Task:**
The task is to complete the function joinTheLists() which takes head1 and head2 references as arguments. The function returns head of the first list after joining both lists. The printing is done automatically by the driver code.

**Expected Time Complexity:** O(n1).

**Expected Auxiliary Space:** O(1).

**Constraints:**

1 <= number of nodes in a linkedlist <= 103


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

'''
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None
'''
def joinTheLists(head1, head2):
    #code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

class Node:
    def __init__(self, data):
        self.data = data
        self.next = None


class Llist:
    def __init__(self):
        self.head = None

    def insert(self, data, tail):
        node = Node(data)

        if not self.head:
            self.head = node
            return node

        tail.next = node
        return node

def printList(head):
    tmp = head
    while(head!=None):
        print(head.data, end=" ")
        head=head.next
    head=tmp
    print()

if __name__ == '__main__':
    t = int(input())

    for tcs in range(t):

        n = int(input())
        arr = [int(x) for x in input().split()]
        m=int(input())
        brr = [int(x) for x in input().split()]

        ll1 = Llist()
        ll2 = Llist()
        tail1 = None
        tail2 = None

        for nodeData in arr:
            tail1 = ll1.insert(nodeData, tail1)
        
        for nodeData in brr:
            tail2 = ll2.insert(nodeData, tail2)
        

        res=joinTheLists(ll1.head,ll2.head)
        printList(res)
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
15.Remove duplicate element from sorted Linked List
</Summary>

### **Remove duplicate element from sorted Linked List**
**Difficulty Level : Easy**

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 
Given a singly linked list consisting of N nodes. The task is to remove duplicates (nodes with duplicate values) from the given list (if exists).
Note: Try not to use extra space. Expected time complexity is O(N). The nodes are arranged in a sorted way.

#### **Example 1:**

    Input:
    LinkedList: 2->2->4->5
    Output: 2 4 5
    Explanation: In the given linked list 
    2 ->2 -> 4-> 5, only 2 occurs more 
    than 1 time.
#### **Example 2:**

    Input:
    LinkedList: 2->2->2->2->2
    Output: 2
    Explanation: In the given linked list 
    2 ->2 ->2 ->2 ->2, 2 is the only element
    and is repeated 5 times.
#### **Your Task:**
The task is to complete the function removeDuplicates() which should remove the duplicates from linked list and return the head of the linkedlist.

**Expected Time Complexity :** O(N)

**Expected Auxilliary Space :** O(1)

**Constraints:**

1 <= Number of nodes <= 104




#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3
'''
	Your task is to remove duplicates from given 
	sorted linked list.
	
	Function Arguments: head (head of the given linked list) 
	Return Type: none, just remove the duplicates from the list.

	{
		# Node Class
		class Node:
		    def __init__(self, data):   # data -> value stored in node
		        self.data = data
		        self.next = None
	}
'''
#Function to remove duplicates from sorted linked list.
def removeDuplicates(head):
    #code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

#Contributed by : Nagendra Jha

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
    
# Node Class
class Node:
    def __init__(self, data):   # data -> value stored in node
        self.data = data
        self.next = None

# Linked List Class
class LinkedList:
    def __init__(self):
        self.head = None
        self.tail = None

    # creates a new node with given value and appends it at the end of the 
    #linked list
    def append(self, new_value):
        new_node = Node(new_value)
        if self.head is None:
            self.head = new_node
            self.tail = new_node
            return
        self.tail.next = new_node
        self.tail = new_node

    # prints the elements of linked list starting with head
    def printList(self):
        if self.head is None:
            print(' ')
            return
        curr_node = self.head
        while curr_node:
            print(curr_node.data,end=" ")
            curr_node=curr_node.next
        print('')
    
if __name__ == '__main__':
    t=int(input())
    for cases in range(t):
        n = int(input())
        a = LinkedList() # create a new linked list 'a'.
        nodes = list(map(int, input().strip().split()))
        for x in nodes:
            a.append(x)
        removeDuplicates(a.head)
        a.printList()
# } Driver Code Ends
```

</details>


</details>


<details>
<summary>
16.Reverse a linked list
</Summary>

### **Reverse a linked list**
**Difficulty Level : Easy**

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 
Given a linked list of N nodes. The task is to reverse this list.

#### **Example 1:**

    Input:
    LinkedList: 1->2->3->4->5->6
    Output: 6 5 4 3 2 1
    Explanation: After reversing the list, 
    elements are 6->5->4->3->2->1.
#### **Example 2:**

    Input:
    LinkedList: 2->7->8->9->10
    Output: 10 9 8 7 2
    Explanation: After reversing the list,
    elements are 10->9->8->7->2.
#### **Your Task:**
The task is to complete the function reverseList() with head reference as the only argument and should return new head after reversing the list.

**Expected Time Complexity:** O(N).

**Expected Auxiliary Space:** O(1).

**Constraints:**

1 <= N <= 104


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#function Template for python3

"""
# Node Class

class node:
    def __init__(self, val):
        self.data = val
        self.next = None

"""

class Solution:
    #Function to reverse a linked list.
    def reverseList(self, head):
        # Code here




#{ 
 # Driver Code Starts
# Node Class    
class Node:
    def __init__(self, val):
        self.data = val
        self.next = None

# Linked List Class
class Linked_List:
    def __init__(self):
        self.head = None
        self.tail = None

    def insert(self, val):
        if self.head is None:
            self.head = Node(val)
            self.tail = self.head
        else:
            self.tail.next = Node(val)
            self.tail = self.tail.next

def printList(head):
    tmp = head
    while tmp:
        print(tmp.data, end=' ')
        tmp=tmp.next
    print()

if __name__=='__main__':
    for i in range(int(input())):
        n = int(input())
        arr = [int(x) for x in input().split()]
        
        lis = Linked_List()
        for i in arr:
            lis.insert(i)
        
        newHead = Solution().reverseList(lis.head)
        printList(newHead)

# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
17.Maximum And Minimum In Linked List
</Summary>

### **Maximum And Minimum In Linked List**
**Difficulty Level : Basic**

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 
Given a singly linked list of N elements. The task is to find the maximum and minimum element.

#### **Example 1:**

    Input:
    LinkedList: 1->2->3->4->5
    Output: 5 1
#### **Example 2:**

    Input:
    LinkedList: 2->4->6->7->5->1->0
    Output: 7 0
#### **Your Task:**
Your task is to complete the given functions both of which take head reference as argument and return maximum and minimum element as mentioned. The printing is done by driver code.

**Constraints:**

1 <= n <= 100
1 <= value <= 103

**Expected Time Complexity:** O(N).

**Expected Auxiliary Space:** O(1).


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

'''
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None
'''
def maximum(head):
    #code here
    
    
def minimum(head):
    #code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

import io
import sys

    
# Node class
class Node:
    def __init__(self,data):
        self.data=data
        self.next=None
#Linked list class
class LinkedList:
    def __init__(self):
        self.head=None
        self.tail=None

    # append at the end of the list
    def append(self,new_node):
        if self.head is None:
            self.head=new_node
            self.tail=new_node
            return
        self.tail.next=new_node
        self.tail = self.tail.next

if __name__ == '__main__':
    t=int(input())
    for cases in range(t):
        n=int(input())
        a=LinkedList()
        nodes=list(map(int,input().strip().split())) #list containing nodes
        for x in nodes:
            node=Node(x) # create a new node
            a.append(node)
        print(maximum(a.head), end = " ")
        print(minimum(a.head))
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
18.Identical Linked Lists
</Summary>

### **Identical Linked Lists**
**Difficulty Level : Basic**

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 
Given two Singly Linked List of N and M nodes respectively. The task is to check whether two linked lists are identical or not. 
Two Linked Lists are identical when they have same data and with same arrangement too.

#### **Example 1:**

    Input:
    LinkedList1: 1->2->3->4->5->6
    LinkedList2: 99->59->42->20
    Output: Not identical 
#### **Example 2:**
    
    Input:
    LinkedList1: 1->2->3->4->5
    LinkedList2: 1->2->3->4->5
    Output: Identical
 
#### **Your Task:**
The task is to complete the function areIdentical() which takes the head of both linked lists as arguments and returns True or False.

**Constraints:**

1 <= N <= 103

**Expected Time Complexity :** O(N)

**Expected Auxilliary Space :** O(1)


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
# your task is to complete this function
# function should return true/1 if both
# are identical else return false/0
'''
# Node Class    
class node:
    def __init__(self, val):
        self.data = val
        self.next = None
        
'''

#Function to check whether two linked lists are identical or not.
def areIdentical(head1, head2):
    # Code here


#{ 
 # Driver Code Starts
# Node Class    
class node:
    def __init__(self, val):
        self.data = val
        self.next = None
        
# Linked List Class
class Linked_List:
    def __init__(self):
        self.head = None

    def insert(self, val):
        new_node = node(val)
        new_node.data = val
        new_node.next = self.head
        self.head = new_node
        
def printList(head):
    while head:
        print(head.data, end=' ')
        head=head.next
    print()

def createList(arr, n):
    lis = Linked_List()
    for i in range(n):
        lis.insert(arr[i])
    return lis.head

if __name__=='__main__':
    t = int(input())
    for i in range(t):
        n = int(input())
        arr = list(map(int, input().strip().split()))
        head1 = createList(arr, n)
        n = int(input())
        arr = list(map(int, input().strip().split()))
        head2 = createList(arr, n)
        if(areIdentical(head1, head2)):
            print('Identical')
        else:
            print('Not identical')
# Contributed by: Harshit Sidhwa
# } Driver Code Ends
```

</details>


</details>


