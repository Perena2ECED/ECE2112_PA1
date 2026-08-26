# ECE2112 PA1
__Paulene Anne V. Pereña | 2ECE-D__  
This repository contains the Programming Assignment 1 for the course _Advanced Computer Programming_ (ECE2112).  
This project consists of three Python problems assigned to _Module 1 - Base Computing with Python._

# A. WORD ROTATION PROBLEM
The problem asked for a function that takes a string and returns a new string with the first character appended to the end, while the remaining characters retain their positions and capitalization.

The function name given was utilized to achieve the desired outputs following the requirements of the problem:
* `rotate_word(text)` --> a user-defined function that shifts the first character of a string to the very end of that string while keeping its capitalization.
  > __Example:__ `rotate_word("python")` --> "ythonp"

The following functions and operators were used to create the syntax that would follow the requirement given in the problem:
* `text[1: ]` --> a built-in syntax operator called __string slicing__, where it extracts a subset of a string starting from index 1, known as the second letter, until the end of the word.
  > __Example:__ text1 = "python" <br>    print(`text1[1: ]`) --> ython
  
* `text[0]` --> a built-in syntax operator called __string indexing__, which focuses on accessing the character located at index 0, the first character of the word.
  > __Example:__ text1 = "python" <br> print(`text1[0]`) --> p
  
* `+` -- > a built-in operator, known as __string concatenation operator__, that joins string together to a single string. <br>
  > __Example:__ def python_word(): <br>
  > text1 = "ython" <br>
  > text2 = "p" <br>
  > result = text1 `+` text2 <br>
  > print(result) <br>
  
  > python_word() --> ythonp

The combined functions are used to create a defined function that moves the first character of the string to the end.  
```
    def rotate_word(text):   
        return text[1:] + text[0]

    rotate_word("A") --> 'A'
```
# B. Username Builder Problem
The problem asks to create a function that accepts two strings, first and last name, with the following requirements: all letters are in lowercase, the first and last name are joined by a period, and spaces are removed.

The function name was used to achieve the desired output, so that it follows the requirements of the problem:
* `make_username(first_name, last_name)` --> a user-defined function that accepts two names as strings and format it following the requirements asked. 
    > __Example:__ `make_username("Ana Maria", "De Leon")` 

The following string methods were used to achieve the desired output for the problem:
* `.lower()` --> a built-in string method used to convert all letters in a string to lowercase.
    > __Example:__ text1 = "Ana Maria"  <br>
                  > `text1.lower()`

* `.replace(" ", "")` --> a built-in string method used to remove all spaces, replacing every space character with an empty string to remove gaps.
    > __Example:__ text1 = "Ana Maria"  <br>
    > `text1.replace(" ", "")`

* `+` -- > a built-in operator, known as __string concatenation operator__, that joins string together to a single string.
  > __Example:__ def make_username():  <br>
  > uname1 = "anamaria"  <br>
  > uname2 = "deleon"  <br>
  > result = uname1 `+` "." `+` uname2  <br>
  
  > print(result)

The following function and string methods were combined to achieve the desired syntax that will satisfy the requirements of the problem: 
```
  def make_username(first_name, last_name):
      first_name = first_name.lower().replace(" ","")
      last_name = last_name.lower().replace(" ", "")

      return first_name + "." + last_name

  make_username("Ana Maria", "De Leon") --> 'anamaria.deleon'
```

# C. Bookend Swap Problem
The problem asks to create a function that accepts a list with at least two elements and divides it into three variables: first, middle, and last. It asks that the first and last elements be exchanged while the middle remains in its original order.

The function name was used to achieve the desired output, so that it follows the requirements of the problem:
* `swap_bookends(items)` --> a user-defined function created to change the position of the first and last elements of the items.
  > __Example:__ `swap_bookends([1, 8])`--> [8, 1]

The following feature and operator were combined to form a syntax that holds the middle elements as one, and combines all elements while the first and last exchange positions:
* first, `*middle`, last --> a built-in Python feature used to combine into one the elements in between the first and last.
  > __Example:__ items = [1, `4,` 3] --> [4]

* `+` -- > a built-in operator, known as __list concatenation operator__, that joins string together to a single list.
  > __Example:__ def items():  <br>
  > first = 1  <br>
  > middle = [2]  <br>
  > last = 3  <br>
  > result = [last] `+` middle `+` [first]  <br>
  > return result  <br>
  
  > print(result) --> [1, 2, 3]

The following functions were combined to the desired syntax that will satisfy the requirements of the problem: 
```
  def swap_bookends(items):
      first, *middle, last = items

      return [last] + middle + [first]

swap_bookends(["red", "green", "blue"]) --> ['blue', 'green', 'red']
```

# Version History
* 2026, August 22 - README file was created, and the initial .ipynb file was uploaded.
* 2026, August 23 - README file initial contents were input.
* 2026, August 24 - The format and contents of the README file are still being finalized.
* 2026, August 27 - Final touches for the README file were committed.
