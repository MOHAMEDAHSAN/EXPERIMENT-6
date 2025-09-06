
### Name : S Mohamed Ahsan
### Reg No : 212223240089

# EXPERIMENT-6

## AIM:
To write a Python program for checking Palindrome and to write test cases for ir. 

## ALGORITHM

Step 1: Start
Step 2: Get an input from the user by prompting
Step 3: Run a loop form 0 to len/2.
Step 4: Check if the characters are the same both from the start and the end till len/2.
Step 5: If it is, return the result that it is a palindrome.
Step 6: Else, return that it is not a palindrome.
Step 7: Stop. 

## PROGRAM
```python
def Palindrome(string):
    for i in range(0, int(len(string) / 2)):
        if string[i] != string[len(string) - i - 1]:  # Fixed indexing
            return False
    return True


s = input("Enter a string: ")  # Added a prompt for clarity

c = 1
for i in s:
    if not i.isalpha():
        c = 0
        break  # Added break to stop checking after finding a non-alphabetic character

if c == 0:
    print("Enter a valid string")
    print("Test Case:Fail")
else:
    answer = Palindrome(s)
    if answer:
        print("The given string is a palindrome")
        print("Test Case:Pass")
    else:
        print("The given string is not a palindrome")
        print("Test Case:Pass") 

```
## OUTPUT
<img width="550" height="150" alt="image" src="https://github.com/user-attachments/assets/77d607c3-a27c-4220-b2ea-cf79afb5de5c" />

## RESULT
hus,python program for checking Palindrome and to write test cases for ir is successfully executed.
