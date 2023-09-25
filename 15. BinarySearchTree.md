### list of Questions
1. Search a node in BST
2. Insert a node in a BST
3. Delete a node from BST
4. Preorder in BST
5. Inorder in BST
6. Postorder in BST
7. Level Order in BST
8. Floor in BST
9. Ceil in BST
10. Minimum element in BST


----



## Details of Questions Listed Above

<details>
<summary>
Search a node in BST
</Summary>

### **Search a node in BST**
**Difficulty Level : Basic** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 
Given a Binary Search Tree and a node value X, find if the node with value X is present in the BST or not.


#### **Example 1:**

    Input:         2
                    \
                     81 
                   /    \ 
                 42      87 
                  \       \ 
                   66      90 
                  / 
                45
    X = 87
    Output: 1
    Explanation: As 87 is present in the
    given nodes , so the output will be
    1.
#### **Example 2:**

    Input:      6
                 \ 
                  8 
                 / \ 
                7   9
    X = 11
    Output: 0
    Explanation: As 11 is not present in 
    the given nodes , so the output will
    be 0.

#### **Your Task:**
You don't need to read input or print anything. Complete the function search()which returns true if the node with value x is present in the BSTelse returns false.


**Expected Time Complexity:** O(Height of the BST)

**Expected Auxiliary Space:** O(1).


**Constraints:**

1 <= Number of nodes <= 105


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#Your task is to complete this function

class BST:
    
    #Function to search a node in BST.
    def search(self, node, x):
        #code here




#{ 
 # Driver Code Starts
class Node:
    """ Class Node """
    def __init__(self, value):
        self.left = None
        self.data = value
        self.right = None

class Tree:
    def createNode(self, data):
        return Node(data)
    
    def insert(self, node, data):
        if node is None:
            return self.createNode(data)
        else:
            if data < node.data:
                node.left = self.insert(node.left, data)
            else:
                node.right = self.insert(node.right, data)
            return node

    def traverseInorder(self, root):
        if root is not None:
            print(root.data, end= " ")
            self.traverseInorder(root.left)
            self.traverseInorder(root.right)
    
if __name__=='__main__':
    t=int(input())
    for i in range(t):
        n=int(input())
        arr = input().strip().split()
        root = None
        tree = Tree()
        root = tree.insert(root, int(arr[0]))
        for j in range(1, n):
            root = tree.insert(root, int(arr[j]))
        #tree.traverseInorder(root)
        num = int(input())
        find = BST()
        if find.search(root, num):
            print(1)
        else:
            print(0)

# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Insert a node in a BST
</Summary>

### **Insert a node in a BST**
**Difficulty Level : Easy** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 
Given a BST and a key K. If K is not present in the BST, Insert a new Node with a value equal to K into the BST. 
Note: If K is already present in the BST, don't modify the BST.


#### **Example 1:**

    Input:
         2
       /   \
      1     3
    K = 4
    Output: 1 2 3 4
    Explanation: After inserting the node 4
    Inorder traversal will be 1 2 3 4.
#### **Example 2:**

    Input:
            2
          /   \
         1     3
                 \
                  6
    K = 4
    Output: 1 2 3 4 6
    Explanation: After inserting the node 4
    Inorder traversal of the above tree
    will be 1 2 3 4 6.

#### **Your Task:**
You don't need to read input or print anything. Your task is to complete the function insert() which takes the root of the BST and Key K as input parameters and returns the root of the modified BST after inserting K. 
Note: The generated output contains the inorder traversal of the modified tree.


**Expected Time Complexity:** O(Height of the BST).

**Expected Auxiliary Space:** O(Height of the BST).


**Constraints:**

1 <= Number of nodes initially in BST <= 105
1 <= K <= 106


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3


#Function to insert a node in a BST. 
def insert(root, Key):
    # code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

from collections import deque
# Tree Node
class Node:
    def __init__(self, val):
        self.right = None
        self.data = val
        self.left = None

# Function to Build Tree   
def buildTree(s):
    #Corner Case
    if(len(s)==0 or s[0]=="N"):           
        return None
        
    # Creating list of strings from input 
    # string after spliting by space
    ip=list(map(str,s.split()))
    
    # Create the root of the tree
    root=Node(int(ip[0]))                     
    size=0
    q=deque()
    
    # Push the root to the queue
    q.append(root)                            
    size=size+1 
    
    # Starting from the second element
    i=1                                       
    while(size>0 and i<len(ip)):
        # Get and remove the front of the queue
        currNode=q[0]
        q.popleft()
        size=size-1
        
        # Get the current node's value from the string
        currVal=ip[i]
        
        # If the left child is not null
        if(currVal!="N"):
            
            # Create the left child for the current node
            currNode.left=Node(int(currVal))
            
            # Push it to the queue
            q.append(currNode.left)
            size=size+1
        # For the right child
        i=i+1
        if(i>=len(ip)):
            break
        currVal=ip[i]
        
        # If the right child is not null
        if(currVal!="N"):
            
            # Create the right child for the current node
            currNode.right=Node(int(currVal))
            
            # Push it to the queue
            q.append(currNode.right)
            size=size+1
        i=i+1
    return root

def inOrder(n):
    if n is None:
        return
    inOrder(n.left)
    print(n.data, end=' ')
    inOrder(n.right)

if __name__=="__main__":
    t=int(input())
    for _ in range(0,t):
        s=input()
        root=buildTree(s)
        k=int(input())
        insert(root,k)
        inOrder(root)
        print()
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Delete a node from BST
</Summary>

### **Delete a node from BST**
**Difficulty Level : Medium** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 
Given a Binary Search Tree and a node value X. Delete the node with the given value X from the BST. If no node with value x exists, then do not make any change. 

#### **Example 1:**

    Input:
          2
        /   \
       1     3
    X = 12
    Output: 1 2 3
    Explanation: In the given input there
    is no node with value 12 , so the tree
    will remain same.
#### **Example 2:**

    Input:
                1
                 \
                  2
                    \
                     8 
                   /    \
                  5      11
                /  \    /  \
               4    7  9   12
    X = 9
    Output: 1 2 4 5 7 8 11 12
    Explanation: In the given input tree after
    deleting 9 will be
                 1
                  \
                   2
                     \
                      8
                     /   \
                    5     11
                   /  \     \
                  4    7     12
#### **Your Task:**
You don't need to read input or print anything. Your task is to complete the function deleteNode() which takes two arguments. The first being the root of the tree, and an integer 'X' denoting the node value to be deleted from the BST. Return the root of the BST after deleting the node with value X. Do not make any update if there's no node with value X present in the BST.

Note: The generated output will be the inorder traversal of the modified tree.
 

**Expected Time Complexity:** O(Height of the BST).

**Expected Auxiliary Space:** O(Height of the BST).
 

**Constraints:**

1 <= N <= 105




#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3


#Function to delete a node from BST.
def deleteNode(root, X):
    # code here.


#{ 
 # Driver Code Starts
#Initial Template for Python 3
from collections import deque
# Tree Node
class Node:
    def __init__(self, val):
        self.right = None
        self.data = val
        self.left = None

# Function to Build Tree   
def buildTree(s):
    #Corner Case
    if(len(s)==0 or s[0]=="N"):           
        return None
        
    # Creating list of strings from input 
    # string after spliting by space
    ip=list(map(str,s.split()))
    
    # Create the root of the tree
    root=Node(int(ip[0]))                     
    size=0
    q=deque()
    
    # Push the root to the queue
    q.append(root)                            
    size=size+1 
    
    # Starting from the second element
    i=1                                       
    while(size>0 and i<len(ip)):
        # Get and remove the front of the queue
        currNode=q[0]
        q.popleft()
        size=size-1
        
        # Get the current node's value from the string
        currVal=ip[i]
        
        # If the left child is not null
        if(currVal!="N"):
            
            # Create the left child for the current node
            currNode.left=Node(int(currVal))
            
            # Push it to the queue
            q.append(currNode.left)
            size=size+1
        # For the right child
        i=i+1
        if(i>=len(ip)):
            break
        currVal=ip[i]
        
        # If the right child is not null
        if(currVal!="N"):
            
            # Create the right child for the current node
            currNode.right=Node(int(currVal))
            
            # Push it to the queue
            q.append(currNode.right)
            size=size+1
        i=i+1
    return root
    
# A utility function to do inorder traversal of BST 
def inorder(root): 
    if root is not None: 
        inorder(root.left) 
        print (root.data, end=' '),
        inorder(root.right) 
    
    
if __name__=="__main__":
    t=int(input())
    for _ in range(0,t):
        s=input()
        x=int(input())
        root=buildTree(s)
        root = deleteNode(root,x)
        inorder(root)
        print()
        
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Preorder in BST
</Summary>

### **Preorder in BST**
**Difficulty Level : Basic** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 
Given a Binary Search Tree of size N, find its preorder traversal.

#### **Example 1:**

    Input :
    N = 5
           3
          / \  
         1   4 
          \   \   
           2   5
    
    Output: 3 1 2 4 5
#### **Example 2:**

    Input :
    N = 3
           1
            \
             2 
              \
               3 
    
    Output: 1 2 3

#### **Your Task:**  
You dont need to read input or print anything. Complete the function preOrder() which takes the root of the tree as input parameter and returns a list of integers denoting preorder traversal of the BST.


**Expected Time Complexity:** O(N)

**Expected Auxiliary Space:** O(N)


**Constraints:**

1 ≤ N ≤ 100


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

'''
@Node structure -
class Node:
    def __init__(self,key):
        self.left = None
        self.right = None
        self.val = key
'''
def preOrder(root):
    #code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

class Node:
    def __init__(self,key):
        self.left = None
        self.right = None
        self.val = key

def insert(root,node):
    if root == None:
        root = node
    else:
        if root.val < node.val:
            if root.right is None:
                root.right = node
            else:
                insert(root.right, node)
        else:
            if root.left is None:
                root.left = node
            else:
                insert(root.left, node)

if __name__ == "__main__":
    t = int(input())
    for ti in range(t):
        n = int(input())
        arr = [int(x) for x in input().strip().split()]
        root = Node(arr[0])
        for i in range(1, n):
            insert(root, Node(arr[i]))
        res = preOrder(root)
        for i in range (len (res)):
            print (res[i], end = " ")
        print()

# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Inorder in BST
</Summary>

### **Inorder in BST**
**Difficulty Level : Basic** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 
Given a Binary Search Tree of size N, find its inorder traversal.

#### **Example 1:**

    Input :
    N = 5
           3
          / \  
         1   4 
          \   \   
           2   5
    
    Output: 1 2 3 4 5 
#### **Example 2:**

    Input :
    N = 3
           1
            \
             2 
              \
               3 
    
    Output: 1 2 3

#### **Your Task:**  
You dont need to read input or print anything. Complete the function inOrder() which takes the root of the tree as input parameter and returns a list of integers denoting inorder traversal of the BST.


**Expected Time Complexity:** O(N)

**Expected Auxiliary Space:** O(N)


**Constraints:**

1 ≤ N ≤ 100




#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

"""
@Node Template -
class Node:
    def __init__(self,key):
        self.left = None
        self.right = None
        self.val = key
"""
def InOrder(root):
    #code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

class Node:
    def __init__(self,key):
        self.left = None
        self.right = None
        self.val = key

def insert(root,node):
    if root == None:
        root = node
    else:
        if root.val < node.val:
            if root.right is None:
                root.right = node
            else:
                insert(root.right, node)
        else:
            if root.left is None:
                root.left = node
            else:
                insert(root.left, node)


if __name__ == "__main__":
    t = int(input())
    for ti in range(t):
        n = int(input())
        arr = [int(x) for x in input().strip().split()]
        root = Node(arr[0])
        for i in range(1, n):
            insert(root, Node(arr[i]))
        res = InOrder(root)
        for i in range (len(res)):
            print (res[i], end=" ")
        print()

# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Postorder in BST
</Summary>

#### **Postorder in BST**
**Difficulty Level : Basic** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 
Given a Binary Search Tree of size N, find its postorder traversal.

#### **Example 1:**

    Input :
    N = 5
           3
          / \  
         1   4 
          \   \   
           2   5
    
    Output: 2 1 5 4 3
#### **Example 2:**

    Input :
    N = 3
           1
            \
             2 
              \
               3 
    
    Output: 3 2 1

#### **Your Task:**  
You dont need to read input or print anything. Complete the function postOrder() which takes the root of the tree as input parameter and returns a list of integers denoting postorder traversal of the BST.


**Expected Time Complexity:** O(N)

**Expected Auxiliary Space:** O(N)


**Constraints:**

1 ≤ N ≤ 100


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

'''
@Node Template - 
class Node:
    def __init__(self,key):
        self.left = None
        self.right = None
        self.val = key
'''
def postOrder(root):
    #code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

class Node:
    def __init__(self,key):
        self.left = None
        self.right = None
        self.val = key

def insert(root,node):
    if root == None:
        root = node
    else:
        if root.val < node.val:
            if root.right is None:
                root.right = node
            else:
                insert(root.right, node)
        else:
            if root.left is None:
                root.left = node
            else:
                insert(root.left, node)

        

if __name__ == "__main__":
    t = int(input())
    for ti in range(t):
        n = int(input())
        arr = [int(x) for x in input().strip().split()]
        root = Node(arr[0])
        for i in range(1, n):
            insert(root, Node(arr[i]))
        res = postOrder(root)
        for i in range (len (res)):
            print (res[i], end = " ")
        print()

# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Levelorder in BST
</Summary>

#### **Levelorder in BST**
**Difficulty Level : Basic** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 
Given a Binary Search Tree of size N, find its level-order traversal.

#### **Example 1:**

    Input :
    N = 5
           3
          / \  
         1   4 
          \   \   
           2   5
    
    Output: 3 1 4 2 5
#### **Example 2:**

    Input :
    N = 3
           1
            \
             2 
              \
               3 
    
    Output: 1 2 3

#### **Your Task:**  
You dont need to read input or print anything. Complete the function levelOrder() which takes the root of the tree as input parameter and returns a list of integers denoting level-order traversal of the BST.


**Expected Time Complexity:** O(N)

**Expected Auxiliary Space:** O(N)


**Constraints:**

1 ≤ N ≤ 100


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

'''
@node template - 
class Node:
    def __init__(self,key):
        self.left = None
        self.right = None
        self.val = key
'''
def levelOrder(root):
    #code here 


#{ 
 # Driver Code Starts
#Initial Template for Python 3

class Node:
    def __init__(self,key):
        self.left = None
        self.right = None
        self.val = key



def height(node):
    if node is None:
        return 0
    else :
        lheight = height(node.left)
        rheight = height(node.right)

        if lheight > rheight :
            return lheight+1
        else:
            return rheight+1

def insert(root,node):
    if root == None:
        root = node
    else:
        if root.val < node.val:
            if root.right is None:
                root.right = node
            else:
                insert(root.right, node)
        else:
            if root.left is None:
                root.left = node
            else:
                insert(root.left, node)


if __name__ == "__main__":
    t = int(input())
    for ti in range(t):
        n = int(input())
        arr = [int(x) for x in input().strip().split()]
        root = Node(arr[0])
        for i in range(1, n):
            insert(root, Node(arr[i]))
        res = levelOrder(root)
        for i in range (len (res)):
            print (res[i], end=" ")
        print()

# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Floor in BST
</Summary>

### **Floor in BST**
**Difficulty Level : Medium** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 
Given a Binary search tree and a value X,  the task is to complete the function which will return the floor of x.

Note: Floor(X) is an element that is either equal to X or immediately smaller to X. If no such element exits return -1.

#### **Example 1:**

    Input:
           8
         /  \
        5    9
       / \    \
      2   6   10
    X = 3
    Output: 2
    Explanation: Floor of 3 in the given BST
    is 2
#### **Example 2:**

    Input:
           3
         /   \
        2     5
            /  \
           4    7
          /
         3
    X = 1
    Output: -1
    Explanation: No smaller element exits
#### **Your task:**
You don't need to worry about the insert function, just complete the function floor() which should return the floor of X. If no such element exits return -1.

**Expected Time Complexity:** O(Height of the BST)

**Expected Auxiliary Space:** O(Height of the BST).

**Constraints:**

1 <= Number of nodes <= 105
1 <= X, Value of Node <= 106


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3


#Function to return the floor of given number in BST.
def floor(root,x):
    # code here



#{ 
 # Driver Code Starts
#Initial Template for Python 3

from collections import deque

# Tree Node
class Node:
    def __init__(self, val):
        self.right = None
        self.data = val
        self.left = None

# Function to Build Tree   
def buildTree(s):
    #Corner Case
    if(len(s)==0 or s[0]=="N"):           
        return None
        
    # Creating list of strings from input 
    # string after spliting by space
    ip=list(map(str,s.split()))
    
    # Create the root of the tree
    root=Node(int(ip[0]))                     
    size=0
    q=deque()
    
    # Push the root to the queue
    q.append(root)                            
    size=size+1 
    
    # Starting from the second element
    i=1                                       
    while(size>0 and i<len(ip)):
        # Get and remove the front of the queue
        currNode=q[0]
        q.popleft()
        size=size-1
        
        # Get the current node's value from the string
        currVal=ip[i]
        
        # If the left child is not null
        if(currVal!="N"):
            
            # Create the left child for the current node
            currNode.left=Node(int(currVal))
            
            # Push it to the queue
            q.append(currNode.left)
            size=size+1
        # For the right child
        i=i+1
        if(i>=len(ip)):
            break
        currVal=ip[i]
        
        # If the right child is not null
        if(currVal!="N"):
            
            # Create the right child for the current node
            currNode.right=Node(int(currVal))
            
            # Push it to the queue
            q.append(currNode.right)
            size=size+1
        i=i+1
    return root

if __name__=="__main__":
    for _ in range(int(input())):
        root = buildTree(input())
        x = int(input())
        print(floor(root,x))

# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Ceil in BST
</Summary>

#### **Ceil in BST**
**Difficulty Level : Medium** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 
Given a BST and a number X, find Ceil of X.
Note: Ceil(X) is a number that is either equal to X or is immediately greater than X.

#### **Example 1:**

    Input:
          5
        /   \
       1     7
        \
         2 
          \
           3
    X = 3
    Output: 3
    Explanation: We find 3 in BST, so ceil
    of 3 is 3.
#### **Example 2:**

    Input:
         10
        /  \
       5    11
      / \ 
     4   7
          \
           8
    X = 6
    Output: 7
    Explanation: We find 7 in BST, so ceil
    of 6 is 7.
#### **Your task:**
You don't need to read input or print anything. Just complete the function findCeil() to implement ceil in BST which returns the ceil of X in the given BST.

**Expected Time Complexity:** O(Height of the BST)

**Expected Auxiliary Space:** O(Height of the BST).

**Constraints:**

1 <= Number of nodes <= 105
1 <= Value of nodes<= 105


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#Function to return the ceil of given number in BST.

class Solution:
    def findCeil(self,root, inp):
        # code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

from collections import deque
# Tree Node
class Node:
    def __init__(self, val):
        self.right = None
        self.key = val
        self.left = None

# Function to Build Tree  

def buildTree(s):
        #Corner Case
        if(len(s)==0 or s[0]=="N"):           
            return None
            
        # Creating list of strings from input 
        # string after spliting by space
        ip=list(map(str,s.split()))
        
        # Create the root of the tree
        root=Node(int(ip[0]))                     
        size=0
        q=deque()
        
        # Push the root to the queue
        q.append(root)                            
        size=size+1 
        
        # Starting from the second element
        i=1                                       
        while(size>0 and i<len(ip)):
            # Get and remove the front of the queue
            currNode=q[0]
            q.popleft()
            size=size-1
            
            # Get the current node's value from the string
            currVal=ip[i]
            
            # If the left child is not null
            if(currVal!="N"):
                
                # Create the left child for the current node
                currNode.left=Node(int(currVal))
                
                # Push it to the queue
                q.append(currNode.left)
                size=size+1
            # For the right child
            i=i+1
            if(i>=len(ip)):
                break
            currVal=ip[i]
            
            # If the right child is not null
            if(currVal!="N"):
                
                # Create the right child for the current node
                currNode.right=Node(int(currVal))
                
                # Push it to the queue
                q.append(currNode.right)
                size=size+1
            i=i+1
        return root
    
    
if __name__=="__main__":
    t=int(input())
    for _ in range(0,t):
        s=input()
        n=int(input())
        root=buildTree(s)
        obj=Solution()
        print(obj.findCeil(root,n))
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Minimum element in BST
</Summary>

**Minimum element in BST**
**Difficulty Level : Basic** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 
Given a Binary Search Tree. The task is to find the minimum valued element in this given BST.

#### **Example 1:**

    Input:
               5
             /    \
            4      6
           /        \
          3          7
         /
        1
    Output: 1
#### **Example 2:**

    Input:
                 9
                  \
                   10
                    \
                     11
    Output: 9
#### **Your Task:**
The task is to complete the function minValue() which takes root as the argument and returns the minimum element of BST. If the tree is empty, there is no minimum element, so return -1 in that case.

**Expected Time Complexity:** O(Height of the BST)

**Expected Auxiliary Space:** O(1).

**Constraints:**

0 <= N <= 104


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

"""
class Node:
    def __init__(self, val):
        self.right = None
        self.data = val
        self.left = None
"""

#Function to find the minimum element in the given BST.
def minValue(root):
    ##Your code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

from collections import deque
# Tree Node
class Node:
    def __init__(self, val):
        self.right = None
        self.data = val
        self.left = None

# Function to Build Tree   
def buildTree(s):
    #Corner Case
    if(len(s)==0 or s[0]=="N"):           
        return None
        
    # Creating list of strings from input 
    # string after spliting by space
    ip=list(map(str,s.split()))
    
    # Create the root of the tree
    root=Node(int(ip[0]))                     
    size=0
    q=deque()
    
    # Push the root to the queue
    q.append(root)                            
    size=size+1 
    
    # Starting from the second element
    i=1                                       
    while(size>0 and i<len(ip)):
        # Get and remove the front of the queue
        currNode=q[0]
        q.popleft()
        size=size-1
        
        # Get the current node's value from the string
        currVal=ip[i]
        
        # If the left child is not null
        if(currVal!="N"):
            
            # Create the left child for the current node
            currNode.left=Node(int(currVal))
            
            # Push it to the queue
            q.append(currNode.left)
            size=size+1
        # For the right child
        i=i+1
        if(i>=len(ip)):
            break
        currVal=ip[i]
        
        # If the right child is not null
        if(currVal!="N"):
            
            # Create the right child for the current node
            currNode.right=Node(int(currVal))
            
            # Push it to the queue
            q.append(currNode.right)
            size=size+1
        i=i+1
    return root
    
    
if __name__=="__main__":
    t=int(input())
    for _ in range(0,t):
        s=input()
        root=buildTree(s)
        print(minValue(root))
# } Driver Code Ends
```

</details>


</details>