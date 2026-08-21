# ECE-2112-PA-1
**EXPERIMENT 1: INTRODUCTION TO PYTHON PROGRAMMING**

Rivera, Francis Carlo E. | 2ECE-D

The repository covers Programming Assignment 1 for our ECE2112: Advanced Computer Programming and Algorithms course. The PA contains three programming problems that utilize basic Python functions and operations to acquire desired outputs.

### OBJECTIVES / INTENDED LEARNING OUTCOMES
1. Use basic Python functions, operators, and string operations
2. Manipulate strings using indexing, slicing, and built-in string methods
3. Apply sequence unpacking to manipulate the elements of a list
4. Construct simple Python functions that return a specified result

# A. WORD ROTATION PROBLEM
> Objectives: 
> - Create a function named **rotate_word()** that accepts a non-empty string. Move the first character of the string to the end while keeping all remaining characters in their original order. Preserve the capitalization of every character.
> - Use string indexing or slicing to construct the returned string

The following operations were utilized in constructing the function **rotate_word()**:
 
- `text[1::1]` ---> String splicing which stores the individual characters of a given string excluding the first character. The format [1::1] indicates that the character to be stored starts at index 1, or the second character, while keeping track of each following character at single index increments. The ": :" indicates that the operation will continue until the last character of the string.
  
- `text[0]` ---> String indexing used to store the first character of a given string, denoting that the character is located at index 0.
  
- `+` ---> Addition operation used to add the individual components together.

The operations were combined to create a function that retrieves the first character of a string, tracking the remaining string characters, and placing the first character at the end of the string.

```
def rotate_word(text):
    return text[1::1]+text[0]
```

# B. USERNAME BUILDER PROBLEM
> Objectives:
> - Create a function named **make_username()** that accepts two strings: first name and last name. The
> function must:
> 1. convert all letters to lowercase
> 2. remove all spaces from the first name
> 3. remove all spaces from the last name
> 4. join the processed first and last names using one period (.)
> - Use basic string methods and string concatenation. Return the completed username.

The following operations were utilized in constructing the function **make_username**():
- `.replace(" ","")` ---> Character replacing which replaces the spaces in a given string with blank characters, denoted by the empty placeholder. The operation is used to remove spaces in a string.
  
- `.lower()` ---> Operation that converts all uppercase letters in a given string with lowercase letters before returning the new string.
  
- `first_name.replace(" ","").lower()` ---> String operation composed of the .lower() and .replace(" ","") for the conversion of the first name provided which is denoted by the first string placeholder in the function.
  
- `last_name.replace(" ","").lower()` ---> String operation composed of the .lower() and .replace(" ","") for the conversion of the last name provided which is denoted by the first string placeholder in the function.
  
- `"."` ---> Period character concatenated between the two strings.
  
- `+` ---> Addition operation which concatenates the two strings provided and the period character between them.

The operations were combined to create a function that accepts two strings, a first and last name, and converts all detected uppercase letters into lowercase letters while removing any spaces detected within the strings.

```
def make_username(first_name, last_name):
    return first_name.replace(" ","").lower()+"."+last_name.replace(" ","").lower()
```

# C. BOOKEND SWAP PROBLEM
> Objectives:
> - Create a function named **swap_bookends()** that accepts a list containing at least two elements. Unpack
> the list into three variables:
> 1. first – the first element
> 2. middle – a list containing everything between the first and last elements
> 3. last – the last element
> - Using these variables, return a new list in which the first and last elements have exchanged positions.
> The elements in middle must remain in their original order. Do not modify the input list.

The following operations were utilized in constructing the function **swap_bookends**():
- `first, *middle, last = items` ---> extended sequence unpacking which splits a given list of items into three sections, namely the first item, the last item, and the rest of the elements in between as middle items.

- `return last, *middle, first` ---> Operation that returns a new list wherein the last item is placed first while the first item is placed last.

The operations were combined to create a function that accepts a list of elements and returns a new list where the positions of the first and last item are interchanged while retaining the original positions of the elements in the middle.

```
def swap_bookends(items):
    first, *middle, last = items
    return last, *middle, first
```
# HISTORY
- August 20, 2026: README File created.
- August 20, 2026: Added content for Introductory and Part A of PA1.
- August 21 2026: Added content for Part B and Part C of PA1.
- August 21 2026: Jupyter Notebook File (.ipynb) uploaded.
