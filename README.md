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
Objective: Create a function named **rotate_word()** that accepts a non-empty string, moving the first character of the string to the end while keeping all remaining characters in their original order, and preserving the capitalization of every character.

 The following operations were utilized in constructing the function:
 
- `text[1::1]` ---> String splicing which stores the individual characters of a given string excluding the first character. The format [1::1] indicates that the character to be stored starts at index 1, or the second character, while keeping track of each following character at single index increments. The ": :" indicates that the operation will continue until the last character of the string.
- `text[0]` ---> String indexing used to store the first character of a given string, denoting that the character is located at index 0.
- `+` ---> Addition operation to add the individual components together.

The operations were combined to create a function that retrieves the first character of a string, tracking the remaining string characters, and placing the first character at the end of the string;


