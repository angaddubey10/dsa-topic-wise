### List of Questions
1. Length of Circular Linked List
2. Display Circular Linked List
3. Circular Linked List Head Insert
4. Circular Linked List Tail Insert
5. Delete Tail of Circular Linked List
6. Check If Circular Linked List
7. Delete Head of Circular Linked List
8. Circular Linked List Delete at Position
9. Circular Linked List Insertion At Position


  -----

  ## Details of Questions Listed Above

  <details>
<summary>
Length of Circular Linked List

</Summary>

### **Length of Circular Linked List**
**Difficulty Level : Basic** 

Last Week Of Job Fair 2023. Explore Unlimited Opportunities Now!
Given a circular linked list of size n, you need to find the length of the list (total number of nodes). The tail of the linked list is connected to head.

#### **Example 1:**

    Input:
    LinkedList: 1->2->3->4->5
    (the first and the last node is connected,
    i.e 5 --> 1)
    Output: 5
#### **Example 2:**

    Input:
    LinkedList: 2->5->7->8->99->100
    (the first and the last node is connected,
    i.e 100 --> 2)
    Output: 6
#### **Your Task:**
The task is to complete the function getLength() which takes head reference as argument and returns the total number of nodes in the list. The printing is done by the driver code.

**Expected Time Complexity:** O(N).

**Expected Auxiliary Space:** O(1).

**Constraints:**

1 <= number of nodes <= 1000




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

def getLength(head):
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

        ll = Llist()
        tail = None

        for nodeData in arr:
            tail = ll.insert(nodeData, tail)
        #making circular
        tail.next=ll.head

        print(getLength(ll.head))
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Circular Linked List Head Insert
</Summary>

### **Display Circular Linked List**
**Difficulty Level : Basic** 

Last Week Of Job Fair 2023. Explore Unlimited Opportunities Now!
Given a circular linked list of size n, you need to display the linked list. The tail of the linked list is connected to head.

#### **Example 1:**

    Input:
    LinkedList: 1->2->3->4
    (the last and the first node are connected,
    i.e. 4 -> 1)
    Output: 1 2 3 4
#### **Example 2:**

**Input:
LinkedList: 1->2
(the last and the first node are connected,
i.e. 2 -> 1)
Output: 1 2**
#### **Your Task:**
The task is to complete the function displayList() which takes head reference as argument and returns the circular linked list as a list.

**Expected Time Complexity:** O(N).

**Expected Auxiliary Space:** O(N).

**Constraints:**

1 <= number of nodes <= 1000


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

def displayList(head):
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

        ll = Llist()
        tail = None

        for nodeData in arr:
            tail = ll.insert(nodeData, tail)
        #making circular
        tail.next=ll.head

        a = displayList(ll.head)
        for c in a:
            print(c,end=" ")
        print()
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Circular Linked List Head Insert

</Summary>

### **Circular Linked List Head Insert**
**Difficulty Level : EASY** 

Last Week Of Job Fair 2023. Explore Unlimited Opportunities Now!
Given a circular linked list of size N, you need to insert an element data before the head and make it the new head. The tail of the linked list is connected to head.

#### **Example 1:**

    Input:
    LinkedList: 1->2->3->4
    (the first and last node is connected,
    i.e. 4 --> 1)
    data = 10
    Output: 10 1 2 3 4
#### **Example 2:**

    Input:
    LinkedList: 1 2
    (the first and last node is connected,
    i.e. 2 --> 1)
    data = 5
    Output: 5 1 2
#### **Your Task:**
The task is to complete the function insertInHead() which takes head reference and data as arguments and returns the head of the updated list. The printing is done by the driver code.

**Expected Time Complexity:**O(N).

**Expected Auxiliary Space:** O(1).

1 <= Number of nodes <= 1000




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

def insertInHead(head,x):
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



def displayList(head):
    t=head
    while t.next!=head:
        print(t.data,end=' ')
        t=t.next
    print(t.data,end=' ')



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
        #making circular
        tail.next=ll.head

        resHead=insertInHead(ll.head,data)
        displayList(resHead)
        print()
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Circular Linked List Tail Insert
</Summary>

### **Circular Linked List Tail Insert**
**Difficulty Level : EASY** 

Last Week Of Job Fair 2023. Explore Unlimited Opportunities Now!
Given a circular linked list of size N, you need to insert an element data after the tail.
The tail of the linked list is connected to head.

#### **Example 1:**

    Input:
    LinkedList: 1->2->3->4
    (the first and last node is connected,
    i.e. 4 --> 1)
    data = 10
    Output: 1 2 3 4 10
#### **Example 2:**

    Input:
    LinkedList: 1 2
    (the first and last node is connected,
    i.e. 2 --> 1)
    data = 5
    Output: 1 2 5
#### **Your Task:**
The task is to complete the function insertInTail() which takes head reference and data as arguments and returns the head of the updated list. The printing is done by the driver code.

**Expected Time Complexity:** O(N).

**Expected Auxiliary Space:**O(1).

**Constraints:**

1 <= Number of nodes <= 1000


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

def insertInTail(head,x):
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



def displayList(head):
    t=head
    while t.next!=head:
        print(t.data,end=' ')
        t=t.next
    print(t.data,end=' ')



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
        #making circular
        tail.next=ll.head

        resHead=insertInTail(ll.head,data)
        displayList(resHead)
        print()
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Delete Tail of Circular Linked List

</Summary>

### **Delete Tail of Circular Linked List**
**Difficulty Level : EASY** 

Last Week Of Job Fair 2023. Explore Unlimited Opportunities Now!
Given a circular linked list of size n, you have to delete the tail (last element) in the linked list.
In a circular linked list, the tail is connect to the head using the next pointer.

#### **Example 1:**

    Input:
    LinkedList: 1->2
    (the first and last node are connected,
    i.e. 2 --> 1)
    Output: 1
#### **Example 2:**

    Input:
    LinkedList: 2->5->7->8->99->100
    (the first and last node are connected,
    i.e. 100 --> 2)
    Output: 2 5 7 8 99
#### **Your Task:**
The task is to complete the function deleteTail() which takes head reference  and returns reference to the head node, which is then used to display the list. The printing is done automatically by the driver code.

**Expected Time Complexity:** O(n).

**Expected Auxiliary Space:**O(1).

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



def displayList(head):
    t=head
    while t.next!=head:
        print(t.data,end=' ')
        t=t.next
    print(t.data,end=' ')


if __name__ == '__main__':
    t = int(input())

    for tcs in range(t):

        n = int(input())
        arr = [int(x) for x in input().split()]

        ll = Llist()
        tail = None

        for nodeData in arr:
            tail = ll.insert(nodeData, tail)
        #making circular
        tail.next=ll.head

        deleteTail(ll.head)
        displayList(ll.head)
        print()
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Check If Circular Linked List

</Summary>

### **Check If Circular Linked List**
**Difficulty Level : Basic** 

Last Week Of Job Fair 2023. Explore Unlimited Opportunities Now!
Given head, the head of a singly linked list, find if the linked list is circular or not. A linked list is called circular if it not NULL terminated and all nodes are connected in the form of a cycle. An empty linked list is considered as circular.

Note: The linked list does not contains any inner loop.

#### **Example 1:**

    Input:
    LinkedList: 1->2->3->4->5
    (the first and last node is connected,
    i.e. 5 --> 1)
    Output: 1
#### **Example 2:**

    Input:
    LinkedList: 2->4->6->7->5->1
    Output: 0
#### **Your Task:**
The task is to complete the function isCircular() which checks if the given linked list is circular or not. It should return true or false accordingly. (the driver code prints 1 if the returned values is true, otherwise 0)

**Expected Time Complexity:** O(N).

**Expected Auxiliary Space:** O(1).

**Constraints:**

1 <=Number of nodes<= 100


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#class Node:
#    def __init__(self, data):
#        self.data = data
#        self.next = None


# your task is to complete this function
# function should return true/false or 1/0
def isCircular(head):
    # Code here



#{ 
 # Driver Code Starts
# Node class
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None

class LinkedList:
    # Function to initialize head
    def __init__(self):
        self.head = None

    # Function to insert a new node at the beginning
    def push(self, new_data):
        new_node = Node(new_data)
        new_node.next = self.head
        self.head = new_node

    # Utility function to prit the linked LinkedList
    def printList(self, node):
        temp = node
        while (temp):
            print(temp.data, end=" ")
            temp = temp.next

    def getHead(self):
        return self.head

    def createLoop(self, n):
        if n == 0:
            return None
        temp = self.head
        ptr = self.head
        cnt = 1
        while (cnt != n):
            ptr = ptr.next
            cnt += 1
        # print ptr.data
        while (temp.next):
            temp = temp.next
        temp.next = ptr

# Driver program
if __name__=='__main__':
    t=int(input())
    for i in range(t):
        n,isloop = list(map(int, input().strip().split()))
        arr=list(map(int, input().strip().split()))
        lst=LinkedList()
        for i in arr:
            lst.push(i)
        if(isloop):
            lst.createLoop(1)
        if isCircular(lst.getHead()):
            print(1)
        else:
            print(0)
# Contributed By: Harshit Sidhwa
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Delete Head of Circular Linked List
</Summary>

### **Delete Head of Circular Linked List**
**Difficulty Level : Easy** 

Last Week Of Job Fair 2023. Explore Unlimited Opportunities Now!
Given a circular linked list of size n, you have to delete the head of the linked list and return the new head.
In the circular linked list the tail of the list is connected to the head using the next pointer.

Note:Please also set the next of the original head to null.

#### **Example 1:**

    Input:
    LinkedList: 1->2
    (the first and last node are connected,
    i.e. 2 --> 1)
    Output: 2
#### **Example 2:**

    Input:
    LinkedList: 2->5->7->8->99->100
    (the first and last node are connected,
    i.e. 100 --> 2)
    Output: 5 7 8 99 100
#### **Your Task:**
The task is to complete the function deleteHead() which takes head reference. The function deletes the head node and returns a reference to the new head node, which is then used to display the list. The printing is done automatically by the driver code.

**Expected Time Complexity:** O(n).

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


def displayList(head):
    t=head
    while t.next!=head:
        print(t.data,end=' ')
        t=t.next
    print(t.data,end=' ')


if __name__ == '__main__':
    t = int(input())

    for tcs in range(t):

        n = int(input())
        arr = [int(x) for x in input().split()]

        ll = Llist()
        tail = None

        for nodeData in arr:
            tail = ll.insert(nodeData, tail)
        #making circular
        tail.next=ll.head

        resHead=deleteHead(ll.head)
        displayList(resHead)
        print()
# } Driver Code Ends

```

</details>


</details>

<details>
<summary>
Circular Linked List Delete at Position
</Summary>

### **Circular Linked List Delete at Position**
**Difficulty Level : Easy** 

Last Week Of Job Fair 2023. Explore Unlimited Opportunities Now!
Given a linked list of size n, you have to delete the node at position pos of the linked list and return the new head. The position of initial node is 1.
The tail of the circular linked list is connected to the head using next pointer.

#### **Example 1:**

    Input:
    LinkedList: 1->2->3->4->5
    (the first and last node are connected,
    i.e. 5 --> 1)
    position: 4
    Output: 1 2 3 5
#### **Example 2:**

    Input:
    LinkedList: 2->5->7->8->99->100
    (the first and last node are connected,
    i.e. 5 --> 1)
    position: 6
    Output: 2 5 7 8 99
#### **Your Task:**
The task is to complete the function deleteAtPosition() which takes head reference and pos as argument and returns reference to the new head node, which is then used to display the list. The printing is done automatically by the driver code.

**Expected Time Complexity:** O(n).

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
def deleteAtPosition(head,pos):
    #code here


#{ 
 # Driver Code Starts
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


def displayList(head):
    t=head
    while t.next!=head:
        print(t.data,end=' ')
        t=t.next

    
    print(t.data,end=' ')


if __name__ == '__main__':
    t = int(input())

    for tcs in range(t):

        n = int(input())
        arr = [int(x) for x in input().split()]
        pos=int(input())

        ll = Llist()
        tail = None

        for nodeData in arr:
            tail = ll.insert(nodeData, tail)
        #making circular
        tail.next=ll.head

        resHead=deleteAtPosition(ll.head,pos)
        displayList(resHead)
        print()
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Circular Linked List Insertion At Position
</Summary>

### **Circular Linked List Insertion At Position**
**Difficulty Level : Easy** 

Last Week Of Job Fair 2023. Explore Unlimited Opportunities Now!
You are given a circular linked list of size N. You need to insert an element data just after the given position pos.
The position of first element is 1. If the given position is greater than N, then don't insert anything as it is not possible.
As the given linked list is circular, it means that the tail is connected to the head of the list.

#### **Example 1:**

    Input:
    LinkedList: 1->2->3->4->5
    (the first and last node is connected,
    i.e. 5 --> 1)
    position = 6, element = 10
    Output: 1 2 3 4 5 
#### **Example 2:**

    Input:
    LinkedList: 2->4->6->7->5->1->0
    (the first and last node is connected,
    i.e. 0 --> 2)
    position = 7,data = 99
    Output: 2 4 6 7 5 1 0 99
#### **Your Task:**
You only need to complete the function insertAtPosition that takes head, pos, and data as parameters. The printing is done automatically by the driver code.

**Expected Time Complexity:** O(N).

**Expected Auxiliary Space:** O(1).

**Constraints:**

1 <= N, pos <= 103


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


def displayList(head):
    t=head
    while t.next!=head:
        print(t.data,end=' ')
        t=t.next
    print(t.data,end=' ')


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
        #making circular
        tail.next=ll.head

        insertAtPosition(ll.head,pos,data)
        displayList(ll.head)
        print()
# } Driver Code Ends
```

</details>


</details>