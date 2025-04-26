# EX 1A Reverse a String
## DATE:
## AIM:
To write a program to create a recursive function to reverse a string.

## Algorithm
1. 
2. 
3. 
4.  
5.   

## Program:
```
/*
Program to implement Reverse a String
Developed by: 
Register Number:

def reverse_string(s):
    """
    Recursive function to reverse a string
    """
    if len(s) <= 1:  # base case: if the string is empty or has only one character, return it as is
        return s
    else:
        return reverse_string(s[1:]) + s[0]  


input_string = input()
reversed_string = reverse_string(input_string)
print(reversed_string) 
*/
```

## Output:
![Screenshot 2025-04-26 101504](https://github.com/user-attachments/assets/7bac129d-03e6-4500-8171-c22addc6f7f2)




## Result:
The program successfully reverses the input string using recursion. When the user provides an input string, the output displays the reversed version of the string
