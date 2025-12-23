<hr>

<h2>Object-Oriented Programming (OOP) in Python</h2>
<p>
Object-Oriented Programming (OOP) is a programming paradigm that organizes
code using <b>classes</b> and <b>objects</b>. It helps in writing reusable,
maintainable, and structured programs by modeling real-world entities.
</p>

<hr>

<h3>Class</h3>
<p>
A <b>class</b> is a blueprint or template used to create objects.
It defines variables (data) and methods (functions) that an object will have.
</p>

<pre>
class Student:
    name = "Ravi"
    age = 21
</pre>

<p>
Here, <code>Student</code> is a class that contains variables <code>name</code>
and <code>age</code>.
</p>

<hr>

<h3>Object</h3>
<p>
An <b>object</b> is an instance of a class. It represents a real-world entity
created using the class blueprint.
</p>

<pre>
s1 = Student()
print(s1.name)
print(s1.age)
</pre>

<p>
Here, <code>s1</code> is an object of the <code>Student</code> class.
</p>

<hr>

<h3>The self Keyword</h3>
<p>
The <b>self</b> keyword represents the current object. It is used to access
instance variables and methods inside a class.
</p>

<pre>
class Demo:
    def show(self):
        print("This is self example")

obj = Demo()
obj.show()
</pre>

<p>
Without <code>self</code>, Python cannot identify which object's data is being accessed.
</p>

<hr>

<h3>Instance Variables</h3>
<p>
Instance variables are variables that belong to a specific object.
They are defined using <code>self</code>.
</p>

<pre>
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age

p1 = Person("Ram", 22)
p2 = Person("Shyam", 25)
</pre>

<p>
Each object has its own copy of instance variables.
</p>

<hr>

<h3>Class Variables</h3>
<p>
Class variables are shared among all objects of a class.
</p>

<pre>
class Company:
    company_name = "ABC Pvt Ltd"

    def show(self):
        print(self.company_name)

c1 = Company()
c2 = Company()
</pre>

<hr>

<h3>Constructor (__init__ Method)</h3>
<p>
A constructor is a special method that is automatically called
when an object is created. It is used to initialize data.
</p>

<pre>
class Employee:
    def __init__(self, id, salary):
        self.id = id
        self.salary = salary

e1 = Employee(101, 25000)
</pre>

<hr>

<h3>Methods in a Class</h3>
<p>
A method is a function defined inside a class. It performs operations
using object data.
</p>

<pre>
class Calculator:
    def add(self, a, b):
        return a + b

    def sub(self, a, b):
        return a - b

calc = Calculator()
print(calc.add(10, 5))
print(calc.sub(10, 5))
</pre>

<hr>

<h3>Calling One Method Inside Another</h3>
<p>
A method can call another method of the same class using <code>self</code>.
</p>

<pre>
class Math:
    def add(self):
        print(10 + 20)

    def display(self):
        self.add()

m = Math()
m.display()
</pre>

<hr>

<h3>Advantages of OOP</h3>
<ul>
  <li>Code reusability</li>
  <li>Better organization of code</li>
  <li>Easy maintenance</li>
  <li>Real-world problem modeling</li>
  <li>Improved readability</li>
</ul>

<hr>

<h2>Final Summary</h2>
<p>
This README covers complete <b>Python Fundamentals</b> including variables,
data types, operators, loops, functions, file handling, exception handling,
and <b>Object-Oriented Programming concepts</b> such as class, object, self,
constructors, variables, and methods.
</p>

<p>
These concepts form a strong foundation for:
</p>

<ul>
  <li>Python exams</li>
  <li>Technical interviews</li>
  <li>Real-world Python projects</li>
  <li>Advanced topics like Django, Data Science, and Machine Learning</li>
</ul>
