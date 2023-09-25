### List of Questions
1. Length of String
2. Count Distinct Vowels in String
3. Vowels in String
4. Lowercase to Upercase
5. Uppercase to Lowercase
6. Reverse a String
7. Anagram
8. Pangram Checking
9. Missing Characters in Panagram
10. Count Words in String
11. String Validation

-----

##  Details of Questions Listed Above

<details>
<summary>
Length of String
</Summary>

### **Length of String**
**Difficulty Level : Basic** 

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 
You are given a string s. You need to find the length of the string.

#### **Example 1:**

    Input:
    s = Geeks
    Output: 
    5
#### **Example 2:**

    Input:
    s = Hello1234
    Output: 
    9
#### **Your Task:**
You only need to complete the function lengthString() that takes s as parameter and returns the length of the string. 

**Expected Time Complexity:** O(1).

**Expected Auxiliary Space:** O(1).

**Constraints:**

1 <= | s |  <= 100000


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
def lengthString(self, str):
    #code here
    


#{ 
 # Driver Code Starts
#Initial Template for Python 3

#contributed by RavinderSinghPB
if __name__ =='__main__':
    tcs = int(input())
    
    for _ in range(tcs):
        s=input()
        
        print(Solution().lengthString(s))
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Count Distinct Vowels in String
</Summary>

### **Count Distinct Vowels in String**
**Difficulty Level : Basic**

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 
You are given a string s. You need to count the total distinct vowels in the string. The string s contains lowercase letters only.

#### **Example 1:**

    Input:
    geeks
    
    Output: 
    1
#### **Example 2:**

    Input:
    world
    
    Output:
    1
#### **Your Task:**

You only need to complete the function countVowels() that takes s as parameter and returns the count of distinct vowels in the string. 

**Expected Time Complexity:** O(|S|).

**Expected Auxiliary Space:** O(1).

**Constraints:**

1 <= |s| <= 10000


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    def countVowels(self,s):
        #code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

#contributed by RavinderSinghPB
if __name__ == '__main__':
    tcs=int(input())
    
    for _ in range(tcs):
        s=input()
        obj = Solution()
        print(obj.countVowels(s))
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Vowels in String
</Summary>

#### **Vowels in String**
**Difficulty Level : Basic**

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 
You are given a string s. You need to count the total vowels in the string. The string s contains lowercase letters only.

#### **Example 1:**

    Input:
    s = geeks
    Output: 
    2
#### **Example 2:**

    Input:
    s = world
    Output: 
    1
#### **Your Task:**

You only need to complet the function countVowels() that takes s as parameter and returns the count of vowels in the string. 

**Expected Time Complexity:** O(|S|).

**Expected Auxiliary Space:** O(1).

**Constraints:**

1 <= |s| <= 10000


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    def countVowels(self,s):
        #code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

#contributed by RavinderSinghPB
if __name__ == '__main__':
    tcs=int(input())
    
    for _ in range(tcs):
        s=input()
        obj = Solution()
        print(obj.countVowels(s))
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Lowercase to Upercase
</Summary>

### **Lowercase to Upercase**
**Difficulty Level : Basic**

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 
You are given a string s. You need to convert the case of lowercase letter to uppercase letters.

#### **Example 1:**

    Input:
    Geeks
    Output: 
    GEEKS
#### **Example 2:**

    Input:
    for
    Output: 
    FOR
#### **Your Task:**

You only need to complete the function caseConversion() that takes s as parameter and returns the  converted string. 

**Expected Time Complexity:** O(|S|).

**Expected Auxiliary Space:** O(1).

**Constraints:**

1 <= |s| <= 10000


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    def caseConversion(self,s):


#{ 
 # Driver Code Starts
#Initial Template for Python 3

if __name__ == "__main__":
    t = int(input())
    while(t>0):
        s = input()
        obj = Solution()
        print(obj.caseConversion(s))
        t = t-1

# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Uppercase to Lowercase
</Summary>

### **Uppercase to Lowercase**
**Difficulty Level : Easy**

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 
You are given a string s. You need to convert the case of uppercase letters to lowercase letters.

#### **Example 1:**

    Input:
    GeekS
    
    Output: 
    geeks
#### **Example 2:**

    Input:
    FOR
    
    Output: 
    for
#### **Your Task:**

You only need to complete the function caseConversion() that takes s as parameter and returns the converted string. 

**Expected Time Complexity:** O(|S|).

**Expected Auxiliary Space:** O(1).

**Constraints:**

1 <= |s| <= 10000


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

"""
input -
@s :- string to be converted

output - 
return converted string 
"""
class Solution:
    def caseConversion(self,s):
       #your code here



#{ 
 # Driver Code Starts
#Initial Template for Python 3

if __name__ == "__main__":
    t = int(input())
    while(t>0):
        s = input()
        obj = Solution()
        print(obj.caseConversion(s))
        t = t-1

# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Reverse a String
</Summary>

### **Reverse a String**
**Difficulty Level : Basic**
Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 
You are given a string s. You need to reverse the string.

#### **Example 1:**

    Input:
    s = Geeks
    Output: skeeG
#### **Example 2:**
Input:
    s = for
    Output: rof
    
#### **Your Task:**

You only need to complete the function reverseWord() that takes s as parameter and returns the reversed string.

**Expected Time Complexity:** O(|S|).

**Expected Auxiliary Space:** O(1).

**Constraints:**

1 <= |s| <= 10000


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

def reverseWord(s):
    #your code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

if __name__ == "__main__":
    t = int(input())
    while(t>0):
        s = input()
        print(reverseWord(s))
        t = t-1

# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Anagram
</Summary>

### **Anagram**
**Difficulty Level : Easy**

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 
Given two strings a and b consisting of lowercase characters. The task is to check whether two given strings are an anagram of each other or not. An anagram of a string is another string that contains the same characters, only the order of characters can be different. For example, act and tac are an anagram of each other.

Note:-

If the strings are anagrams you have to return True or else return False

|s| represents the length of string s.


#### **Example 1:**

    Input:a = geeksforgeeks, b = forgeeksgeeks
    Output: YES
    Explanation: Both the string have same characters with
            same frequency. So, both are anagrams.
#### **Example 2:**

    Input:a = allergy, b = allergic
    Output: NO
    Explanation: Characters in both the strings are 
            not same, so they are not anagrams.
#### **Your Task:**
You don't need to read input or print anything. Your task is to complete the function isAnagram() which takes the string a and string b as input parameter and check if the two strings are an anagram of each other. The function returns true if the strings are anagram else it returns false.

**Expected Time Complexity:**O(|a|+|b|).

**Expected Auxiliary Space:** O(Number of distinct characters).

**Constraints:**

1 ≤ |a|,|b| ≤ 105


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3


class Solution:
    
    #Function is to check whether two strings are anagram of each other or not.
    def isAnagram(self,a,b):
        #code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

if __name__=='__main__':
    t = int(input())
    for i in range(t):
        a,b=map(str,input().strip().split())
        if(Solution().isAnagram(a,b)):
            print("YES")
        else:
            print("NO") 
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Pangram Checking
</Summary>


### **Pangram Checking**
**Difficulty Level : Bacic**

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 
You are given a string s. You need to find if the string is a panagram or not.
A panagram contains all the letters of english alphabet at least once.

#### **Example 1:**

    Input:
    s = Thequickbrownfoxjumpsoverthelazydog
    Output: 1
#### **Example 2:**

    Input:
    s = HeavyDuty
    Output: 0
#### **Your Task:**

You only need to complete the function isPanagram() that takes s as parameter and returns either true or false. (the driver's code print 1 if the returned value is true, otherwise 0)

**Expected Time Complexity:** O(|S|).

**Expected Auxiliary Space:** O(1).

**Constraints:**

1 <= |s| <= 10000

#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

"""
input - 
s - given string 

output - 
return 0 if not panagram else return 1
"""
class Solution:
    def isPanagram(self,s):
        #your code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

if __name__ == "__main__":
    t = int(input())
    while(t>0):
        s = input()
        print(int(Solution().isPanagram(s)))
        t = t-1

# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Missing Characters in Panagram
</Summary>

#### **Missing Characters in Panagram**
**Difficulty Level : Bacic**

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 
You are given a string s. You need to find the missing characters in the string to make a panagram ( a sentence using every letter of english alphabet at least once ).
Note: The output characters will be lowercase and lexicographically sorted.

 

#### **Example 1:**

    Input:
    s = Abcdefghijklmnopqrstuvwxy
    Output: z
     

#### **Example 2:**

    Input:
    s = Abc
    Output: defghijklmnopqrstuvwxyz
 

#### **Your Task:**

You only need to complete the function misssingPanagram() that takes s as parameter and returns -1 if the string is a panagram, else it returns a string that consists missing characters.

 

**Expected Time Complexity:** O(|S|).

**Expected Auxiliary Space:** O(1).

 

**Constraints:**
1 <= |s| <= 10000


#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

"""
input - 
@s = given string 

output - 
return -1 or required ans
"""
class Solution:
    def missingPanagram(self, s):



#{ 
 # Driver Code Starts
#Initial Template for Python 3

if __name__ == "__main__":
    t = int(input())
    while(t>0):
        s = input()
        obj = Solution()
        print(obj.missingPanagram(s))
        t = t-1

# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
Count Words in String
</Summary>


#### **Count Words in String**
**Difficulty Level : Bacic**

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 
You are given a string s consisting of multiple words. You need to count the total words in the string. Words are separated by a single space.
Note: It is guaranteed that the last character of the given string is not a white space.

#### **Example 1:**
    Input:
    s = Geeks
    
    Output: 
    1
#### **Example 2:**

    Input:
    s = World is hello
    
    Output: 
    3
#### **Your Task:**

You only need to complet the function countWords() that takes s as parameter and returns the count of words in the string. 

**Expected Time Complexity:** O(|S|).

**Expected Auxiliary Space:** O(1).

**Constraints:**

1 <= |s| <= 10000

#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

class Solution:
    def countWords(self,s):
        #code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

#contributed by RavinderSinghPB
if __name__ == '__main__':
    tcs=int(input())
    
    for _ in range(tcs):
        s=input()
        obj = Solution()
        print(obj.countWords(s))
# } Driver Code Ends
```

</details>


</details>

<details>
<summary>
String Validation
</Summary>


### **String Validation**
**Difficulty Level : Bacic**

Join the most popular course on DSA. Master Skills & Become Employable by enrolling today! 
Given a string s representing a password, you need to check if the string is valid or not. A valid string has the following properties:

    String must have the length greater than or equal to 10.
    String must contain at least 1 numeric character.
    String must contain at least 1 uppercase character.
    String must contain at least 1 lowercase character.
    String must contain at least 1 special character from @#$-*.
 

#### **Example 1:**

    Input: eHello123@
    Output: 1
    Explanation: String is valid.

 

#### **Example 2:**

    Input: hella
    Output: 0
    Explanation: String is not valid.
 

#### **Your Task:**
You don't need to read input or print anything. Complete the function validate() which takes string s as input parameter and returns true if the string is valid, else it returns false.
 

**Expected Time Complexity:** O(|S|).

**Expected Auxiliary Space:** O(1).

 

**Constraints:**

1 ≤ |s| ≤ 103

#### **Python Code Template**

<details>
<summary>Expand For Python Code Template</summary>

```python
#User function Template for python3

"""
input - 
s = string given 

output - 
return 0 if not validated else return true
"""

def validate(s):
    #your code here


#{ 
 # Driver Code Starts
#Initial Template for Python 3

if __name__ == "__main__":
    t = int(input())
    while(t>0):
        s = input()
        print(validate(s))
        t = t-1

# } Driver Code Ends
```

</details>


</details>

