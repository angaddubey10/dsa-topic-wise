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

Given a singly linked list of integers.the task is to display the linked list

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
**Difficulty Level : EASSY**

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

<details>


</details>

