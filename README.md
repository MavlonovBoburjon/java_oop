# Java OOP
![image](https://user-images.githubusercontent.com/109073010/192253367-0b8c058c-5279-4470-aaf8-aebc1b8cd6fa.png)

>## Definition of OOP Concepts in Java
>The main ideas behind Java’s Object-Oriented Programming, OOP concepts include abstraction, encapsulation, inheritance and polymorphism. Basically, Java OOP concepts let us create working methods and variables, then re-use all or part of them without compromising security. Grasping OOP concepts is key to understanding how Java works.
# ♦Abstraction
![image](https://user-images.githubusercontent.com/109073010/192253712-2a5498e7-d5b6-4ed2-ae4c-bc230d0fe4bd.png)

Using simple things to represent complexity. We all know how to turn the TV on, but we don’t need to know how it works in order to enjoy it. In Java, abstraction means simple things like objects, classes and variables represent more complex underlying code and data. This is important because it lets you avoid repeating the same work multiple times.
>## How Abstraction Works
>Abstraction lets programmers create useful and reusable tools. For example, a programmer can create several different types of objects, which can be variables, functions or data structures. Programmers can also create different classes of objects as ways to define the objects. For instance, a class of variable might be an address. The class might specify that each address object shall have a name, street, city and zip code. The objects, in this case, might be employee addresses, customer addresses or supplier addresses.For instance, a class of variable might be an address. The class might specify that each address object shall have a name, street, city and zip code. The objects, in this case, might be employee addresses, customer addresses or supplier addresses.
# ♦Encapsulation
![image](https://user-images.githubusercontent.com/109073010/192254398-011642ca-21ea-4862-b405-13aaa9ecc36f.png)

The practice of keeping fields within a class private, then providing access to those fields via public methods. Encapsulation is a protective barrier that keeps the data and code safe within the class itself. We can then reuse objects like code components or variables without allowing open access to the data system-wide.
>## How Encapsulation Works
>Encapsulation lets us reuse functionality without jeopardizing security. It’s a powerful, time-saving OOP concept in Java. For example, we may create a piece of code that calls specific data from a database. It may be useful to reuse that code with other databases or processes. Encapsulation lets us do that while keeping our original data private. It also lets us alter our original code without breaking it for others who have adopted it in the meantime.
# ♦Inheritance
![image](https://user-images.githubusercontent.com/109073010/192255436-9cfa5d70-9ef1-44f3-915b-a22f7c8de45b.png)

A special feature of Object-Oriented Programming in Java, Inheritance lets programmers create new classes that share some of the attributes of existing classes. Using Inheritance lets us build on previous work without reinventing the wheel.
>## How Inheritance Works
>Inheritance is another labor-saving Java OOP concept that works by letting a new class adopt the properties of another. We call the inheriting class a subclass or a child class. The original class is often called the parent. We use the keyword extends to define a new class that inherits properties from an old class.

# ♦Polymorphism
![image](https://user-images.githubusercontent.com/109073010/192257183-d9c1e9f9-acea-4a40-a7c7-ed8f020294ef.png)

Allows programmers to use the same word in Java to mean different things in different contexts. One form of polymorphism is method overloading. That’s when the code itself implies different meanings. The other form is method overriding. That’s when the values of the supplied variables imply different meanings. Let’s delve a little further.
>## How Polymorphism Works
>Polymorphism in Java works by using a reference to a parent class to affect an object in the child class. We might create a class called “horse” by extending the “animal” class. That class might also implement the “professional racing” class. The “horse” class is “polymorphic,” since it inherits attributes of both the “animal” and “professional racing” class.
>
>Two more examples of polymorphism in Java are method overriding and method overloading.
>
>In method overriding, the child class can use the OOP polymorphism concept to override a method of its parent class. That allows a programmer to use one method in different ways depending on whether it’s invoked by an object of the parent class or an object of the child class.
>
>In method overloading, a single method may perform different functions depending on the context in which it’s called. This means a single method name might work in different ways depending on what arguments are passed to it.
# 
## Examples of OOP Concepts in Java 
Now that we explained the foundational OOP concepts in Java, let’s look at a few common examples.

>### Short Encapsulation Example in Java
>In the example below, encapsulation is demonstrated as an OOP concept in Java. Here, the variable “name” is kept private or “encapsulated.”
  
	//save as Student.java
    package com.javatpoint;
    
    public class Student {
        private String name;
        public String getName() {
            return name;
        }
        public void setName(String name) {
            this.name = name;
        }
    }
    
    
    //save as Test.java
    package com.javatpoint;
    class Test {
        public static void main(String[] args) {
            Student s = new Student();
            s.setName("Donik");
            System.out.println(s.getName());
        }
    }
# 
	Compile By: javac -d . Test.java
	Run By: java com.javatpoint.Test

	Output: Donik
	
>## Example of Inheritance in Java
>It’s quite simple to achieve inheritance as an OOP concept in Java. Inheritance can be as easy as using the extends keyword:

	class Students {

	}
	class Teachers extends Students {

	}
	class Univercity extends Teachers {

	}
#
>## Short Example of Polymorphism in Java
>In the example below of polymorphism as an OOP concept in Java, we have two classes: Person and Employee. The Employee class inherits from the Person class by using the keyword extends. Here, the child class overrides the parent class.

	package com.javatpoint;

	class Person {
    	void walk() {
        	System.out.println("Can Run….");
    	}
	}
	class Employee extends Person {
    	public static void main(String args[]) {
        	Person p = new Employee(); //upcasting
        	p.walk();
    	}
    	void walk() {
        	System.out.println("Running Fast…");
    	}
	}
#
	Compile By: javac -d . Employee.java
	Run By: java com.javatpoint.Employee

	Output: Running Fast…
#	
