<h1>Python Fundamentals – Detailed Explanation</h1>
<hr>

<h2>Python Variables</h2>
<p>
A variable in Python is a named location in memory that stores data.
When we assign a value to a variable, Python automatically decides the
type of data stored. This is called <b>dynamic typing</b>.
</p>

<p>
Variables make programs flexible and reusable. Instead of using fixed
values repeatedly, we store values in variables and use them whenever required.
</p>

<h3>Important Rules for Variables</h3>
<ul>
  <li>Variable names must start with a letter or underscore (_)</li>
  <li>They cannot start with a number</li>
  <li>Only letters, numbers, and underscores are allowed</li>
  <li>Python is case-sensitive (age and Age are different)</li>
  <li>Keywords like if, for, while cannot be used as variable names</li>
</ul>

<h3>Examples</h3>
<pre>
x = 10        # integer variable
name = "Ram" # string variable
_marks = 90
</pre>

<p>
In the above example, Python automatically assigns data types to variables
based on the values stored.
</p>

<hr>

<h2>Python Data Types</h2>
<p>
Data types specify what kind of data a variable can store.
Python provides built-in data types to handle numbers, text, and collections.
</p>

<h3>Numeric Data Types</h3>
<p>
Numeric data types are used to store numerical values.
</p>

<ul>
  <li><b>int</b> – stores whole numbers (positive or negative)</li>
  <li><b>float</b> – stores decimal values</li>
  <li><b>complex</b> – stores real and imaginary values</li>
</ul>

<pre>
a = 25
b = 10.5
c = 3 + 4j

print(type(a))
print(type(b))
print(type(c))
</pre>

<p>
Integers are used for counting, floats for precision values, and complex
numbers mainly in scientific calculations.
</p>

<hr>

<h3>String Data Type</h3>
<p>
A string is a sequence of characters enclosed in single, double,
or triple quotes. Strings are <b>immutable</b>, meaning once created,
they cannot be changed.
</p>

<pre>
text = "Python Programming"
print(text[0])      # First character
print(text[-1])     # Last character
print(text[0:6])    # Slicing
</pre>

<h3>Important String Operations</h3>
<pre>
s = " python language "
print(s.upper())
print(s.lower())
print(s.strip())
print(s.replace("python", "java"))
print(s.split())
</pre>

<p>
Strings are widely used for handling user input, messages, and text processing.
</p>

<hr>

<h3>List Data Type</h3>
<p>
A list is an ordered, mutable collection of elements.
It allows duplicate values and different data types in a single list.
</p>

<pre>
data = [10, "Python", 3.5]
data.append(100)
data[0] = 50
print(data)
</pre>

<p>
Lists are commonly used when data needs to be modified frequently.
</p>

<hr>

<h3>Tuple Data Type</h3>
<p>
A tuple is similar to a list, but it is immutable.
Once created, elements cannot be added, removed, or modified.
</p>

<pre>
t = (10, 20, 30)
print(t[1])
</pre>

<p>
Tuples are used to protect data from accidental modification.
</p>

<hr>

<h3>Set Data Type</h3>
<p>
A set is an unordered collection of unique elements.
Duplicate values are automatically removed.
</p>

<pre>
s = {1, 2, 3, 3, 4}
print(s)
</pre>

<h3>Set Operations</h3>
<pre>
a = {1, 2, 3}
b = {3, 4, 5}
print(a.union(b))
print(a.intersection(b))
</pre>

<p>
Sets are mainly used for mathematical operations and removing duplicates.
</p>

<hr>

<h3>Dictionary Data Type</h3>
<p>
A dictionary stores data in key-value pairs.
Keys must be unique and immutable, while values can be any data type.
</p>

<pre>
student = {
  "name": "Ravi",
  "age": 21,
  "course": "Python"
}

print(student["name"])
print(student.get("age"))
</pre>

<p>
Dictionaries are used to represent structured data like records.
</p>

<hr>

<h2>Type Conversion</h2>
<p>
Type conversion is the process of converting one data type into another.
It can be implicit or explicit.
</p>

<h3>Implicit Type Conversion</h3>
<pre>
x = 10
y = 5.5
z = x + y
print(z)
print(type(z))
</pre>

<p>
Python automatically converts int to float to avoid data loss.
</p>

<h3>Explicit Type Conversion</h3>
<pre>
a = "100"
b = int(a)
print(b + 20)
</pre>

<p>
Explicit conversion is done manually using functions like int(), float(), str().
</p>

<hr>

<h2>Python Operators</h2>

<h3>Arithmetic Operators</h3>
<pre>
a = 10
b = 3
print(a + b)
print(a - b)
print(a * b)
print(a / b)
print(a % b)
</pre>

<h3>Comparison Operators</h3>
<pre>
print(10 > 5)
print(10 == 5)
print(10 != 5)
</pre>

<h3>Logical Operators</h3>
<pre>
x = True
y = False
print(x and y)
print(x or y)
print(not x)
</pre>

<h3>Membership Operators</h3>
<pre>
nums = [1, 2, 3]
print(2 in nums)
print(5 not in nums)
</pre>

<h3>Identity Operators</h3>
<pre>
a = 10
b = 10
print(a is b)
print(a is not b)
</pre>

<hr>

<h2>Loops</h2>

<h3>for Loop</h3>
<pre>
for i in range(1, 6):
    print(i)
</pre>

<h3>while Loop</h3>
<pre>
i = 1
while i <= 5:
    print(i)
    i += 1
</pre>

<h3>Loop Control Statements</h3>
<pre>
for i in range(1, 6):
    if i == 3:
        continue
    if i == 5:
        break
    print(i)
</pre>

<hr>

<h2>Functions</h2>

<h3>Function Definition</h3>
<pre>
def greet():
    print("Hello Python")

greet()
</pre>

<h3>Function with Parameters and Return</h3>
<pre>
def add(a, b):
    return a + b

print(add(10, 20))
</pre>

<h3>Default Arguments</h3>
<pre>
def welcome(name="User"):
    print("Welcome", name)

welcome()
welcome("Python")
</pre>

<hr>

<h2>Lambda Functions</h2>
<pre>
square = lambda x: x * x
print(square(5))
</pre>

<hr>

<h2>File Handling</h2>
<pre>
file = open("data.txt", "w")
file.write("Hello Python")
file.close()

file = open("data.txt", "r")
print(file.read())
file.close()
</pre>

<hr>

<h2>Exception Handling in Python</h2>
<p>
Exception handling is used to handle runtime errors so that the normal
flow of the program is not interrupted.
</p>

<h3>try and except</h3>
<pre>
try:
    a = 10 / 0
except ZeroDivisionError:
    print("Cannot divide by zero")
</pre>

<h3>Exception Keyword</h3>
<pre>
try:
    x = int("abc")
except Exception as e:
    print("Error:", e)
</pre>

<h3>finally Block</h3>
<pre>
try:
    print(10 / 2)
except:
    print("Error occurred")
finally:
    print("This block always executes")
</pre>

<hr>

<h2>Common Errors in Python</h2>

<h3>NameError</h3>
<pre>
print(x)
</pre>

<h3>ValueError</h3>
<pre>
int("abc")
</pre>

<h3>IndentationError</h3>
<pre>
if True:
print("Hello")
</pre>

<h3>ZeroDivisionError</h3>
<pre>
print(10 / 0)
</pre>

<h3>SyntaxError</h3>
<pre>
if True
    print("Hi")
</pre>

<h3>FileNotFoundError</h3>
<pre>
open("sample.txt")
</pre>



<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Object-Oriented Programming (OOP) in Python – Detailed Explanation</title>
</head>
<body>

<h1>Object-Oriented Programming (OOP) in Python – Detailed Explanation</h1>

<p>
This document explains the <b>concepts used in the given Python file</b> and also provides a
<b>very detailed explanation of core OOP topics</b> such as
<b>class, object, self, variables, and methods</b> with clear examples.
</p>

<hr>

<h2>1. What is Object-Oriented Programming (OOP)?</h2>

<p>
<b>Object-Oriented Programming (OOP)</b> is a programming approach where we organize code using
<b>classes</b> and <b>objects</b>.
</p>

<p>Instead of writing only functions, OOP helps us:</p>
<ul>
    <li>Group related data and behavior together</li>
    <li>Make code reusable</li>
    <li>Make programs easier to understand and maintain</li>
</ul>

<p>Python supports OOP completely.</p>

<hr>

<h2>2. Class</h2>

<h3>What is a Class?</h3>

<p>
A <b>class</b> is a <b>blueprint or template</b> for creating objects.
</p>

<p>
Think of a class like a <b>design of a house</b>:
</p>

<ul>
    <li>The design is the same</li>
    <li>But many houses (objects) can be built from it</li>
</ul>

<h3>Syntax of a Class</h3>

<pre>
class ClassName:
    variables
    methods
</pre>

<h3>Example from the Given File</h3>

<pre>
class PPP:
    a = 10
    b = 20
</pre>

<p>Here:</p>
<ul>
    <li><code>PPP</code> is a <b>class</b></li>
    <li><code>a</code> and <code>b</code> are <b>class variables</b></li>
</ul>

<hr>

<h2>3. Object</h2>

<h3>What is an Object?</h3>

<p>
An <b>object</b> is a <b>real instance</b> of a class.
</p>

<ul>
    <li>Class = Blueprint</li>
    <li>Object = Actual thing created using the blueprint</li>
</ul>

<h3>Example</h3>

<pre>
anil = PPP()
</pre>

<p>Here:</p>
<ul>
    <li><code>PPP()</code> creates an object</li>
    <li><code>anil</code> is an object of class <code>PPP</code></li>
</ul>

<p>You can create multiple objects:</p>

<pre>
x = PPP()
y = PPP()
</pre>

<p>Each object can access the class data and methods.</p>

<hr>

<h2>4. Variables in OOP</h2>

<h3>Types of Variables in Python Classes</h3>

<h3>1️⃣ Class Variables</h3>

<ul>
    <li>Defined <b>inside the class</b></li>
    <li>Shared by <b>all objects</b></li>
</ul>

<pre>
class PPP:
    a = 10
    b = 20
</pre>

<p>All objects of <code>PPP</code> share <code>a</code> and <code>b</code>.</p>

<hr>

<h3>2️⃣ Instance Variables</h3>

<ul>
    <li>Defined using <code>self</code></li>
    <li>Different for each object</li>
</ul>

<pre>
class Student:
    def __init__(self, name, marks):
        self.name = name
        self.marks = marks
</pre>

<p>Here:</p>
<ul>
    <li><code>name</code> and <code>marks</code> are <b>instance variables</b></li>
</ul>

<hr>

<h2>5. Functions vs Methods</h2>

<h3>Function</h3>

<p>A <b>function</b> is written outside a class.</p>

<pre>
def add(a, b):
    return a + b
</pre>

<hr>

<h3>Method</h3>

<p>A <b>method</b> is a function written <b>inside a class</b>.</p>

<pre>
class Demo:
    def show(self):
        print("Hello")
</pre>

<hr>

<h2>6. self Keyword (Very Important)</h2>

<h3>What is <code>self</code>?</h3>

<p>
<code>self</code> refers to the <b>current object</b>.
</p>

<p>It is used to:</p>
<ul>
    <li>Access variables of the current object</li>
    <li>Call other methods of the same class</li>
</ul>

<h3>Why <code>self</code> is Required?</h3>

<p>
Without <code>self</code>, Python does not know <b>which object</b> is using the method.
</p>

<h3>Example from the Given File</h3>

<pre>
def add(self):
    print(self.a + self.b)
</pre>

<p>Here:</p>
<ul>
    <li><code>self.a</code> refers to variable <code>a</code> of the object</li>
    <li><code>self.b</code> refers to variable <code>b</code> of the object</li>
</ul>

<hr>

<h2>7. Methods in the Given File</h2>

<h3>add() Method</h3>

<pre>
def add(self):
    print(self.a + self.b)
</pre>

<ul>
    <li>Adds <code>a</code> and <code>b</code></li>
    <li>Uses object variables</li>
</ul>

<h3>sub() Method</h3>

<pre>
def sub(self):
    print(self.a - self.b)
</pre>

<ul>
    <li>Subtracts <code>b</code> from <code>a</code></li>
</ul>

<h3>mult() Method</h3>

<pre>
def mult(self):
    print(self.a * self.b)
</pre>

<ul>
    <li>Multiplies <code>a</code> and <code>b</code></li>
</ul>

<h3>div() Method</h3>

<pre>
def div(self):
    print(self.a / self.b)
</pre>

<ul>
    <li>Divides <code>a</code> by <code>b</code></li>
</ul>

<hr>

<h2>8. Calling One Method Inside Another Method</h2>

<h3>common() Method</h3>

<pre>
def common(self):
    self.add()
    self.sub()
    self.mult()
    self.div()
</pre>

<h3>Explanation</h3>

<ul>
    <li>One method is calling other methods</li>
    <li><code>self.method_name()</code> is used</li>
    <li>Helps reduce repeated code</li>
</ul>

<hr>

<h2>9. Object Calling a Method</h2>

<pre>
anil = PPP()
anil.common()
</pre>

<h3>Execution Flow</h3>

<ol>
    <li>Object <code>anil</code> is created</li>
    <li><code>common()</code> method is called</li>
    <li>Inside <code>common()</code>:
        <ul>
            <li><code>add()</code> runs</li>
            <li><code>sub()</code> runs</li>
            <li><code>mult()</code> runs</li>
            <li><code>div()</code> runs</li>
        </ul>
    </li>
</ol>

<hr>

<h2>10. Another Class Example (Simple)</h2>

<pre>
class Calculator:
    def __init__(self, x, y):
        self.x = x
        self.y = y

    def add(self):
        return self.x + self.y

c = Calculator(5, 3)
print(c.add())
</pre>

<h3>Explanation</h3>

<ul>
    <li><code>__init__</code> initializes values</li>
    <li><code>self.x</code> and <code>self.y</code> are instance variables</li>
    <li>Object <code>c</code> accesses methods</li>
</ul>

<hr>

<h2>11. Summary of Concepts Used</h2>

<table border="1" cellpadding="8">
    <tr>
        <th>Concept</th>
        <th>Explanation</th>
    </tr>
    <tr>
        <td>Class</td>
        <td>Blueprint of objects</td>
    </tr>
    <tr>
        <td>Object</td>
        <td>Instance of class</td>
    </tr>
    <tr>
        <td>self</td>
        <td>Refers to current object</td>
    </tr>
    <tr>
        <td>Variables</td>
        <td>Store data</td>
    </tr>
    <tr>
        <td>Methods</td>
        <td>Functions inside class</td>
    </tr>
    <tr>
        <td>Method Calling</td>
        <td>One method calls another</td>
    </tr>
    <tr>
        <td>OOP</td>
        <td>Organizing code using classes</td>
    </tr>
</table>

<hr>

<h2>12. Why OOP is Important?</h2>

<ul>
    <li>Code reusability</li>
    <li>Easy maintenance</li>
    <li>Real-world modeling</li>
    <li>Better structure for large programs</li>
</ul>

</body>
</html>


