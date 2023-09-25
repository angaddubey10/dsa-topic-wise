### list of Questions
 1. Display Doubly Linked List
 2. Doubly Linked List Head Insert
 3. Display Circular Doubly Linked List
 4. Is The Doubly Linked List Circular
 5. Doubly Linked List Tail Insert
 6. Doubly linked list Insertion at given position
 7. Delete Head of Doubly Linked List
 8. Find Middle of Circular Doubly Linked List
 9. Delete node in Doubly Linked List
 10. Delete Tail of Doubly Linked List
 11. Reverse a Doubly Linked List
 12. Insert in Sorted way in a Sorted DLL
 13. Compare Circular Doubly Linked Lists


----


 ## Details of Questions Listed Above
<details>
<summary>
Display Doubly Linked List
</Summary>

### **Display Doubly Linked List**
**Difficulty Level : Basic** 

Last Week Of Job Fair 2023. Explore Unlimited Opportunities Now!
Given a doubly linked list of n elements. The task is to display the linked list.

#### **Example 1:**

    Input:
    LinkedList: 1<->2<->3<->4<->5
    Output:
    1 2 3 4 5
    5 4 3 2 1
#### **Your Task:**
Your task is to complete the given function displayList(), which takes head reference as argument and returns the doubly linked list as an array ( vector in cpp, ArrayList in java, list in python)
The driver's code print the list forward and backward.

**Expected Time Complexity:** O(n).

**Expected Auxiliary Space:**O(1).

**Constraints:**

1 <= number of nodes <= 103
0 <= value of nodes <= 103


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

def displayList(head):
    #code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

#contributed by RavinderSinghPB
class Node:
    def __init__(self,data):
        self.data=data
        self.next=None
        self.prev=None

class doublyLL:
    def __init__(self):
        self.head=None

    def insert(self,tail,data):
        head=self.head

        node=Node(data)

        if not head:

            self.head=node
            return node

        tail.next=node
        node.prev=tail
        return node

if __name__=='__main__':
    tcs=int(input())

    for _ in range(tcs):
        n=int(input())
        arr=[int(x) for x in input().split()]

        dll=doublyLL()

        tail=None

        for nodeData in arr:
            tail=dll.insert(tail,nodeData)

        l = displayList(dll.head)
        for x in l:
            print(x,end = ' ')
        print()
        
        for i in range(len(l)-1,-1,-1):
            print(l[i],end = ' ')
        print()

# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Doubly Linked List Head Insert
</Summary>

### **Doubly Linked List Head Insert**
**Difficulty Level : Basic** 

Last Week Of Job Fair 2023. Explore Unlimited Opportunities Now!
Given a doubly linked list of size n, you need to insert an element data before the head and make it the new head.

#### **Example 1:**

    Input:
    LinkedList: 1<->2<->3<->4<->5
    data = 8
    Output:
    8 1 2 3 4 5
    5 4 3 2 1 8
#### **Example 2:**

    Input:
    LinkedList: 2<->4<->6<->7<->5<->1<->10
    data = 89
    Output:
    89 2 4 6 7 5 1 10
    10 1 5 7 6 4 2 89
#### **Your Task:**
The task is to complete the function insertInHead() which takes head reference and data as arguments and returns the head of the updated list. (The driver's code print the updated linked list twice, once forward and once backward)

**Expected Time Complexity:** O(1).

**Expected Auxiliary Space:** O(1).

**Constraints:**

1 <= number of nodes <= 1000


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

def insertInhead(head,data):
    #code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

#contributed by RavinderSinghPB
class Node:
    def __init__(self,data):
        self.data=data
        self.next=None
        self.prev=None

class doublyLL:
    def __init__(self):
        self.head=None

    def insert(self,tail,data):
        head=self.head

        node=Node(data)

        if not head:

            self.head=node
            return node

        tail.next=node
        node.prev=tail
        return node

def displayList(head):
    while head:
        print(head.data,end=' ')
        pvs=head
        head=head.next
    print()

    while pvs:
        print(pvs.data,end=' ')
        pvs=pvs.prev






if __name__=='__main__':
    tcs=int(input())

    for _ in range(tcs):
        n=int(input())
        arr=[int(x) for x in input().split()]
        headData=int(input())

        dll=doublyLL()

        tail=None

        for nodeData in arr:
            tail=dll.insert(tail,nodeData)

        dll.head=insertInhead(dll.head,headData)
        displayList(dll.head)
        print()




# } Driver Code Ends

```

</details>


</details>

<details>
<summary>
Display Circular Doubly Linked List
</Summary>

### **Display Circular Doubly Linked List**
**Difficulty Level : Basic**

Last Week Of Job Fair 2023. Explore Unlimited Opportunities Now!
Given a circular doubly linked list consisting of N nodes, the task is to print the elements from head to tail, then from tail to head in two separate lines.
The tail of a circular doubly linked list is connected to head via its next pointer, and the previous pointer of head is connected to the tail.

#### **Example 1:**

    Input:
    LinkedList: 1<->2
    (the last and first node are connected,
    i.e. 2<->1)
    Output:
    1 2
    2 1
#### **Example 2.**
    Input:
    LinkedList: 2<->5<->7<->8<->99<->100
    Output:
    2 5 7 8 99 100
    100 99 8 7 5 2
#### **Your Task:**
The task is to complete the function displayList() which takes head reference as an argument and return  the the circular doubly linked list as a list. 
Note: The returned list is printed twice, once forward and once backward.

**Expected Time Complexity:** O(N).

**Expected Auxiliary Space:** O(N).

**Constraints:**

1 <= N<= 103
#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

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
        self.prev = None


class doublyLL:
    def __init__(self):
        self.head = None

    def insert(self, tail, data):
        head = self.head

        node = Node(data)

        if not head:
            self.head = node
            return node

        tail.next = node
        node.prev = tail
        return node

if __name__ == '__main__':
    tcs = int(input())

    for _ in range(tcs):
        n = int(input())
        arr = [int(x) for x in input().split()]

        dll = doublyLL()

        tail = None

        for nodeData in arr:
            tail = dll.insert(tail, nodeData)

        # making circular
        tail.next = dll.head
        dll.head.prev = tail

        a = displayList(dll.head)
        for x in a:
            print(x,end=' ')
        print()
        
        for i in range(len(a)-1,-1,-1):
            print(a[i],end=' ')
        print()




# } Driver Code Ends
```

</details>

</details>

<details>
<summary>
Is The Doubly Linked List Circular
</Summary>

### **Is The Doubly Linked List Circular**
**Difficulty Level : Easy**

Last Week Of Job Fair 2023. Explore Unlimited Opportunities Now!
Given a doubly linked list, the task is to check if it is circular or not.

#### **Example 1:**

    Input:
    LinkedList: 2<->3<->4<->5<->6
    Output: 0
#### **Example 2:**

    Input:
    LinkedList: 4<-->6
    (the last and the first node is connected,
    i.e. 6 <--> 4
    Output: 1
#### **User Task:**
The task is to complete the function isCircular() which takes head reference as an argument. The function should return true if the doubly LL is circular and false if it is not. (if the returned value if true, the driver code prints 1, otherwise 0)

**Expected Time Complexity:** O(n).

**Expected Auxiliary Space:**O(1).

**Constraints:**

1 <= Number of nodes <= 106


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution: 
    def isCircular(self, head):
        #code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

# contributed by RavinderSinghPB
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None
        self.prev = None


class doublyLL:
    def __init__(self):
        self.head = None

    def insert(self, tail, data):
        head = self.head

        node = Node(data)

        if not head:
            self.head = node
            return node

        tail.next = node
        node.prev = tail
        return node

if __name__ == '__main__':
    tcs = int(input())

    for _ in range(tcs):
        n = int(input())
        arr = [int(x) for x in input().split()]
        x=int(input())


        dll = doublyLL()

        tail = None

        for nodeData in arr:
            tail = dll.insert(tail, nodeData)

        if x==1:
            # making circular
            tail.next = dll.head
            dll.head.prev = tail
        ob=Solution()
        print(ob.isCircular(dll.head))





# } Driver Code Ends
```

</details>


</details>


<details>
<summary>
Doubly Linked List Tail Insert
</summary>

### **Doubly Linked List Tail Insert**
**Difficulty Level : Basic**

Last Week Of Job Fair 2023. Explore Unlimited Opportunities Now!
Given a doubly linked list of size n, you need to insert an element data after the tail.

#### **Example 1:**

    Input:
    LinkedList: 1<->2<->3<->4<->5
    data = 8
    Output:
    1 2 3 4 5 8
    8 5 4 3 2 1
#### **Example 2:**

    Input:
    LinkedList: 2<->4<->6<->7<->5<->1<->10
    data = 89
    Output:
    2 4 6 7 5 1 10 89
    89 10 1 5 7 6 4 2
#### **Your Task:**
The task is to complete the function insertInTail() which takes head reference and data as arguments and returns the head of the updated list. (The driver's code print the updated linked list twice, once forward and once backward)

**Expected Time Complexity:** O(N).

**Expected Auxiliary Space:** O(1).

**Constraints:**

1 ≤ number of nodes ≤ 1000






#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

def insertInTail(head,data):
    #code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

#contributed by RavinderSinghPB
class Node:
    def __init__(self,data):
        self.data=data
        self.next=None
        self.prev=None

class doublyLL:
    def __init__(self):
        self.head=None

    def insert(self,tail,data):
        head=self.head

        node=Node(data)

        if not head:

            self.head=node
            return node

        tail.next=node
        node.prev=tail
        return node

def displayList(head):
    while head:
        if (head.next != None):
            print(head.data, end=' ')
        else:
            print(head.data, end='\n')
        pvs=head
        head=head.next

    while pvs:
        if (pvs.prev != None):
            print(pvs.data, end=' ')
        else:
            print(pvs.data, end='\n')
        pvs=pvs.prev


if __name__=='__main__':
    tcs=int(input())

    for _ in range(tcs):
        n=int(input())
        arr=[int(x) for x in input().split()]
        tailData=int(input())

        dll=doublyLL()

        tail=None

        for nodeData in arr:
            tail=dll.insert(tail,nodeData)

        dll.head=insertInTail(dll.head,tailData)
        displayList(dll.head)
        # print()


# } Driver Code Ends
```

</details>


</details>


<details>
<summary>
Doubly linked list Insertion at given position
</Summary>

### **Doubly linked list Insertion at given position**
**Difficulty Level : Basic**

Last Week Of Job Fair 2023. Explore Unlimited Opportunities Now!
Given a doubly-linked list, a position p, and an integer x. The task is to add a new node with value x at the position just after pth node in the doubly linked list.

#### **Example 1:**

    Input:
    LinkedList: 2<->4<->5
    p = 2, x = 6 
    Output: 2 4 5 6
    Explanation: p = 2, and x = 6. So, 6 is
    inserted after p, i.e, at position 3
    (0-based indexing).
#### **Example 2:**

    Input:
    LinkedList: 1<->2<->3<->4
    p = 0, x = 44
    Output: 1 44 2 3 4
    Explanation: p = 0, and x = 44 . So, 44
    is inserted after p, i.e, at position 1
    (0-based indexing).
#### **Your Task:**
The task is to complete the function addNode() which head reference, position and data to be inserted as the arguments, with no return type.

**Expected Time Complexity :** O(N)

**Expected Auxilliary Space :** O(1)

**Constraints:**

1 <= N <= 104
0 <= p < N

 


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
# Your task is to complete this function
# function should add a new node after the pth position
# function shouldn't print or return any data

'''
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None
        self.prev = None

'''
#Function to insert a new node at given position in doubly linked list.
def addNode(head, p, data):
    # Code here



#{ 
 # Driver Code Starts
class Node:
    def __init__(self, data):
        self.data = data
        
        
        self.next = None
        self.prev = None


class DoublyLinkedList:
    def __init__(self):
        self.head = None
        self.tail = None

    def add(self, new_data):
        new_node = Node(new_data)
        if(self.head == None):
            self.head = new_node
            self.tail = new_node
            return
        
        self.tail.next = new_node
        new_node.prev = self.tail
        self.tail = new_node
        return
        
    def printList(self, node):
        while(node.next is not None):
            node = node.next
        while node.prev is not None:
            node = node.prev
        while(node is not None):
            print(node.data, end=" ")
            node = node.next
        print()
        
if __name__=='__main__':
    t = int(input())
    for i in range(t):
        n = int(input())
        arr = map(int, input().strip().split())
        llist = DoublyLinkedList()
        for e in arr:
            llist.add(e)
            
        pos,data = map(int, input().strip().split())
        
        addNode(llist.head, pos, data)
        llist.printList(llist.head)

# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Delete Head of Doubly Linked List

</Summary>

### **Delete Head of Doubly Linked List**
**Difficulty Level : Easy**

Last Week Of Job Fair 2023. Explore Unlimited Opportunities Now!
Given a doubly linked list of size n, you have to delete the head of the linked list and return the new head.
Note: Please set the previous of new head to null, and set the next of old head to null, and then delete the old head.

#### **Example 1:**

    Input:
    LinkedList: 1<-->2
    Output:
    2
    2
#### **Example 2:**

    Input:
    LinkedList: 2<-->5<-->7<-->8<-->99<-->100
    Output:
    5 7 8 99 100
    100 99 8 7 5
#### **Your Task:**
The task is to complete the function deleteHead() which takes head reference and returns reference to the new head node, which is then used to display the list. (The driver's code print the modified list twice, once forward and once backward)

**Expected Time Complexity:** O(n).

**Expected Auxiliary Space:** O(1).

**Constraints:**

2 <= number of nodes <= 103


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

def deleteHead(head):
    #code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

#contributed by RavinderSinghPB
class Node:
    def __init__(self,data):
        self.data=data
        self.next=None
        self.prev=None

class doublyLL:
    def __init__(self):
        self.head=None

    def insert(self,tail,data):
        head=self.head

        node=Node(data)

        if not head:

            self.head=node
            return node

        tail.next=node
        node.prev=tail
        return node

def displayList(head):
    while head:
        print(head.data,end=' ')
        pvs=head
        head=head.next
    print()

    while pvs:
        print(pvs.data,end=' ')
        pvs=pvs.prev


if __name__=='__main__':
    tcs=int(input())

    for _ in range(tcs):
        n=int(input())
        arr=[int(x) for x in input().split()]

        dll=doublyLL()

        tail=None

        for nodeData in arr:
            tail=dll.insert(tail,nodeData)

        dll.head=deleteHead(dll.head)
        displayList(dll.head)
        print()




# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Find Middle of Circular Doubly Linked List
</Summary>

### **Find Middle of Circular Doubly Linked List**
**Difficulty Level : Easy**

Last Week Of Job Fair 2023. Explore Unlimited Opportunities Now!
Given a circular doubly linked list of odd size n, the task is to print the middle element.
The tail of a circular doubly linked list is connected to head via its next pointer, and the previous pointer of head is connected to the tail.

#### **Example 1:**

    Input:
    LinkedList: 1<-->2<-->3
    (The first and the last node is connected,
    i.e 3 <--> 1)
    Output: 2
#### **Your Task:**
The task is to complete the function findMiddle() which takes head reference as an argument. The function should return the middle element of CDLL. 

**Expected Time Complexity:** O(N).

**Expected Auxiliary Space:** O(1).

**Constraints:**

1 <= Number of nodes <= 103


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    def findMiddle(self, head):
        #code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

# contributed by RavinderSinghPB
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None
        self.prev = None


class doublyLL:
    def __init__(self):
        self.head = None

    def insert(self, tail, data):
        head = self.head

        node = Node(data)

        if not head:
            self.head = node
            return node

        tail.next = node
        node.prev = tail
        return node


if __name__ == '__main__':
    tcs = int(input())

    for _ in range(tcs):
        n = int(input())
        arr = [int(x) for x in input().split()]

        dll = doublyLL()

        tail = None

        for nodeData in arr:
            tail = dll.insert(tail, nodeData)

        # making circular
        tail.next = dll.head
        dll.head.prev = tail

        ob=Solution()
        print(ob.findMiddle(dll.head))




# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Delete node in Doubly Linked List
</Summary>

### **Delete node in Doubly Linked List**
**Difficulty Level : BASIC**

Last Week Of Job Fair 2023. Explore Unlimited Opportunities Now!
Given a doubly linked list and a position. The task is to delete a node from given position in a doubly linked list.

#### **Example 1:**

    Input:
    LinkedList = 1 <--> 3 <--> 4 
    x = 3
    Output: 1 3  
    Explanation: After deleting the node at
    position 3 (position starts from 1),
    the linked list will be now as 1->3.
#### **Example 2:**

    Input:
    LinkedList = 1 <--> 5 <--> 2 <--> 9  
    x = 1
    Output: 5 2 9
#### Your Task:
The task is to complete the function deleteNode() which should delete the node at given position and return the head of the linkedlist.

**Expected Time Complexity :** O(N)

**Expected Auxilliary Space :** O(1)

**Constraints:**

2 <= size of the linked list <= 1000
1 <= x <= N


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python 
#User function Template for python3

'''class Node:
    def __init__(self, data):
        self.data = data
        self.next = None
        self.prev = None
'''
class Solution:
    def deleteNode(self,head, x):
        # Code here



#{ 
 # Driver Code Starts
#Initial Template for Python 3


class Node:
    def __init__(self, data):
        self.data = data
        self.next = None
        self.prev = None


class DoublyLinkedList:
    def __init__(self):
        self.head = None
        self.tail = None

    def append(self, new_data):
        new_node = Node(new_data)
        new_node.next = None
        if self.head is None:
            new_node.prev = None
            self.head = new_node
            self.tail = self.head
            return
        self.tail.next = new_node
        self.tail.next.prev = self.tail
        self.tail = self.tail.next

    def printList(self, node):
        while (node.next is not None):
            node = node.next
        while node.prev is not None:
            node = node.prev
        while (node is not None):
            print(node.data, end=" ")
            node = node.next
        print()


if __name__ == '__main__':
    t = int(input())
    for i in range(t):
        n = int(input())
        arr = list(map(int, input().strip().split()))
        llist = DoublyLinkedList()
        for e in arr:
            llist.append(e)
        pos = int(input())
        Solution().deleteNode(llist.head, pos)
        llist.printList(llist.head)
# Contributed by: Harshit Sidhwa

                               
# } Driver Code Ends

```

</details>


</details>

<details>
<summary>
Delete Tail of Doubly Linked List</Summary>

**Delete Tail of Doubly Linked List**
**Difficulty Level : Easy**

Last Week Of Job Fair 2023. Explore Unlimited Opportunities Now!
Given a doubly linked list of size n, you have to delete the tail (last element) in the linked list.

#### **Example 1:**

    Input:
    LinkedList: 1<-->2
    Output:
    1
    1
#### **Example 2:**

    Input:
    LinkedList: 2<-->5<-->7<-->8<-->99<-->100
    Output:
    2 5 7 8 99
    99 8 7 5 2
#### **Your Task:**

The task is to complete the function deleteTail() which takes head reference and returns reference to the head node of the modifies list, which is then used to display the list. (The driver's code print the modified list twice, once forward and once backward)

**Expected Time Complexity:** O(n).

**Expected Auxiliary Space:** O(1).

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

class Node:
    def __init__(self,data):
        self.data=data
        self.next=None
        self.prev=None

class doublyLL:
    def __init__(self):
        self.head=None

    def insert(self,tail,data):
        head=self.head

        node=Node(data)

        if not head:

            self.head=node
            return node

        tail.next=node
        node.prev=tail
        return node

def displayList(head):
    while head:
        print(head.data,end=' ')
        pvs=head
        head=head.next
    print()

    while pvs:
        print(pvs.data,end=' ')
        pvs=pvs.prev


if __name__=='__main__':
    tcs=int(input())

    for _ in range(tcs):
        n=int(input())
        arr=[int(x) for x in input().split()]

        dll=doublyLL()

        tail=None

        for nodeData in arr:
            tail=dll.insert(tail,nodeData)

        deleteTail(dll.head)
        displayList(dll.head)
        print()

# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Reverse a Doubly Linked List
</Summary>

#### **Reverse a Doubly Linked List
Compare Circular Doubly Linked Lists
EasyAccuracy: 50.92%Submissions: 4K+Points: 2
Last Week Of Job Fair 2023. Explore Unlimited Opportunities Now!
Given two circular doubly linked lists of sizes n1 and n2 respectively, the task is check if the corresponding elements of the lists are same or not.
The tail of a circular doubly linked list is connected to head via its next pointer, and the previous pointer of head is connected to the tail.

Example 1:

Input:
LinkedList1: 1
LinkedList2: 1
Output: 1
Example 2:

Input:
LinkedList1: 2<->5<->7<->8<->99<->100
LinkedList2: 7<->8<->9<->73<->2
Output: 0
Your Task:
The task is to complete the function compareCLL() which takes head1 and head2 references as an arguments. The function should return true if all the corresponding elements of the lists are same, else it should return false. (The driver's code print 1 if the returned value is true, otherwise false.)

Expected Time Complexity: O(n1 + n2).
Expected Auxiliary Space: O(1).

Constraints:
1 <= number of nodes <= 105

Last Week Of Job Fair 2023. Explore Unlimited Opportunities Now!
Given a doubly linked list of n elements. The task is to reverse the doubly linked list.

#### **Example 1:**

    Input:
    LinkedList: 3 <--> 4 <--> 5
    Output: 5 4 3
#### **Example 2:**

    Input:
    LinkedList: 75 <--> 122 <--> 59 <--> 196
    Output: 196 59 122 75
#### **Your Task:**
Your task is to complete the given function reverseDLL(), which takes head reference as argument and should reverse the elements so that the tail becomes the new head and all pointers are correctly pointed. You need to return the new head of the reversed list. The printing and verification is done by the driver code.

**Expected Time Complexity:** O(n).

**Expected Auxiliary Space:** O(1).

**Constraints:**

1 <= number of nodes <= 103
0 <= value of nodes <= 103


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
        self.prev = None
'''

def reverseDLL(head):
    #return head after reversing



#{ 
 # Driver Code Starts
#Initial Template for Python 3

#contributed by RavinderSinghPB
class Node: 
    def __init__(self, data): 
        self.data = data  
        self.next = None
        self.prev = None
  
class DoublyLinkedList: 
    def __init__(self): 
        self.head = None
   
    def push(self, new_data,tail):
        if not self.head:
            self.head=Node(new_data)
            return self.head
        Nnode=Node(new_data)
        Nnode.prev=tail
        tail.next=Nnode
        return Nnode
        
    def printList(self, node): 
        while(node is not None): 
            print (node.data,end=' ') 
            node = node.next
            

            
if __name__ == '__main__':
    t=int(input())
    
    for tcs in range(t):
        n=int(input())
        arr=[int(x) for x in input().split()]
        
        
        dll=DoublyLinkedList()
        tail=None
        
        for e in arr:
            tail=dll.push(e,tail)
        
        resHead=reverseDLL(dll.head)
        dll.printList(resHead)
        print()
        
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Insert in Sorted way in a Sorted DLL
</Summary>

### **Insert in Sorted way in a Sorted DLL**
**Difficulty Level : Easy**

Last Week Of Job Fair 2023. Explore Unlimited Opportunities Now!
Given a sorted doubly linked list and an element X, your need to insert the element X into correct position in the sorted DLL.

Example:1

Input:
LinkedList:
3  
X = 9
Output:

#### **Your Task:**
You only need to complete the function sortedInsert() that takes head reference and x as arguments and returns the head of the modified list. The printing and checking tasks are done by the driver code.

**Expected Time Complexity:** O(n).

**Expected Auxiliary Space:** O(1).

**Constraints:**

1 <= Number of nodes <= 103


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
        self.prev = None
'''

def sortedInsert(head, x):
    #code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

# contributed by RavinderSinghPB
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None
        self.prev = None


class doublyLL:
    def __init__(self):
        self.head = None

    def insert(self, tail, data):
        head = self.head

        node = Node(data)

        if not head:
            self.head = node
            return node

        tail.next = node
        node.prev = tail
        return node


def displayList(head):
    pvs=None
    while head:
        print(head.data, end=' ')
        if head.prev !=pvs:
            print('prev pointer not connected')
        pvs = head
        head = head.next
        


if __name__ == '__main__':
    tcs = int(input())

    for _ in range(tcs):
        n = int(input())
        arr = [int(x) for x in input().split()]
        x = int(input())

        dll = doublyLL()

        tail = None

        for nodeData in arr:
            tail = dll.insert(tail, nodeData)

        dll.head=sortedInsert(dll.head, x)
        displayList(dll.head)
        print()




# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Compare Circular Doubly Linked Lists
</Summary>

### **Compare Circular Doubly Linked Lists**
**Difficulty Level : Easy**

Last Week Of Job Fair 2023. Explore Unlimited Opportunities Now!
Given two circular doubly linked lists of sizes n1 and n2 respectively, the task is check if the corresponding elements of the lists are same or not.
The tail of a circular doubly linked list is connected to head via its next pointer, and the previous pointer of head is connected to the tail.

#### **Example 1:**

    Input:
    LinkedList1: 1
    LinkedList2: 1
    Output: 1
#### **Example 2:**

    Input:
    LinkedList1: 2<->5<->7<->8<->99<->100
    LinkedList2: 7<->8<->9<->73<->2
    Output: 0
#### **Your Task:**
The task is to complete the function compareCLL() which takes head1 and head2 references as an arguments. The function should return true if all the corresponding elements of the lists are same, else it should return false. (The driver's code print 1 if the returned value is true, otherwise false.)

**Expected Time Complexity:** O(n1 + n2).

**Expected Auxiliary Space:** O(1).

**Constraints:**

1 <= number of nodes <= 105


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    def compareCLL(self,head1,head2):
        #code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

#contributed by RavinderSinghPB
class Node:
    def __init__(self,data):
        self.data=data
        self.next=None
        self.prev=None

class doublyLL:
    def __init__(self):
        self.head=None

    def insert(self,tail,data):
        head=self.head

        node=Node(data)

        if not head:

            self.head=node
            return node

        tail.next=node
        node.prev=tail
        return node

def getLength(head):
    temp=head
    count=1
    while(temp.next!=head):
        temp=temp.next
        count+=1
    return count
    

if __name__=='__main__':
    tcs=int(input())

    for _ in range(tcs):
        n1=int(input())
        arr1=[int(x) for x in input().split()]
        n2=int(input())
        arr2=[int(x) for x in input().split()]

        dll1=doublyLL()
        tail=None
        for nodeData in arr1:
            tail=dll1.insert(tail,nodeData)

        # making circular
        tail.next = dll1.head
        dll1.head.prev = tail

        dll2 = doublyLL()
        tail = None
        for nodeData in arr2:
            tail = dll2.insert(tail, nodeData)

        # making circular
        tail.next = dll2.head
        dll2.head.prev = tail
        ob=Solution()
        if(ob.compareCLL(dll1.head,dll2.head)):
            print(1)
        else:
            print(0)




# } Driver Code Ends
```

</details>


</details> 