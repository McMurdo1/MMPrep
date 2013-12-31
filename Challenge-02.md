From the Lynda.com video series “Foundations of Programming: Object-Oriented
Design”, watch each (short) video and answer the correlating questions:


Section 0: Introduction
=======================
[0.1] What to expect from this course (3:06)
--------------------------------------------
What is the intended purpose and potential advantage of learning object oriented
design?

It's a framework designed to allow great communication and reduce errors, inflexibility, and wasted time. 

[0.2] Exploring object-oriented analysis, design, and development (1:41)
------------------------------------------------------------------------
Why might it be advantageous to analyze and design before beginning programming?

Understanding what problem you're trying to solve and how you plan on solving it will help guide what you program. It allows the developer to focus on the right things and do them the right way, with a better understanding of how what is being programmed fits into the big picture of solving the problem. 

[0.3] Reviewing software development methodologies (4:08)
---------------------------------------------------------
What is the difference between a "waterfall" and an "agile" approach to
development? What is an iteration and how do we to use them to build software?

Agile is designed to be more responsive to problems that come up during development. When one feature is complete in waterfall development, it may contain errors or unexpected corner cases. Agile is designed to address these. An iteration is usually a short sprint (a few weeks) between pushes where new feature are built or problems with existing features are address. 


Section 1: Core Concepts
========================
[1.1] Why we use object-orientation (2:42)
------------------------------------------
What are the various types of programming languages and in which domain is each
used?

Procedural languages such as Cobol and Fortran are used on mainframes. Functional programming languages are used in specialized settings such as academia. Most commercial applications use object oriented programming.

[1.2] What is an object? (5:22)
-------------------------------
Describe in your own words the three properties of a computing object.

Identity: The actual name of an object that uniquely distinguishes it from other objects.
Attributes: The characteristics of an object. Different objects can have the same attributes but with different values. The attributes are the minimal characteristics required to make an object, ignoring things that are unimportant. The "nouns" of the object.
Behaviors: What can be done with an object.  The "verbs" of the object.

[1.3] What is a class? (4:43)
-----------------------------
Explain how classes are analogous to blueprints. Include the relationship
between a class and an object. Can you think of how the analogy breaks down?

Classes are what objects are built off of. They describe the generic names, attributes, and behavior of classes. However, unlike blueprints, which describe in detail exactly how each house should be built, the objects created from a class may differ. Building 1000 houses off the same blueprint would give you 1000 exact copies of the house. With objects and classes, each object may have four walls, but the size and color of the walls may be different. 

[1.4] What is abstraction? (2:45)
---------------------------------
When a developer uses the term “abstraction” what are they describing?

Focusing on the basic principles that define a class/object rather than the specifics of the any one instance.


[1.5] What is encapsulation? (3:45)
-----------------------------------
What does encapsulation prevent? What does it enable?

Encapsulation is protecting or hiding data within an object from everything outside the object. The idea is to limit the interdependencies and protect against bad effects of making changes.

[1.6] What is inheritance? (3:35)
---------------------------------
Describe the inheritance relationship between classes. When would this
relationship be advantageous to establish?

Inheritance is a way to reuse code between classes without having to re-write the code. If a class uses all the same attributes or behaviors as another class, but requires a few new ones, you can make the new class a subclass of the original class. The subclass will have all the attributes and behaviors as the superclass, and you can make any changes as necessary.

[1.7] What is polymorphism? (3:22)
----------------------------------
What is the basic idea behind polymorphism? How can it make the classes we
create more flexible?

Polymorphism allows the program to do the right thing when working with different forms. It can be used to perform the correct action even when using inherited classes, as each subclass can use polymorphism to make behavioral changes specific to its unique rules. 


Section 2: Object-Oriented Analysis and Design
==============================================
[2.1] Understanding the object-oriented analysis and design processes (4:13)
----------------------------------------------------------------------------
What are the steps of analysis that come before writing code for an application?
Why do you think these steps make writing the code easier?

Gather requirements, describe the application, identify the most important objects, describe the interactions between those objects, and create a class diagram. These steps will help avoid conflict between different objects and create a more efficient program. 

[2.2] Defining requirements (6:09)
----------------------------------
What should you have after you've completed the first phase of defining your
requirements?

Something written down which describes the requirements.

[2.3] Introduction to the Unified Modeling Language (UML) (1:54)
----------------------------------------------------------------
What is UML? Why Is it useful to visualize your application before coding it?

Unified Modeling Language. Visualizing the application is helpful for seeing where things live and how they interact with each other.

Section 3: Utilizing Use Cases
==============================
[3.1] Understanding use cases (6:11)
------------------------------------
Write a use case for creating an event on your phone's calendar.

Title: Create Event
Actor: User
Scenario: User provides event title, location, start time, and end time.

[3.2] Identifying the actors (4:16)
-----------------------------------
Can you think of a use case for a mobile application in which the actor is not
the user of the mobile device?

When the user logs in to an application using Facebook, Facebook will validate the credentials. In that case, Facebook is an actor providing information into the app. 

[3.3] Identifying the scenarios (5:07)
--------------------------------------
Write another use case for a mobile device user interacting with a calendar
application. This time include a couple extensions when crafting your scenario.

Title: Create Event
Actor: User
Scenario: User provides event title, location, start time, and end time.
Extension: The user may set an alarm to be reminded of the upcoming event.
Extension: The user is alerted if the end time is before the beginning time.


[3.4] Diagramming use cases (4:18)
----------------------------------
Do a google image search for "use case diagram." Notice how many variations
there are. What do they all generally have in common?

They all use stick figures for actors and ellipses for use cases. The use cases are all in boxes representing the systems. Lines represent interaction between actors and use cases.

[3.5] Employing user stories (3:43)
-----------------------------------
Write 5 user stories to describe a mobile user interacting with his or her maps
application.

1) As a user I need to know my present location so that I have a reference point.
2) As a user I need to be able to input a destination so that the map knows where I'm going.
3) As a user I need to get transit directions so that I know which bus to take.
4) As a user I need to be able to zoom in so I can see street names.
5) As a user I need to see buildings so that I can visually identify landmarks.


Section 4: Domain Modeling (Modeling the App)
=============================================
[4.1] Creating a conceptual model (1:59)
----------------------------------------
What’s your favorite color?

White

[4.2] Identifying the classes (2:27)
------------------------------------
Identify the classes in the use case you constructed for a user interacting with
his or her calendar application in chapter 3.

User
Event
Time
Location
Alert


[4.3] Identifying class relationships (2:38)
--------------------------------------------
Identify the relationships among the classes you found above. Create a
conceptual model where you diagram these relationships and then upload a picture
of your model below.

**ANSWER HERE**

[4.4] Identifying class responsibilities (6:43)
-----------------------------------------------
Identify the responsibilities of the classes you found above. List them here.

User inputs start time, end time, title, and location
Alert checks is end time is before start time

[4.5] Using CRC cards (2:49)
----------------------------
If you’d like, try creating CRC cards for the model you made above. There's no
need to respond here, just try it out and see if you like this form of
organization.

**ANSWER HERE… IF YOU LIKE**


Section 5: Creating Classes
===========================
[5.1] Creating class diagrams (6:11)
------------------------------------
Construct Class Diagrams for the classes you imagine exist in a twitter app, a
maps app, a calendar app, or any other app you would like to make. Do you find
that it is easier to come up with the attributes or with the behaviors? Why do
you think that is?

Attributes. When thinking of an object it's easy to think of the attributes that define the object. It's harder to think of what that object does and how it relates to other objects. 

[5.2] Converting class diagrams to code (4:57)
----------------------------------------------
How might the separation of interface and implementation in Objective-C be an
advantage when working with class diagrams?

It clearly delineates working on the attributes in the interface versus working on the behaviors in the implementation. 

[5.3] Exploring object lifetime (5:55)
--------------------------------------
What are the constructors and destructors in Objective-C? Why do we use them?

The constructors are alloc and init. They are used to ensure that new classes are set to a meaningful state. Destructors are used to destroy an object at the end of its life, generally to free resources.

[5.4] Using static or shared members (5:22)
-------------------------------------------
Like the interest rate example in the video, give three additional examples of
data that would be the same for all instances of a class.

Gravitational constant
Fuel efficiency of a model of car
Fixed costs associated with a product


Section 6: Inheritance and Composition
======================================
6.1 Identifying inheritance situations (6:49)
---------------------------------------------
Describe in your own words what inheritance is and how it is useful when
constructing classes.

Inheritance is used to create variations of a common theme. If you have a lot of items that are very similar and share many attributes, you can create a superclass of them and make each subclass inherit the common items from the super class. It can be useful and more efficient so you don't have to create classes that have the same attributes or methods over and over again. 

[6.2] Using inheritance (2:43)
------------------------------
Referring to the apps on your phone, come up with three examples where you
believe methods are being inherited from superclasses and called by subclasses.

In the Starbucks app, the drinks might inherit from "hot" or "cold" super classes. Likewise, when giving egift cards through the app, the "From" information might inherit from my account information. In Fruit Ninja, each specifc type of fruit (apple, banana, etc) might inherit from a generic "fruit" super class. 
