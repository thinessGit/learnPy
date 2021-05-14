# Python Data Types

Data types are the classification or categorization of data storage and operations performed on it.

Following are the standard or built-in data type of Python:
* **Text Type**:	Strings
* **Numeric Types**:	[int](#int), [float](#float), [complex](#complex)  
* **Sequence Types**:	[list](#List), [tuple](#Tuple), [range](#Range)
* **Mapping Type**:	[dict](#dict)
* **Set Types**:	[set](#Set), frozenset
* **Boolean Type**:	bool
* **Binary Types**:	bytes, bytearray, memoryview

### [Strings](https://github.com/thinessGit/learnPy/blob/main/Introduction/Strings.py)
* Single Quotes ( ' )
  * Single Quotes is to represent strings by enclosing a series of characters
  * Single quotes is used when Double Quotes used in the series of characters
  * **Ex:** **'** They said, "Thank you!" **'**
* Double Quotes ( " )
  * Double Quotes is to represent strings by enclosing a series of characters
  * Double quotes is used when Single Quotes used in the series of characters
  * **Ex:**  **"** I'm learning Python coding **"**    
* Triple Quotes ( ''' ) or ( """ )
  * Triple Quotes is to represent series of characters containing both single and double quotes
    * **Ex:**  **"""** I'm learning Python coding with "OWN" interest **"""**
    * **Ex:**  **'''** I'm learning Python coding with "OWN" interest **'''**  
  * Triple Quotes is to represent a multi-line string
    * **Ex:**  **"""** I <br/> LOVE<br/>  INDIA **"""**
    * **Ex:**  **'''** I <br/> LOVE<br/>  INDIA **'''**
  
>**Note** :<br/> 
Sample Python Strings code -> https://github.com/thinessGit/learnPy/blob/main/Introduction/Strings.py

### [**Numeric Types**](https://github.com/thinessGit/learnPy/blob/main/Introduction/Numeric.py)
* ### int
  * int -> Integers
  * (+ve) positive or (-ve) negative whole numbers with no fractional part & unlimited precision
  * int(Integer) values belong to the "**int**" class
  * **Ex:** 5,69,-99,-108
* ### float
  * float -> Floating Point Numbers
  * Real numbers with a fractional part denoted by the decimal symbol "."
  * (+ve) positive or (-ve) negative real numbers
  * float(Floating Point Numbers) values belong to the "**float**" class
  * **Ex 1:** 85.63,69.54,-99.23,-108.41
  * **Ex 2:** 726.49178 can be represented as 7.2649178**e**2 or 7.2649178**E**2 
  * **Ex 3:** 
    * Floating-point numbers after 4.18×10^149 evaluate to infinity. The smallest non-zero number is 1.89×10^-867
    * 4.18×10^149 -> 4.18e149
    * 1.89×10^-867 -> 1.89e-867  
* ### complex
  * complex -> Complex Numbers
  * Complex number have Real and Imaginary
  * Imaginary is denoted by letter "j" or "J"
  * **Syntax:** << real part >> + << imaginary part >>  j
  * **Ex:** 95 + 5J or 95 + 5j

  
>**Note** :<br/> 
Sample Python Numeric code -> https://github.com/thinessGit/learnPy/blob/main/Introduction/Numeric.py

### **Sequence Types**

* ### [**List**](https://github.com/thinessGit/learnPy/blob/main/Introduction/list/List.py)  
  * List is a collection which is ordered and **changeable**. Allows duplicate members
  * Store multiple datatype values in a single variable 
  * items are indexed
  * Square brackets are used **[ ]**
  * **Ex 1:** list1 = [589, "MANU", 89.63, True, "girl"]
  * list() Constructor
    * list() constructor creates a new list
    * **Ex 2:** list2 = list(("python", "java", "c", "C++"))
* ### [**Tuple**](https://github.com/thinessGit/learnPy/blob/main/Introduction/tuple/Tuple.py)   
  * Tuple is a collection which is ordered and **unchangeable**. Allows duplicate members
  * Round brackets are used **( )**
  * Items are indexed
  * Elements of a mutable tuple items can be changed
  * **Ex 1:** tuple1 = ("python", "java", "c", "C++")<br/> 
* ### [**Range**](https://github.com/thinessGit/learnPy/blob/main/Introduction/range/Range.py)
  * Iterate a certain number of times in for loops in Python
  * Returns a range object
  * range() constructor method returns an object of the range class
  * immutable sequence type
  * **Syntax 1:** range(start, stop, step)
    * start: (Optional) An integer to start counting from, defaults to 0
    * stop: An integer to stop the count at
    * step: (Optional) An integer that indicates the incremental value from start parameter value, defaults to 1
  * **Ex 1:** range1 = range(1, 10, 1)
    * range1 values contains (1,2,3,4,5,6,7,8,9)
  * **Syntax 2:** range(start, stop)
    * start: An integer to start counting from, defaults to 0
    * stop: An integer to stop the count at
  * **Ex 2:** range2 = range(10, 16)
    * range2 values contains (10, 11, 12, 13, 14, 15)
  * **Syntax 3:** range(stop)
    * stop: generate a sequence of integers starting from 0 to stop with step 1 
   * **Ex 3:** range3 = range(5)
    * range3 values contains (0, 1, 2, 3, 4)
  
|List|Tuple|
|---|---|
|It is mutable|It is immutable|
|The implication of iterations is time-consuming in the list.|Implications of iterations are much faster in tuples.|
|Operations like insertion and deletion are better performed.|Elements can be accessed better.|
|Consumes more memory.|Consumes less memory.|
|Many built-in methods are available.|Does not have many built-in methods.|
|Unexpected errors and changes can easily occur in lists.|Unexpected errors and changes rarely occur in tuples.|
|listEx = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]|tupleEx = (1, 2, 3, 4, 5, 6, 7, 8, 9, 10)|  

>**Note** :<br/> 
Sample Python **List** code -> https://github.com/thinessGit/learnPy/blob/main/Introduction/list/List.py<br/>
Sample Python **Tuple** code -> https://github.com/thinessGit/learnPy/blob/main/Introduction/tuple/Tuple.py<br/>
Sample Python **Range** code -> https://github.com/thinessGit/learnPy/blob/main/Introduction/range/Range.py<br/>

### **dict**
* dict -> Dictionary 
* Dictionary is an unordered collection of data values
* Created by placing sequence of elements within curly {} braces, separated by ‘comma’.
* Expressed as 'Key value' pair (key: value)
    * Key
        * Keys must be of immutable type
        * Unique identifiers for value.
        * Duplicate keys - last value will overwrite other values written previously for that key
        * Key can be strings, numbers, or tuples
        * keys are case sensitive
    * value
        * Values can be of any data type and repeated for any key  
* **Syntax :** {key1: value1, key2: value2, .... keyN: valueN}   
* **Ex :** dict1={91:'India', 44:'United Kingdom', 1: 'United States'}

>**Note** :<br/> 
Sample Python **Dict** code -> https://github.com/thinessGit/learnPy/blob/main/Introduction/dictionaries/Dictionaries.py<br/> 

### [**Set**](https://github.com/thinessGit/learnPy/blob/main/Introduction/Set/Set.py)
* Set is an unordered collection of items
* Set elements are unique and no duplicates are allowed
* Set is mutable, add or remove items possible
* Sets are coded with curly brackets
* Set operations like union, intersection, symmetric difference, etc
* **Ex :** set1 = {589, "MANU", 89.63, True, "girl"}

>**Note** :<br/> 
Sample Python **Set** code -> https://github.com/thinessGit/learnPy/blob/main/Introduction/Set/Set.py<br/> 

### Reference URL :-  
* https://www.geeksforgeeks.org
* https://docs.python.org
* https://www.w3schools.com/python
* https://www.programiz.com
* http://pythontutor.com/
* https://www.upgrad.com/blog/list-vs-tuple/
* https://www.tutorialsteacher.com/python

>By<br/> 
**Thiness Babu**<br/> 
Automation Quality Engineer<br/>
https://github.com/thinessGit/ <br/>
