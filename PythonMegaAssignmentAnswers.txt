## Assignment Part-1
Q1.) Why do we call Python as a general purpose and high-level programming language?
Ans:) Python is called as a general purpose and high-level programming language because it is an object-oriented language. 
It is based around objects (such as data) rather than functions, and high-level means it is easy for humans to understand.

Q2.) Why is Python called a dynamically typed language?
Ans:) Python is a dynamically typed language because we donot have to declare the type of a variable or manage the memory while assigning a value to a variable in Python. 
Other languages like C, C++, Java, etc., there is a strict declaration of variables before assigning values to them. 
We have to declare the kind of variable before assigning a value to it in the languages C, C++, Java, etc.
Python donot have any problem even if we donot declare the type of variable. 
It states the kind of variable in the runtime of the program. 
Python also take cares of the memory management which is crucial in programming. 
So, Python is a dynamically typed language. 

Example: 
Assignment-1.py:
# assigning a value to a variable
a = 10

# 'a' is an integer
print(type(a))

# reassigning a boolean value to the 'a'
a = True

# 'a' is a bool here
print(type(a))
# we can also redefine 'a' as many times as we want

Output:
[Running] python -u "/config/workspace/Assignment-1.py"
<class 'int'>
<class 'bool'>

[Done] exited with code=0 in 0.024 seconds

Q3.) List some pros and cons of Python programming language?
Ans:) Pros:
-> Python is easy to learn and read
-> Python enhances productivity
-> Python has a vast collection of libraries
-> Python is free, open-source, and has a vibrant community
-> Python is a portable programming language
-> Python is an interpreted language

Cons: 
-> Python has speed limitations
-> Python is not so strong with mobile computing
-> Python can have runtime errors
-> Python consumes a lot of memory space
-> Python is not easy to test
 
Q4.) In what all domains can we use Python?
Ans:) In the following seven domains, we can use Python:
-> Machine learning / Artificial intelligence
-> Desktop GUI
-> Data analytics and data visualization 
-> Web development
-> Game development
-> Mobile app development
-> Embedded systems

Q5.) What are variable and how can we declare them?
Ans:) A Variable is a name given to the specific memory location for storing the data value.
Python has no command for declaring a variable.
Thus, declaring a variable in Python is very simple.
Just name the variable.
Assign the required value to it.
The data type of the variable will be automatically determined from the value assigned, we need not define it explicitly.
Example:
x = 4       # x is of type int
x = "Sally" # x is now of type str
print(x)

Q6.) How can we take an input from the user in Python?
Ans:) We take an input from the user in Python by using input() function.
Example:
name = input('Enter the Username = ')
print(" The Username entered is - ", name)
Output:
Enter the Username = Sam
 The Username entered is -  Sam

Q7.) What is the default datatype of the value that has been taken as an input using input() function?
Ans:) It takes "String" datatype as default datatype.
Example:
Val = input('Enter the value = ')
print(" The value entered is - ", Val)
print(type(Val))
Output:
(a) Enter the value = 45
 The value entered is -  45
<class 'str'>

(b) Enter the value = GUI
 The value entered is -  GUI
<class 'str'>

Q8.) What is type casting?
Ans:) Type Casting is the method to convert the variable data type into a certain data type in order to the operation required to be performed by users. 
There can be two types of Type Casting in Python –
(i) Implicit Type Casting: In this,  methods, Python converts data type into another data type automatically. In this process, users donot have to involve in this process. 
Example:
# Python program to demonstrate
# implicit type Casting
 
# Python automatically converts
# a to int
a = 7
print(type(a))
 
# Python automatically converts
# b to float
b = 3.0
print(type(b))
 
# Python automatically converts
# c to float as it is a float addition
c = a + b
print(c)
print(type(c))
 
# Python automatically converts
# d to float as it is a float multiplication
d = a * b
print(d)
print(type(d))

Output:

<class 'int'>
<class 'float'>
10.0
<class 'float'>
21.0
<class 'float'>

(ii) Explicit Type Casting: In this method, Python need user involvement to convert the variable data type into certain data type in order to the operation required.
Mainly in type casting can be done with these data type function:
Int() : Int() function take float or string as an argument and return int type object.
float() : float() function take int or string as an argument and return float type object.
str() : str() function take float or int as an argument and return string type object.
Example:
Type Casting int to float:

Here, we are casting integer object to float object with float() function.

# Python program to demonstrate
# type Casting
 
# int variable
a = 5
 
# typecast to float
n = float(a)
 
print(n)
print(type(n))
Output:

5.0
<class 'float'>

Q9.) Can we take more than one input from the user using single input() function? If yes, how? If no, why?
Ans:) Yes, by using input().split() function.
Using split() method : 
This function helps in getting multiple inputs from users. It breaks the given input by the specified separator. If a separator is not provided then any white space is a separator. 
Generally, users use a split() method to split a Python string but one can use it in taking multiple inputs.
Syntax : 
input().split(separator, maxsplit)
Example : 
# Python program showing how to
# multiple input using split
# taking two inputs at a time
x, y = input("Enter two values: ").split()
print("Number of boys: ", x)
print("Number of girls: ", y)

Output:
Enter two values: 2 45
Number of boys:  2
Number of girls:  45
  
Q10.) What are keywords?
Ans:) Python keywords are special reserved words that have specific meanings and purposes. They cannot be used for anything but those specific purposes. 
These keywords are always available and we never have to import them into our code. There are 33 keywords.
>>> help("keywords")
Here is a list of the Python keywords.  Enter any keyword to get more help.

False               class               from                or
None                continue            global              pass
True                def                 if                  raise
and                 del                 import              return
as                  elif                in                  try
assert              else                is                  while
async               except              lambda              with
await               finally             nonlocal            yield
break               for                 not                 

Q11.) Can we use keywords as a variable? Support your answer with reason.
Ans:) No, they cannot be used for anything except for those specific purposes.
For Example:
False="amp"
print("Check for keywords=", False)
Output:
abc@72b93dbe7d47:~/workspace$ /bin/python /config/workspace/Assignment-1.py
  File "/config/workspace/Assignment-1.py", line 16
    False="amp"
    ^
SyntaxError: cannot assign to False

Q12.) What is indentation? What's the use of indentaion in Python?
Ans:) Indentation refers to the spaces at the beginning of a code line.
Where in other programming languages the indentation in code is for readability only, the indentation in Python is very important.
Python uses indentation to indicate a block of code.
Example
if 5 > 2:
  print("Five is greater than two!")
Output: 
Five is greater than two!

Python will give you an error if you skip the indentation:
Example
Syntax Error:
if 5 > 2:
print("Five is greater than two!")
 print("Five is greater than two!")
        ^
IndentationError: expected an indented block

Q13.) How can we throw some output in Python?
Ans:) The basic way to do output is the print statement. To end the printed line with a newline, add a print statement without any objects.
Example:
print('Hello World')
a=10
print("The value of a= ", a)
Output:
Hello World
The value of a=  10

Q14.) What are operators in Python?
Ans:) Operators are used to perform operations on variables and values. There are seven operators.
Python divides the operators in the following groups:
Arithmetic operators
Assignment operators
Comparison operators
Logical operators
Identity operators
Membership operators
Bitwise operators

Q15.) What is difference between / and // operators?
Ans:) / is used for float division.
// is used for integer division.
Example:
a=199
b=10
print("/ float division a/b=", a / b)
print("// integer division a//b=", a // b)
Output:
/ float division a/b= 19.9
// integer division a//b= 19

Q16.) Write a code that gives following as an output.

iNeuroniNeuroniNeuroniNeuron

Ans:) 
a= "iNeuron"
print(a * 4)

Q17.) Write a code to take a number as an input from the user and check if the number is odd or even.
Ans:)
a= int(input("Enter a number to check if it is Odd or Even = "))
if (a % 2 == 0):
    print ("Even number")
else:
    print ("Odd number")

Output:
Enter a number to check if it is Odd or Even = 94
Even number

Q18.) What are boolean operator?
Ans:) The logical operators and, or and not are also referred to as boolean operators. 
While and as well as or operator needs two operands, which may evaluate to true or false, not operator needs one operand evaluating to true or false.

Boolean and operator returns true if both operands return true.

>>> a=50
>>> b=25
>>> a>40 and b>40
False
>>> a>10 or b>100
True
>>> not(a==0)
True

Q19.) What will the output of the following?

1 or 0

0 and 0

True and False and True

1 or 0 or 0

Ans:) True, False, False, True

Q20.) What are conditional statements in Python?
Ans:) A conditional statement as the name suggests itself, is used to handle conditions in your program. 
These statements guide the program while making decisions based on the conditions encountered by the program.
Python has 3 key Conditional Statements that you should know:
(i) if statement
(ii) if-else statement
(iii) if-elif-else ladder

Q21.) What is use of 'if', 'elif' and 'else' keywords?
Ans:) The if/elif/else structure is a common way to control the flow of a program, allowing you to execute specific blocks of code depending on the value of some data.
if, elif, else are conditional statements that provide you with the decision making that is required when you want to execute code based on a particular condition.
The if, elif, else statement used in Python helps automate that decision making process.

Q22.) Write a code to take the age of person as an input and if age >= 18 display "I can vote". If age is < 18 display "I can't vote".
Ans:)
age= int(input("Enter age of person  = "))
if (age >= 18):
    print ("I can vote")
else:
    print ("I can't vote")

Output:
Enter age of person  = 22
I can vote

Q23.) Write a code that displays the sum of all the even numbers from the given list.

numbers = [12, 75, 150, 180, 145, 525, 50]

Ans:) 
numbers = [12, 75, 150, 180, 145, 525, 50]
sum=0
for i in numbers:
    if (i%2==0):
        sum=sum+i
print("Sum of Even numbers given in list = ", sum)

Output:
Sum of Even numbers given in list =  392

Q24.) Write a code to take 3 numbers as an input from the user and display the greatest no as output.
Ans:)
x = input("Enter first value: ")
y = input("Enter second value: ")
z = input("Enter third value: ")
if (x>y and x>z):
    print("Greatest number = ", x)
elif (y>z):
    print("Greatest number = ", y)
else:
    print("Greatest number = ", z)

Output:
Enter first value: 12
Enter second value: 13
Enter third value: 14
Greatest number =  14

Q25.) Write a program to display only those numbers from a list that satisfy the following conditions

The number must be divisible by five

If the number is greater than 150, then skip it and move to the next number

If the number is greater than 500, then stop the loop

numbers = [12, 75, 150, 180, 145, 525, 50]

Ans:) 
numbers = [12, 75, 150, 180, 145, 525, 50]
for i in numbers:
    if (i>500):
        break;
    if (i%5==0 and i<=150):
        print(i)

Output:
75
150
145
  

Q26.) What is a string? How can we declare string in Python?
Ans:) Strings are sequences of characters. Your name can be considered a string. Or, say you live in Zambia, then your country name is "Zambia", which is a string.
Declare string in Python:
--------------------------
To create a string, put the sequence of characters inside either single quotes, double quotes, or triple quotes and then assign it to a variable.

Example:
triple_quote_example = """this is a sentence written in triple quotes"""
double_quote_multiple_characters = "aeiou"
single_quote_multiple_characters = 'aeiou'
print(type(double_quote_multiple_characters), type(single_quote_multiple_characters), type(triple_quote_example))
<class 'str'> <class 'str'> <class 'str'>

Q27.) How can we access the string using its index?
Ans:) Often in programming languages, individual items in an ordered set of data can be accessed directly using a numeric index or key value. This process is referred to as indexing.

In Python, strings are ordered sequences of character data, and thus can be indexed in this way. Individual characters in a string can be accessed by specifying the string name followed by a number in square brackets ([]).

String indexing in Python is zero-based: the first character in the string has index 0, the next has index 1, and so on. The index of the last character will be the length of the string minus one.

Example:
Str="Apple"
print(Str[0])
print(Str[1])
print(Str[4])

Output:
A
p
e

Q28.) Write a code to get the desired output of the following
```
string = "Big Data iNeuron"
desired_output = "iNeuron"
```
Ans:)
string = "Big Data iNeuron"
#slicing
txt=string[9:]
print("desired_output=", txt)

Output:
desired_output= iNeuron

Q29.) Write a code to get the desired output of the following
```
string = "Big Data iNeuron"
desired_output = "norueNi"
```
Ans:)
string = "Big Data iNeuron"
#slicing
txt=string[:7:-1]
print("desired_output=", txt)

Output:
desired_output= norueNi 

Q30.) Resverse the string given in the above question.
Ans:)
string = "Big Data iNeuron"
#slicing
txt=string[::-1]
print("desired_output=", txt)

Output:
desired_output= norueNi ataD giB

Q31.) How can you delete entire string at once?
Ans:) By using replace() function we can delete entire string at once.

string = "Big Data iNeuron"
print("Given string=", string)
string=string.replace(string,"")
print("After deletion of entire string the output is = ", string)

Output:
Given string= Big Data iNeuron
After deletion of entire string the output is = 


Q32.) What is escape sequence?
Ans:) An escape sequence is a sequence of characters that, when used inside a character or string, does not represent itself but is converted into another character or series of characters that may be difficult or impossible to express directly, like newline (\n), tab (\t), and so on.

In simple terms, to insert characters that are illegal in a string, use an escape character.

An escape character is a backslash \ followed by the character you want to insert.

An example of an illegal character is a double quote inside a string that is surrounded by double quotes:
Example
You will get an error if you use double quotes inside a string that is surrounded by double quotes:
txt = "We are the so-called "Vikings" from the north."

To fix this problem, use the escape character \":
Example
The escape character allows you to use double quotes when you normally would not be allowed:

txt = "We are the so-called \"Vikings\" from the north."

Other escape characters used in Python:

Code	Result 	
\'	Single Quote	
\\	Backslash	
\n	New Line	
\r	Carriage Return	
\t	Tab	
\b	Backspace	
\f	Form Feed	
\ooo	Octal value	
\xhh	Hex value

Q33.) How can you print the below string?
```
'iNeuron's Big Data Course'
```
Ans:) 
string = "\'iNeuron's Big Data Course\'"
print(string)

Output:
'iNeuron's Big Data Course'

Q34.) What is a list in Python?
Ans:) Python Lists are just like dynamically sized arrays, declared in other languages (vector in C++ and ArrayList in Java). 
In simple language, a list is a collection of things, enclosed in [ ] and separated by commas. 
The list is a sequence data type which is used to store the collection of data.
Lists are the simplest containers that are an integral part of the Python language. 
Lists need not be homogeneous always which makes it the most powerful tool in Python. 
A single list may contain DataTypes like Integers, Strings, as well as Objects. Lists are mutable, and hence, 
they can be altered even after their creation.
Example:
Var = ["Apple", "for", "Rs1"]
print(Var)

Q35.) How can you create a list in Python?
Ans:) Lists in Python can be created by just placing the sequence inside the square brackets[]. 
Example:
# Creating a List
List = []
print("Blank List: ")
print(List)
 
# Creating a List of numbers
List = [10, 20, 14]
print("\nList of numbers: ")
print(List)
 
# Creating a List of strings and accessing
# using index
List = ["Apple", "For", "Rs1"]
print("\nList Items: ")
print(List[0])
print(List[2])

Output:
Blank List: 
[]

List of numbers:
[10, 20, 14]

List Items:
Apple
Rs1

Q36.) How can we access the elements in a list?
Ans:) In order to access the list items refer to the index number. 
Use the index operator [ ] to access an item in a list. The index must be an integer. 
Nested lists are accessed using nested indexing.
Example:
# accessing of element from list
# the use of multiple values
List = ["Apple", "For", "Rs1"]
 
# accessing a element from the
# list using index number
print("Accessing a element from the list")
print(List[0])
print(List[2])

# Creating a Multi-Dimensional List
# (By Nesting a list inside a List)
List = [['Apple', 'For'], ['Rs1']]
 
# accessing an element from the
# Multi-Dimensional List using
# index number
print("Accessing a element from a Multi-Dimensional list")
print(List[0][1])
print(List[1][0])

Output:
Accessing a element from the list
Apple
Rs1
Accessing a element from a Multi-Dimensional list
For
Rs1

Q37.) Write a code to access the word "iNeuron" from the given list.
```
lst =   [1,2,3,"Hi",[45,54, "iNeuron"], "Big Data"]
``` 
Ans:)
lst = [1,2,3,"Hi",[45,54, "iNeuron"], "Big Data"]
print("Print \"iNeuron\" from a Multi-Dimensional list")
print(lst[4][2])

Output:
Print "iNeuron" from a Multi-Dimensional list
iNeuron

Q38.) Take a list as an input from the user and find the length of the list.
Ans:)
list  = input("Enter any kind of input items in the list separated by space = ").split()
print("Printing all items in the list",list)
print("The length of the list=", len(list))

Output:
Enter any kind of input items in the list separated by space = 1 2 mm
Printing all items in the list ['1', '2', 'mm']
The length of the list= 3

Q39.) Add the word "Big" in the 3rd index of the given list.
```
lst = ["Welcome", "to", "Data", "course"]
```
Ans:)
lst = ["Welcome", "to", "Data", "course"]
lst.insert(3,"Big")
print(lst)

Output:
['Welcome', 'to', 'Data', 'Big', 'course']

Q40.) What is a tuple? How is it different from list?
Ans:) Tuples are used to store multiple items in a single variable.

Tuple is one of 4 built-in data types in Python used to store collections of data, the other 3 are List, Set, and Dictionary, all with different qualities and usage.
A tuple is a collection which is ordered and unchangeable.
Tuples are written with round brackets.

List and Tuple in Python are the classes of Python Data Structures. The list is dynamic, whereas the tuple has static characteristics. This means that lists can be modified whereas tuples cannot be modified, the tuple is faster than the list because of static in nature. Lists are denoted by the square brackets but tuples are denoted as parenthesis.

Important differences between List and Tuple in Python
	LIST	                                            TUPLE
1	Lists are mutable	                                Tuples are immutable.
2	The implication of iterations is Time-consuming	    The implication of iterations is comparatively Faster.
3	The list is better for performing operations,       In tuple, it is hard to take place.
    such as insertion and deletion.	
4	Lists consume more memory	                        Tuple consumes less memory as compared to the list.
5	Lists have several built-in methods	                Tuple does not have many built-in methods.
6	The unexpected changes and errors are more likely   In tuple, it is hard to take place.
    to occur	

Q41.) How can you create a tuple in Python?
Ans:) A tuple is a collection which is ordered and unchangeable.
Tuples are written with round brackets.
Example:
thistuple = ("apple", "banana", "cherry")
print(thistuple)

Output:
("apple", "banana", "cherry")

Q42.) Create a tuple and try to add your name in the tuple. Are you able to do it? Support your answer with reason.
Ans:) Tuple items are ordered, unchangeable, and allow duplicate values.
Tuple items are indexed, the first item has index [0], the second item has index [1] etc.
When we say that tuples are ordered, it means that the items have a defined order, and that order will not change.
Tuples are unchangeable, meaning that we cannot change, add or remove items after the tuple has been created.
Since tuples are indexed, they can have items with the same value.

tuple=(1,"app","de")
print("Given tuple=", tuple)
tuple[3]="Lalli"

Output:
Cell In [2], line 3
      1 tuple=(1,"app","de")
      2 print("Given tuple=", tuple)
----> 3 tuple[3]="Lalli"

TypeError: 'tuple' object does not support item assignment

Q43.) Can two tuple be appended. If yes, write a code for it. If not, why?
Ans:) Yes, two tuples can be appended.
Code:
t1=("me", "amL", "mm")
t2=(1, 2, 3)
print("Tuple1=",t1,"Tuple2=",t2)
print("appended two tuples=", t1+t2)

Output:
Tuple1= ('me', 'amL', 'mm') Tuple2= (1, 2, 3)
appended two tuples= ('me', 'amL', 'mm', 1, 2, 3)

Q44.) Take a tuple as an input and print the count of elements in it.
Ans:)
tuple=(1,"app","de")
print("Length/Count of entered tuple=", len(tuple))

Output:
Length/Count of entered tuple= 3

Q45.) What are sets in Python?
Ans:) Sets are used to store multiple items in a single variable.
Set is one of 4 built-in data types in Python used to store collections of data, the other 3 are List, Tuple, and Dictionary, all with different qualities and usage.
A set is a collection which is unordered, unchangeable*, and unindexed.
* Note: Set items are unchangeable, but you can remove items and add new items.
Sets are written with curly brackets.
Note: Sets are unordered, so you cannot be sure in which order the items will appear.
Sets cannot have two items with the same value.

Q46.) How can you create a set?
Ans:) 
thisset = {"apple", "banana", "cherry"}
print(thisset)

Output:
{'apple', 'cherry', 'banana'}

Q47.) Create a set and add "iNeuron" in your set.
Ans:) The Python set add() method adds a given element to a set if the element is not present in the set in Python. 
Syntax: set.add( elem )

set_a={"iNeuron"}
print("The Set=",set_a)
#(or)

set_a=set()
set_a.add("iNeuron")
print("The Set=",set_a)

Output:
The Set= {'iNeuron'}

Q48.) Try to add multiple values using add() function.
Ans:)
s = {'g', 'e', 'e', 'k', 's'}
t = ('f', 'o')
print("Initial set=",s)
# adding tuple t to set s.
s.add(t)
print("After add() of tuple to set=",s) 
 
Output:
Initial set= {'g', 's', 'k', 'e'}
After add() of tuple to set= {'s', 'e', 'k', ('f', 'o'), 'g'}

Q49.) How is update() different from add()?
Ans:) In python, set class provides two different functions to add or append elements in the set. 
The basic overview about them,
set.add() Function:
set.add(element)
It accepts an element as an argument and if that element is not already present in the set, then it adds that to the set. It returns nothing i.e. None.
set.update() Function:
set.update(*args)
It expects a single or multiple iterable sequences as arguments and appends all the elements in these iterable sequences to the set. It returns nothing i.e. None.

Differences between add() and update()
(a) Use add() function to add a single element. Whereas use update() function to add multiple elements to the set.
(b) add() is faster than update().
(c) add () accepts immutable parameters only. Whereas accepts iterable sequences.
(d) add() accepts a single parameter, whereas update() can accept multiple sequences.

So, these were the 4 main differences between update() and add() functions of set in python.

The complete example is as follows,
def main():
    sample_set = {"Hi", "This", "is", 4, 3, 3}
    print('Original Set:')
    print(sample_set)
    print(' **** Differences between add() & update() functions of set ****')
    print('*** Difference 1: Number of elements to be added ***')
    print('Add an element in set using add() function')
    # Add only a single element in set
    sample_set.add(10)
    print('Modified Set:')
    print(sample_set)
    print('Add multiple element in set using update() function')
    sample_set = {"Hi", "This", "is", 4, 3, 3}
    # Adding multiple elements to the set
    sample_set.update([11, 12, 13, 14])
    print('Modified Set:')
    print(sample_set)
    print('*** Difference 3: Mutable and immutable parameters *** ')
    sample_set = {"Hi", "This", "is", 4, 3, 3}
    print('Passing a mutable object to add() will give error')
    # Passing a mutable list object to the add() function
    # It will give error => TypeError: unhashable type: 'list'
    # sample_set.add([11, 12, 13, 14])
    print('Passing a mutable object like list to update() function')
    # Passing a list to update() will add all elements in list to the set
    sample_set.update([11, 12, 13, 14])
    print('Modified Set:')
    print(sample_set)
    print('Passing anything other than iterable sequence to the update() function will give error')
    # As 55 is not iterable sequence, so it will give error
    # Error => TypeError: 'int' object is not iterable
    #sample_set.update(55)
    print('*** Difference 4: Passing multiple arguments ***')
    sample_set = {"Hi", "This", "is", 4, 3, 3}
    # passing multiple sequences to the update() function
    sample_set.update([11, 12], (21, 22), [31, 32])
    print('Set contents: ')
    print(sample_set)
if __name__ == '__main__':
   main()

Output:
Original Set:
{3, 4, 'is', 'This', 'Hi'}
 **** Differences between add() & update() functions of set ****
*** Difference 1: Number of elements to be added ***
Add an element in set using add() function
Modified Set:
{3, 4, 10, 'is', 'This', 'Hi'}
Add multiple element in set using update() function
Modified Set:
{3, 4, 11, 12, 13, 14, 'is', 'This', 'Hi'}
*** Difference 3: Mutable and immutable parameters *** 
Passing a mutable object to add() will give error
Passing a mutable object like list to update() function
Modified Set:
{3, 4, 11, 12, 13, 14, 'is', 'This', 'Hi'}
Passing anything other than iterable sequence to the update() function will give error
*** Difference 4: Passing multiple arguments ***
Set contents: 
{32, 3, 4, 11, 12, 'is', 21, 22, 'This', 31, 'Hi'}

Q50.) What is clear() in sets?
Ans:) The clear() method removes all elements in a set.

fruits = {"apple", "banana", "cherry"}
fruits.clear()
print(fruits)

Output:
set()

Q51.) What is frozen set?
Ans:) The frozenset() function returns an immutable frozenset object initialized with elements from the given iterable.
Frozen set is just an immutable version of a Python set object. 
While elements of a set can be modified at any time, elements of the frozen set remain the same after creation.
Due to this, frozen sets can be used as keys in Dictionary or as elements of another set. But like sets, it is not ordered (the elements can be set at any index).
The syntax of frozenset() function is:
frozenset([iterable])
frozenset() Parameters
The frozenset() function takes a single parameter:
iterable (Optional) - the iterable which contains elements to initialize the frozenset with.
Iterable can be set, dictionary, tuple, etc.
Return value from frozenset()
The frozenset() function returns an immutable frozenset initialized with elements from the given iterable.
If no parameters are passed, it returns an empty frozenset.

Example 1: Working of Python frozenset()
# tuple of vowels
vowels = ('a', 'e', 'i', 'o', 'u')

fSet = frozenset(vowels)
print('The frozen set is:', fSet)
print('The empty frozen set is:', frozenset())

# frozensets are immutable
fSet.add('v')

Output:

The frozen set is: frozenset({'a', 'o', 'u', 'i', 'e'})
The empty frozen set is: frozenset()
Traceback (most recent call last):
  File "<string>, line 8, in <module>
    fSet.add('v')
AttributeError: 'frozenset' object has no attribute 'add'

Example 2: frozenset() for Dictionary

When you use a dictionary as an iterable for a frozen set, it only takes keys of the dictionary to create the set.

# random dictionary
person = {"name": "John", "age": 23, "sex": "male"}

fSet = frozenset(person)
print('The frozen set is:', fSet)

Output:

The frozen set is: frozenset({'name', 'sex', 'age'})

Frozenset operations
Like normal sets, frozenset can also perform different operations like copy, difference, intersection, symmetric_difference, and union.

# Frozensets
# initialize A and B
A = frozenset([1, 2, 3, 4])
B = frozenset([3, 4, 5, 6])

# copying a frozenset
C = A.copy()  # Output: frozenset({1, 2, 3, 4})
print(C)

# union
print(A.union(B))  # Output: frozenset({1, 2, 3, 4, 5, 6})

# intersection
print(A.intersection(B))  # Output: frozenset({3, 4})

# difference
print(A.difference(B))  # Output: frozenset({1, 2})

# symmetric_difference
print(A.symmetric_difference(B))  # Output: frozenset({1, 2, 5, 6})

Output:

frozenset({1, 2, 3, 4})
frozenset({1, 2, 3, 4, 5, 6})
frozenset({3, 4})
frozenset({1, 2})
frozenset({1, 2, 5, 6})
Similarly, other set methods like isdisjoint, issubset, and issuperset are also available.

# Frozensets
# initialize A, B and C
A = frozenset([1, 2, 3, 4])
B = frozenset([3, 4, 5, 6])
C = frozenset([5, 6])

# isdisjoint() method
print(A.isdisjoint(C))  # Output: True

# issubset() method
print(C.issubset(B))  # Output: True

# issuperset() method
print(B.issuperset(C))  # Output: True

Output:

True
True
True

Q52.) How is frozen set different from set?
Ans:) Frozen set is just an immutable version of a Python set object. 
While elements of a set can be modified at any time, elements of the frozen set remain the same after creation.
Due to this, frozen sets can be used as keys in Dictionary or as elements of another set. 
But like sets, it is not ordered (the elements can be set at any index).

Q53.) What is union() in sets? Explain via code.
Ans:) The union of two sets A and B is the set of elements which are in A, in B, or in both A and B. 
For example, if A = {1, 3, 5, 7} and B = {1, 2, 4, 6, 7} then A ∪ B = {1, 2, 3, 4, 5, 6, 7}.
Python Set union() Method:
The union() method returns a set that contains all items from the original set, and all items from the specified set(s).
Code:
x = {"apple", "banana", "cherry", 1}
y = {"google", "microsoft", "apple", 4, 9}
z = x.union(y)
print("x union y =", z)
Output:
x union y = {1, 'microsoft', 'apple', 4, 'banana', 9, 'cherry', 'google'}

Q54.) What is intersection() in sets? Explain via code.
Ans:) The intersection of sets can be denoted using the symbol '∩'. As defined above, the intersection of two sets A and B is the set of all those elements which are common to both A and B. Symbolically, we can represent the intersection of A and B as A ∩ B.
Python Set intersection() Method:
The intersection() method returns a set that contains the similarity between two or more sets. Meaning: The returned set contains only items that exist in both sets, or in all sets if the comparison is done with more than two sets.
Code:
x = {"apple", "banana", "cherry", 1}
y = {"google", "microsoft", "apple", 4, 9}
z = x.intersection(y)
print("x intersection y =", z)
Output:
x intersection y = {'apple'}

Q55.) What is dictionary ibn Python?
Ans:) Dictionaries are used to store data values in key:value pairs.
A dictionary is a collection which is ordered*, changeable and do not allow duplicates.
Note: As of Python version 3.7, dictionaries are ordered. In Python 3.6 and earlier, dictionaries are unordered.

Q56.) How is dictionary different from all other data structures.
Ans:) Dictionary in Python is a collection of keys values, used to store data values like a map, which, unlike other data types which hold only a single value as an element.
Dictionary holds key:value pair. Key-Value is provided in the dictionary to make it more optimized. 
Dict = {1: 'Green', 2: 'Frock', 3: 'Girls'}
print(Dict)
Output:
{1: 'Green', 2: 'Frock', 3: 'Girls'}

Q57.) How can we delare a dictionary in Python?
Ans:) Dictionaries are written with curly brackets, and have keys and values.
Example
Create and print a dictionary:

thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
print(thisdict)

Output:
{'brand': 'Ford', 'model': 'Mustang', 'year': 1964}

Q58.) What will the output of the following?
```
var = {}
print(type(var))
```
Ans:) Output: <class 'dict'>

Q59.) How can we add an element in a dictionary?
Ans:) The syntax for adding a new value to a dictionary:
dictionary_name[key] = value

Example:
dict={}
dict[1]="Name"
print(dict)

Output:
{1: 'Name'}

Q60.) Create a dictionary and access all the values in that dictionary.
Ans:)
dict={0:"Welcome"}
dict[1]="Name"
dict[2]="age"
print(dict)
print("Value at key=2 is =",dict[2])

Output:
{0: 'Welcome', 1: 'Name', 2: 'age'}
Value at key=2 is = age

Q61.) Create a nested dictionary and access all the element in the inner dictionary.
Ans:)
dict1={0: 'Welcome', 1: 'Name', 2: 'age'}
dict2={11:"Game", 22:"People", 33:"Play", 44: dict1, 55:"Trickster"}
print(dict2)
print("inner dictionary some values = \n", dict2[44][0],",", dict2[44][2])

Output:
{11: 'Game', 22: 'People', 33: 'Play', 44: {0: 'Welcome', 1: 'Name', 2: 'age'}, 55: 'Trickster'}
inner dictionary some values = 
 Welcome , age

Q62.) What is the use of get() function?
Ans:) The get() method returns the value of the item with the specified key.
Syntax:
dictionary.get(keyname, value)
The keyname of the item you want to return the value from.
A value to return if the specified key does not exist. Default value None.
Example:
car = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}

x = car.get("model")
y= car.get("color", "Red")

print(x)
print(y)

Output:
Mustang
Red

Q63.) What is the use of items() function?
Ans:) The items() method returns a view object. The view object contains the key-value pairs of the dictionary, as tuples in a list.
The view object will reflect any changes done to the dictionary. 
Syntax:
dictionary.items()
Example:
car = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
x = car.items()
print(x)

Output:
dict_items([('brand', 'Ford'), ('model', 'Mustang'), ('year', 1964)]

Q64.) What is the use of pop() function?
Ans:) The pop() method removes the element at the specified position.
Syntax:
list.pop(pos)
pos	Optional. A number specifying the position of the element you want to remove, default value is -1, which returns the last item.

Example:
#Remove the second element of the fruit list:
fruits = ['apple', 'banana', 'cherry']
x= fruits.pop(1)
print(x)
print(fruits)

Output:
banana
['apple', 'cherry']

Q65.) What is the use of popitems() function?
Ans:) The popitem() method removes the item that was last inserted into the dictionary. In versions before 3.7, the popitem() method removes a random item.
The removed item is the return value of the popitem() method, as a tuple, see example below.
Syntax:
dictionary.popitem()

Example:
car = {
  "brand": "Tata",
  "model": "Nexus",
  "year": 2022,
  "color": "Red",
  "Type": "EV"
}
x = car.popitem()
print("Popitem() on car= ", x)
print("car dictionary after popitems= ", car)

Output:
Popitem() on car=  ('Type', 'EV')
car dictionary after popitems=  {'brand': 'Tata', 'model': 'Nexus', 'year': 2022, 'color': 'Red'}

Q66.) What is the use of keys() function?
Ans:) The keys() method returns a view object. The view object contains the keys of the dictionary, as a list.
The view object will reflect any changes done to the dictionary, see example below.
Syntax:
dictionary.keys()

Example:
car = {
  "brand": "Tata",
  "model": "Nexus",
  "year": 2022,
  "color": "Red",
  "Type": "EV"
}
x = car.keys()
print("Keys of car = ", x)

Output:
Keys of car =  dict_keys(['brand', 'model', 'year', 'color', 'Type'])

Q67.) What is the use of values() function?
Ans:) The values() method returns a view object. The view object contains the values of the dictionary, as a list.
The view object will reflect any changes done to the dictionary, see example below.
Syntax:
dictionary.values()

Example:
car = {
  "brand": "Tata",
  "model": "Nexus",
  "year": 2022,
  "color": "Red",
  "Type": "EV"
}
x = car.values()
print("values of car = ", x)

Output:
values of car =  dict_values(['Tata', 'Nexus', 2022, 'Red', 'EV'])

Q68.) What are loops in Python?
Ans:) In general, statements are executed sequentially: The first statement in a function is executed first, followed by the second, and so on. 
There may be a situation when you need to execute a block of code several number of times.
Programming languages provide various control structures that allow for more complicated execution paths.
A loop statement allows us to execute a statement or group of statements multiple times. 

Q69.) How many type of loop are there in Python?
Ans:) Python programming language provides following types of loops to handle looping requirements.
1)	while loop: Repeats a statement or group of statements while a given condition is TRUE. It tests the condition before executing the loop body.
2)	for loop: Executes a sequence of statements multiple times and abbreviates the code that manages the loop variable.
3)	nested loops: We can use one or more loop inside any another while, for or do..while loop.

Q70.) What is the difference between for and while loops?
Ans:) 
Basis of Comparison	                    For Loop	                                      While Loop
Keyword	                                Uses for keyword	                              Uses while keyword
Used	                                For loop is used when the number of               While loop is used when the number of
                                        iterations is already known.	                  iterations is already Unknown.
absence of condition	                The loop runs infinite times in the               Returns the compile time error in the absence of condition
                                        absence of condition
Nature of Initialization                Once done, it cannot be repeated                  In the while loop, it can be repeated at every iteration
Functions                               To iterate, the range or xrange function          There is no such function in the while loop.
                                        is used.
Initialization based on iteration       To be done at the beginning of the loop.          In the while loop, it is possible to do this anywhere in the loop body.
Generator Support                       Python's for loop can iterate over generators.    While loops cannot be directly iterated on Generators.
Speed                                   The for loop is faster than the while loop.       While loop is relatively slower as compared to for loop.

Q71.) What is the use of continue statement?
Ans:) The continue keyword is used to end the current iteration in a for loop (or a while loop), and continues to the next iteration.

Example:
#Skip the iteration if the variable i is 3, but continue with the next iteration:
for i in range(4):
  if i == 3:
    continue
  print(i)

Output:
0
1
2
4

Q72.) What is the use of break statement?
Ans:) 'Break’ in Python is a loop control statement. It is used to control the sequence of the loop. 
Suppose you want to terminate a loop and skip to the next code after the loop; break will help you do that. 
A typical scenario of using the Break in Python is when an external condition triggers the loop’s termination. 
Another use case for using ‘Break’ in Python is when you’ve taken an input for something, printed it using a loop, 
and want to give the user an option to print it again. If the user inputs “No,” you can terminate the loop. 

You can use break in Python in all the loops: while, for, and nested. If you are using it in nested loops, 
it will terminate the innermost loop where you have used it, and the control of the program will flow to the outer loop. 
In other words, it breaks the sequence of the loop, and the control goes to the first statement outside the loop.
It is used after the loop statements.

Syntax of Break in Python:
break;

Example:
number = 0
for number in range(10):
    if number == 5:
        break    # break here

    print('Number is ' + str(number))
print('Out of loop')

Output:
Number is 0
Number is 1
Number is 2
Number is 3
Number is 4
Out of loop

Q73.) What is the use of pass statement?
Ans:) The pass statement is used as a placeholder for future code.
When the pass statement is executed, nothing happens, but you avoid getting an error when empty code is not allowed.
Empty code is not allowed in loops, function definitions, class definitions, or in if statements.

Example:
def myfunction():
  pass

# having an empty function definition like this, would raise an error without the pass statement

Q74.) What is the use of range() function?
Ans:) The range() function returns a sequence of numbers, starting from 0 by default, and increments by 1 (by default), and stops before a specified number.
Syntax:
range(start, stop, step)
start	Optional. An integer number specifying at which position to start. Default is 0
stop	Required. An integer number specifying at which position to stop (not included).
step	Optional. An integer number specifying the incrementation. Default is 1

Example:
x = range(3, 6)
for n in x:
  print(n)

Output:
3
4
5

Q75.) How can you loop over a dictionary?
Ans:) We can loop through a dictionary by using a for loop.
When looping through a dictionary, the return value are the keys of the dictionary, but there are methods to return the values as well.

Example:
mydict={1:'a', 2:'b', 3:'c', 4:'d'}
for i in mydict:
    print("-------------------")
    print("keys:", i)
    print("values:", mydict[i])

Output:
-------------------
keys: 1
values: a
-------------------
keys: 2
values: b
-------------------
keys: 3
values: c
-------------------
keys: 4
values: d

### Coding problems
Q76.) Write a Python program to find the factorial of a given number.
Ans:) #code:
num=int(input("Enter the number to find its factorial="))
if num==1 or num==0:
    print("Factorial of given number", num, "= 1")
elif num < 0:
    print("Entered number is Invalid !!!")
else:
    fact=1
    for i in range(1, num+1):
        fact=fact*i
    print("Factorial of given number", num, "=", fact)

Output:
Factorial of given number 7 = 5040

Q77.) Write a Python program to calculate the simple interest. Formula to calculate simple interest is SI = (P*R*T)/100
Ans:) #code:
P=int(input("Enter the Principal in Rupees="))
T=int(input("Enter the time in years="))
R=int(input("Enter the Rate of interest per annum in percentage="))
if P < 0 or T < 0 or R < 0:
    print("Entered number/s is/are Invalid !!!")
else:
    SI=(P*T*R)/100
    print("Simple interest is  = ", SI)

Output:
Enter the Principal in Rupees=100000
Enter the time in years=5
Enter the Rate of interest per annum in percentage=10
Simple interest is  =  50000.0

Q78.) Write a Python program to calculate the compound interest. Formula of compound interest is A = P(1+ R/100)^t.
Ans:) #code:
P=int(input("Enter the Principal in Rupees="))
t=int(input("Enter the time in years="))
R=int(input("Enter the Rate of interest per annum in percentage="))
if P < 0 or t < 0 or R < 0:
    print("Entered number/s is/are Invalid !!!")
else:
    #A = P(1+ R/100)^t
    CI = P*((1+ (R/100))**t)-P
    print("Compound interest is  = Rs ", CI)

Output:
Enter the Principal in Rupees=100000
Enter the time in years=5
Enter the Rate of interest per annum in percentage=10
Compound interest is  = Rs  61051.00000000006

Q79.) Write a Python program to check if a number is prime or not.
Ans:) #code:
num=int(input("Enter the number to check if prime or not ="))
if num < 0:
    print("Entered number is invalid !!!")
elif num == 1 or num == 0:
    print("The entered number ",num," is not PRIME NUMBER")
else:
    for i in range(2,num+1):
        if i == num:
            if num%i == 0:
              print("The entered number ",num," is PRIME NUMBER")
            else:
              print("The entered number ",num," is not PRIME NUMBER")

Output:
Enter the number to check if prime or not = 1111
The entered number  1111  is PRIME NUMBER

Q80.) Write a Python program to check Armstrong Number.
Ans:) #code:
num=int(input("Enter the number= "))
#in a given number base b is a number that is the sum of its own digits each raised to the power of the number of digits
s=num
l=len(str(num))
sum=0
while num!=0:
    rem=num%10
    sum=sum+rem**l
    num=num//10
if s==sum:
    print("Given number ", s," is ARMSTRONG NUMBER")
else:
    print("Given number ", s," is not ARMSTRONG NUMBER")

Output:
Enter the number= 12345
Given number  12345  is not ARMSTRONG NUMBER

Q81.) Write a Python program to find the n-th Fibonacci Number.
Ans:) #code:
def solve(n):
   if n <= 2:
      return n - 1
   else:
      return solve(n - 1) + solve(n - 2)

n = int(input("Enter the n fibbonacci number= "))
print(solve(n))

Output:
Enter the n fibbonacci number= 11
55

Q82.) Write a Python program to interchange the first and last element in a list.
Ans:) #By Using * operand: This operand proposes a change to iterable unpacking syntax, allowing to specify a “catch-all” name which will be assigned a list of all #items not assigned to a “regular” name. 
# Python3 program to swap first
# and last element of a list
 
# Swap function
def swapList(list):
     
    start, *middle, end = list
    list = [end, *middle, start]
     
    return list
# Driver code
newList = [12, 35, 9, 56, 24, 45, 65]
print(swapList(newList))

Output:
[65, 35, 9, 56, 24, 45, 12]

Q83.) Write a Python program to swap two elements in a list.
Ans:) #code:
# Python3 program to swap elements
# at given positions
 # Swap function
def swapPositions(list, pos1, pos2):
    list[pos1], list[pos2] = list[pos2], list[pos1]
    return list

# Driver function
List = [23, 65, 19, 90, 100, 200]
pos1, pos2  = 1, 4
print(swapPositions(List, pos1-1, pos2-1))

Output:
[90, 65, 19, 23, 100, 200]

Q84.) Write a Python program to find N largest element from a list.
Ans:) #code:
# Python program to find N largest
# element from given list of integers
l = [100,298,3579,100,200,-45,900]
n = 2
l.sort()
print(l[-n:])

Output:
[900, 3579]

Q85.) Write a Python program to find cumulative sum of a list.
Ans:) #code:
list=[10,20,30,40,50]
new_list=[]
j=0
for i in range(0,len(list)):
    j+=list[i]
    new_list.append(j)
print(new_list)

Output:
[10, 30, 60, 100, 150]

Q86.) Write a Python program to check if a string is palindrome or not.
Ans:) #code:
# function which return reverse of a string
def isPalindrome(s):
    return s == s[::-1]
# Driver code
s = str(input("Enter the input string= "))
ans = isPalindrome(s)
 
if ans:
    print("Yes")
else:
    print("No")

Output:
Enter the input string= amma
Yes

Q87.) Write a Python program to remove i'th element from a string.
Ans:) #code:
# Python3 program for removing i-th 
# indexed character from a string
  
# Removes character at index i
def remove(string, i): 
  
    for j in range(len(string)):
        if j == i:
            string = string.replace(string[i], "", 1)
    return string
      
# Driver Code
string = "geeksFORgeeks"
# Remove nth index element
i = 7
# Print the new string
print(remove(string, i))

Output:
geeksFOgeeks

Q88.) Write a Python program to check if a substring is present in a given string.
Ans:) #code:
# Take input from users
MyString1 = "A friend in need is a friend indeed"
 
if "a" in MyString1:
    print("Yes! it is present in the string")
else:
    print("No! it is not present")

Output:
Yes! it is present in the string

Q89.) Write a Python program to find words which are greater than given length k.
Ans:) #code:
sentence = "hello my dear friends"
length = 4
#print([word for word in sentence.split() if len(word) > length])
for word in sentence.split():
    if len(word) > length:
        print(word)

Output:
hello
friends

Q90.) Write a Python program to extract unquire dictionary values.
Ans:) #code:
# Extract Unique values dictionary values
# initializing dictionary
test_dict = {'gfg' : [5, 6, 7, 8],
            'is' : [10, 11, 7, 5],
            'best' : [6, 12, 10, 8],
            'for' : [1, 2, 5]}
 
# printing original dictionary
print("The original dictionary is : ", test_dict)
 
# Extract Unique values dictionary values
x=[]
for i in test_dict.keys():
    x.extend(test_dict[i])
x=list(set(x))
x.sort()
# printing result
print("The unique values list is : " + str(x))

Output:
The original dictionary is :  {'gfg': [5, 6, 7, 8], 'is': [10, 11, 7, 5], 'best': [6, 12, 10, 8], 'for': [1, 2, 5]}
The unique values list is : [1, 2, 5, 6, 7, 8, 10, 11, 12]

Q91.) Write a Python program to merge two dictionary.
Ans:)  #Code
dict1={0: 'Welcome', 1: 'Name', 2: 'age'}
dict2={11:"Game", 22:"People", 33:"Play", 55:"Trickster"}
print("Merged dictionary = := = ")
#By unpack operator **
dict3={**dict1, **dict2}
print("By ** operator = ", dict3)
#By merge(|)operator
dict4=dict1|dict2
print("By Merge(|) operator = ", dict4)
#By Update()
dict1.update(dict2)
print("By update function= \n", dict1)

Output:
Merged dictionary = := = 
By ** operator =  {0: 'Welcome', 1: 'Name', 2: 'age', 11: 'Game', 22: 'People', 33: 'Play', 55: 'Trickster'}
By Merge(|) operator =  {0: 'Welcome', 1: 'Name', 2: 'age', 11: 'Game', 22: 'People', 33: 'Play', 55: 'Trickster'}
By update function= 
 {0: 'Welcome', 1: 'Name', 2: 'age', 11: 'Game', 22: 'People', 33: 'Play', 55: 'Trickster'}

Q92.) Write a Python program to convert a list of tuples into dictionary.
```
Input : [('Sachin', 10), ('MSD', 7), ('Kohli', 18), ('Rohit', 45)]
Output : {'Sachin': 10, 'MSD': 7, 'Kohli': 18, 'Rohit': 45}
```
Ans:)%code


Q93.) Write a Python program to create a list of tuples from given list having number and its cube in each tuple.
```
Input: list = [9, 5, 6]
Output: [(9, 729), (5, 125), (6, 216)]
```
Ans:) #code:
list = [9, 5, 6]
list_a=[]
for v in list:
    cube=v*v*v
    list_a.append((v,cube))
print(list_a)

Output:
[(9, 729), (5, 125), (6, 216)]

Q94.) Write a Python program to get all combinations of 2 tuples.
```
Input : test_tuple1 = (7, 2), test_tuple2 = (7, 8)
Output : [(7, 7), (7, 8), (2, 7), (2, 8), (7, 7), (7, 2), (8, 7), (8, 2)]
```
Ans:)#code
test_tuple1 = (7, 2) 
test_tuple2 = (7, 8)
list_a=[]
for i in test_tuple1:
    for j in test_tuple2:
        list_a.append((i,j))
print(list_a)
for i in test_tuple2:
    for j in test_tuple1:
        list_a.append((i,j))
print(list_a)

Output:
[(7, 7), (7, 8), (2, 7), (2, 8)]
[(7, 7), (7, 8), (2, 7), (2, 8), (7, 7), (7, 2), (8, 7), (8, 2)]

Q95.) Write a Python program to sort a list of tuples by second item.
```
Input : [('for', 24), ('Geeks', 8), ('Geeks', 30)] 
Output : [('Geeks', 8), ('for', 24), ('Geeks', 30)]
```
Ans:)#code
list_tuples=[('for', 24), ('Geeks', 8), ('Geeks', 30)]
def sort(tup):
    for i in range(0,len(tup)):
        for j in range(len(tup)-i-1):
            if (tup[j+1][1]<tup[j][1]):
              temp=tup[j]
              tup[j]=tup[j+1]
              tup[j+1]=temp
    return(tup)
print("Sorted list of tuples by second item =", sort(list_tuples))

Output:
Sorted list of tuples by second item = [('Geeks', 8), ('for', 24), ('Geeks', 30)]

Q96.) Write a python program to print below pattern.
```
* 
* * 
* * * 
* * * * 
* * * * * 
```  
Ans:)#code
rows=5
for i in range(0,rows):
    for j in range(0,i+1):
        print("* ",end="")
    print("")

Q97.) Write a python program to print below pattern.
```
    *
   **
  ***
 ****
*****
```
Ans:) #code
rows=int(input("Enter number of rows or height of given triangle="))
for num in range(1,rows+1):
    for space in range(0,rows-num+1):
        print(" ",end="")
    for symbol in range(1, num+1):
        print("*",end="")
        #"*", 1,12,123,1234,12345
        #"* "->normal triangle
        #"{0}".format(symbol)
    print()

Q98.) Write a python program to print below pattern.
```
    * 
   * * 
  * * * 
 * * * * 
* * * * * 
```
Ans:) #code
rows=int(input("Enter number of rows or height of given triangle="))
for num in range(1,rows+1):
    for space in range(0,rows-num+1):
        print(" ",end="")
    for symbol in range(1, num+1):
        print("* ",end="")
        #"*", 1,12,123,1234,12345
        #"* "->normal triangle
        #"{0}".format(symbol)
    print()

Q99.) Write a python program to print below pattern.
```
1 
1 2 
1 2 3 
1 2 3 4 
1 2 3 4 5
```
Ans:)#code
rows=int(input("Enter number of rows or height of given triangle="))
for num in range(1,rows+1):
    for symbol in range(1, num+1):
        print("{0} ".format(symbol),end="")
    print()

Q100.) Write a python program to print below pattern.
```
A 
B B 
C C C 
D D D D 
E E E E E 
```
Ans:) #code
rows=int(input("Enter number of rows or height of given triangle="))
# 65 in char is A
# 90 in char is Z
for num in range(1,rows+1):
    for symbol in range(1, num+1):
        print(chr(num+64),end=" ")
    print()