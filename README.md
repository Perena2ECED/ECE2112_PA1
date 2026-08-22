# ECE2112 PA1
__Paulene Anne V. Pereña | 2ECE-D__  
This repository contains the Programming Assignment 1 for the course _Advanced Computer Programming_ (ECE2112).  
This project consists of three Python problems assigned to _Module 1 - Base Computing with Python._
# A. WORD ROTATION PROBLEM
The first problem asked for a function that takes a string and returns a new string with the first character appended to the end, while the remaining characters retain their positions and capitalization.
The following functions and methods were used in this problem:
* `rotate_word(text)` - a user-defined function that shifts the first character of a string to the very end of that string while keeping its capitalization.
  > Example: `rotate_word("python")` --> "ythonp"
* `text[1: ]` --> a built-in function called as __string slicing__, where it extracts a subset of a string starting from index 1, known as the second letter, until the end of the word.
  > Example: `text1 = "python"` <br>    `print(text1[1: ]) --> ython`
* text[0] --> a built-in function called as __string indexing__, it focuses on accessing the character located at index 0, the first character of the word.
  > Example: `text1 = "python"` <br> `print(text1[0]) --> p`
* `+` -- > a built-in operator, known as __string concatenation operator__, that joins string together to a single one. <br>
  Example: def python_word(): 
    > text1 = "ython" <br>
    > text2 = "p" <br>
    >  result = `text1 + text2` <br>
    > return print(result) <br>

    > python_word() --> ythonp

The combined functions are used to create a defined function that moves the first character of the string to the end.  <br>

  >  `def rotate_word(text):` <br>
  > `return text[1:] + text [0]` <br>
  
  > `print(rotate_word("text"))` <br>
