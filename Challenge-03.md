Challenge 3: Get Your Hands Dirty
=================================
Next up, find the Lynda.com video series entitled: “Objective-C Essential
Training”. Watch each video in the following list and answer the corresponding
question.

Section 1: Getting Started
==========================
[1.1] Installing the tools (4:42)
---------------------------------
You should already have Xcode installed, but you will need to register as an
Apple Developer.

Do you like cats?

They're okay.

[1.2] Creating your first application (11:28)
---------------------------------------------
Create your first application using the same steps Simon describes in the video.
Familiarize yourself with the Xcode environment, specifically notice how it can
be manipulated to display different helper tools and how it will attempt to fill
in your code as you type it.

Cross my heart...

[1.3] Updates to this course (3:31)
-----------------------------------
Why do you think it's important to be aware of the idiosyncracies with older
versions of Objective-C and to keep up with new features as they are added?

Being aware of older versions is important because you will run across those versions "in the wild", and it's important to know what the idiosyncracies are doing. Likewise, if you don't keep up with them, you'll end up wasting time by not using more efficient code or coming across new code you don't recognize. 

Section 2: Objective-C Basics
=============================
[2.1] The Objective-C language (4:11)
-------------------------------------
How did Objective-C become the language to learn if you want to make apps for
the iPhone and iPad?

Objective-C was the language adopted by NeXT, founded by Steve Jobs when he left Apple. When Apple bought NeXT computers, they also adopted their programming standards. Further iterations of Apple devices, including the iPhone and iPad, subsequently ran on later versions of Objective-C.

[2.2] The structure of an Objective-C program (6:15)
----------------------------------------------------
Create a new project. Go to the menu option `Xcode`, `Preferences`,
`Text Editing` and make sure *Line Numbers* is checked in the section marked
"Show." Then add comments describing the purpose of each auto-generated line in
the main.m file. For example on Line 17 I would write: 

```
NSLog(@"Hello, World!");  // instructs the console to output: Hello, World!
```

[2.3] Compiling and running your code (8:37)
--------------------------------------------
Why might you build in one version of iOS but deploy in an older version?

To allow your users who might have an older version of iOS to use your app.



Section 3: Program Flow
=======================
[3.1] Logging messages to the command line (6:07)
-------------------------------------------------
Following the example in the video, write a program that calculates and outputs
to the console the number of seconds in ten years. Copy and paste your code
here.

#import <Foundation/Foundation.h>

int main(int argc, const char * argv[])
{

    @autoreleasepool {
        
        // insert code here...
       
        int seconds = 60;
        int minutes = 60;
        int hours = 24;
        float days = 365.242;
        int decade = 10;
        
        float secondsInADecade = seconds * minutes * hours * days * decade;
        
        NSLog(@"There are %f seconds in a decade", secondsInADecade);
        
    }
    return 0;
}

[3.2] Writing conditional code (7:01)
-------------------------------------
Using Objective-C, create an integer variable called "day" that represents the
days of the week. Write an if statement that checks whether "day" is a weekend
day. If the day is a weekend day then have your program print a message saying
"Have a nice weekend!" and if it's not, print a message saying "I hope you're
having a good week!"

#import <Foundation/Foundation.h>

int main(int argc, const char * argv[])
{

    @autoreleasepool {
        
        // insert code here...
       
        int day = 6;
        
        if ( day > 5 )
        {
            NSLog(@"Have a nice weekend!");
        }
        else
        {
            NSLog(@"I hope you're having a good week!");
        }
        
    }
    return 0;
}

[3.3] The switch statement (5:58)
---------------------------------
Create a variable called "hurricaneCategory" and a switch statement that prints
out a message describing a hurricane's category from 1-5.

#import <Foundation/Foundation.h>

int main(int argc, const char * argv[])
{

    @autoreleasepool {
        
        // insert code here...
       
        int hurricaneCategory = 1;
        
        switch (hurricaneCategory)
        {
            case 1:
                NSLog(@"It's a category 1. You'll be fine.");
                break;
            case 2:
                NSLog(@"It's a category 2. Gettin' a little gusty.");
                break;
            case 3:
                NSLog(@"It's a category 3. Better batten down the hatches.");
                break;
            case 4:
                NSLog(@"It's a category 4. It blows. Hard.");
                break;
            case 5:
                NSLog(@"It's a category 5. Better start praying to whatever god you believe in.");
                break;
                default:
                NSLog(@"That's what you get for moving to Florida.");
                break;
        }
        
    }
    return 0;
}

[3.4] Code snippets (5:15)
--------------------------
Grab a code snippet, indent it to match the indent of your project, then add
comments to it, then select the entire snippet you just modified and save it as
your own code snippet. Time yourself and record how many seconds it takes you to
do all this.

**IT TOOK ME [56] SECONDS**

[3.5] Operators and expressions (11:08)
---------------------------------------
List the 6 types of operators described in this video. Provide their name, a
description of their meaning, and the syntax you would use to execute them. What
code snippet does the ternary operator replace?

Arithmetic Operators: Basic math functions such as addition (+), subtraction (-), multiplication (*), and division (/), along with assignment (=). 
Comparison Operators: Used to compare two values. 
- Equal (==)
- Not Equal (!=)
- Greater than (>)
- Less than (<)
- Greater than or equal to (>=)
- Less than or equal to (<=)
Logical Operators: Used to string comparisons together.
- And (&&)
- Or (||)
Modulus: Used to provide the remainder of a division.
- (%)
Increment and Decrement: Used to add or subtract one from a variable.
- Increment (++)
- Decrement (--)
Ternary: Evaluates an express as an if/then/else statement. Replaces the if/else code snippet.
- (condition) ? value if true : value if false;


[3.6] Loops (8:53)
------------------
Think of a scenario while using a mobile app that might require you to use a
"continue" statement in the middle of a loop.

When working to create a list of election years.

[3.7] Functions (10:16)
-----------------------
What is a function? What is a function prototype? What are the purposes of each?
What are the rules for when and how you can call a function?

A function is a chunk of related code wrapped up and given a name. A function prototype is a description of a function without any of the nuts and bolts. It can be used to group all of your function names together to see what is available. A function is the code that actually executes, a function prototype merely tells the compiler to expect the fuction to exist later on. 

The function must have a name, and the code it executes must be in curly brackets. You must also declare teh output data type, along with any variables passed in to the function. 


Section 4: Variables
====================
[4.1] Data types (7:06)
-----------------------
What are the primitive data types in Objective-C? Why did Apple add a set of
classes to handle other data types?

int, float, double, char, and BOOL. Apple wrote classes to handle other data types to make Objective-C easier to work with. Using a string is much easier than linking together a long list of char data types, for example. 

[4.2] Working with numbers (9:33)
---------------------------------
Make a table of Objective-C primitive data types. Add numeric data types and
their properties to this table.

type   | properties
-----------------------
int    | Holds whole numbers, takes up 4 bytes. %i
float  | Holds decimal numbers, takes up 4 bytes. %f/%e/%g
double | Holds decimal numbers, takes up 8 bytes. %f/%e/%g
char   | Holds single characters, uses single quotes, types up 1 byte. %c
BOOL   | Holds logical results YES and NO. No quotes needed. All uppercase. %i (0 or 1)


[4.3] Working with characters (4:39)
------------------------------------
Add char and BOOL (the character data types) to your table created above.

**ANSWER ABOVE!**

[4.4] Variable scope (8:06)
---------------------------
Describe in your own words what the scope of a variable is in Objective-C

Variables are local to what is contained within their statement block. Variables can go down into small statement blocks, but can't go back up into larger ones. Global variables are available for use thoughout the program, but can be hard to track where they're being used. 



[4.5] Enumerations (3:35)
-------------------------
What does the `enum` keyword allow you to do?

enum allows you to almost create your own data types in order to restrict the range of values. enum myEnumName {value1, value2, ...};

[4.6] Using typedef (2:17)
--------------------------
When would you define your own data type versus using an enum?

It's mostly used to shorten code in places where using an enum would require  more repetition or writing.

[4.7] Preprocessor directives (5:56)
------------------------------------
Describe the three common preprocessor directives, `#import`, `#define`, and
`#if DEBUG`. Come up with one example where you would use each.

Import goes and grabs other files and pastes them into the code. Define is like a find/replace. It can be used to set constants in the code. It differs from a variable in that it cannot be changed. If DEBUG will excute code before the endif if the code is being compiled in debug mode. If it is being compiled in release mode, it will ignore everything in the if DEBUG statement.

I would use import if I need to call or have access to functions in another file. I would use define to set a constant, such as the maximum amount of money someone can withdrawal from their bank account at one time. I would use if DEBUG when running in debug mode to provide me with error codes. Using if DEBUG means I don't have to strip all that code out when releasing the program to the public. 

[4.8] Working with strings (7:52)
---------------------------------
Define the same string using both NSString and C-style string syntax. Describe
the purpose behind each part of your definition.

NSString * myString = @"This is my NS String.";
string message = "This is my C string syntax."

The NSString tells the compiler to prepare for an array of characters. The * is a pointer which tells the compiler where to find the contents of the string. myString is the name of the string. The @ creates the object of the string and fills it wil the values of "This is my NS String".

In C-style syntax, the string tells the compiler that the variable 'message' is a string itself and should store the value of "This is my C string syntax."


Section 5: Classes
==================
[5.1] Introduction to object orientation (7:36)
-----------------------------------------------
Create an encapsulated (including generalized attributes and behavior)
description of a `MobileMakersParticipant` class. Instantiate a single object
representing yourself as a member of this class.

**DO YOU PROMISE YOU DID IT?**

[5.2] Using objects and pointers (6:38)
---------------------------------------
What is the pointer’s role in instantiating an object from a class? How is a
pointer different than a primitive?

The pointer serves as an address for an object. When an object is created, instead of storing the whole object in memory assigned to the object, it stores the address instead. This is in contrast to a primitive data type, where the memory assigned directly holds the value. 

[5.3] Messages and methods (6:44)
---------------------------------
What is the main difference between Objective-C’s messages and method calls in
other languages? How can this difference be seen as an advantage while
programming?

Other languages use dot syntax, whereas Objective-C uses square brackets. Additionally, when passing arguments in to a method, other languages generally use commas, whereas Objective-C uses the colon. Objective-C also breaks up the arguments and explicitly names this. This can be advantageous because, even though it results in longer code, it can be easier to read. You know what each argument corresponds to. 

[5.4] Using existing classes in the foundation framework (8:40)
---------------------------------------------------------------
What's the difference between a class method and an instance method?

A class method is designed to work on the entire class, without having to reference a specific instance of that class. An instance method will only work on one specific instance of the class. 

Try typing "NSD..." into your code window. Use the autofill feature and select a
single class name that starts with those three letters. Once the name has been
auto-completed, use the handy shortcut (Option + click) and investigate the
class whose name just got printed to the screen. Examine the task list for this
class. Do this a few more times until you're familiar with the process, or until
you've exhausted your curiosity, whichever comes last.


Section 6: Memory Management
============================
[6.1] What's new with memory management? (1:45)
-----------------------------------------------
Let it soak in. No questions for this one.

**PHEW**

[6.2] Memory management in Objective-C (6:58)
---------------------------------------------
What is the relationship between a pointer to an object, a block of memory, and
the owning and releasing process. Can you come up with an analogy for this
relationship?

A pointer is an address in the block of memory for an object. If you created an object, you should release it when you're done with it. If you didn't create it, don't release it. Once release, it can't be referenced again. 

Pointers are similar to web addresses. When browsing the web, you don't pass around entire web pages. You merely pass around the link to that web page. 

[6.3] Object creation (7:31)
----------------------------
What does the new method do when used to create an object instance of a class?
Why do we avoid using this method? How long is an object's lifetime?

It allocates an area of memory, initializes the value of that memory, and returns the memory address. Alloc init is more popular as there are many classes that have various init methods. Objects exist for the life of the program. 

[6.4] Using autorelease pools (5:14)
------------------------------------
How does the autorelease pool work? How and when can you use it deliberately?

It's full of objects that need to be released at some point in the future. The pool is drained at the end of the event loop. You can use it in methods which need to pass an object back. Releasing the object after the method returns will do no good becuase the code will never get there. Releasing it beforehand won't work because then it will be destroyed before it can be passed back. 

[6.5] Apple autoreleased objects (3:39)
---------------------------------------
What does ARC stand for? Why is it important to remember this?

New
Alloc
Retain
Copy

If you use any of these words, you own the object and have the responsilibity to release it.

[6.6] Introduction to Automatic Reference Counting (ARC) (4:43)
---------------------------------------------------------------
What does ARC save us from having to do? How does it keep us from having to make
this extra effort?

ARC saves us from having to write retain and release calls. It does this at the compiler level. The compiler scans through the program and determines where objects are and aren't being used, and auto-releases them at the optimal location.

[6.7] What ARC manages (2:42)
-----------------------------
What are the differences between ARC and garbage collection? What makes these
differences advantageous?

ARC occurs at compile time, not run time. This makes it predictable. In garbage collection, the garbage collector runs whenever things get out of hand, and can have a negative impact on program performance. With ARC, since this process occurs at compile time, it is a much more efficient way of managing memory and minimizes the impact on the program itself.

[6.8] The rules of ARC (4:20)
-----------------------------
Why can you not release or dealloc memory when working with ARC?

Because ARC manages all of the release and dealloc tasks. Manually writing them will get in its way. 


Section 7: Custom Classes
=========================
[7.1] Creating your own classes (14:01)
---------------------------------------
What are the two different sections used to create a class? What do they hold
and what files are they placed in?

The interface and the implementation. The interface is held in the .h file and shows what properties and methods are available. The implementation is held in a .m file. It is where the real code of the class lives, and actually executes what the interface says is available. 
    
**Challenge!** Create a Tweet class for a twitter style app.

Done!

[7.2] Defining methods (8:36)
-----------------------------
**Challenge!** Define what should get passed in and what should get returned by
each of your methods in your Tweet class above.

I don't really use Twitter.

[7.3] Defining properties (7:21)
--------------------------------
How did Objective-C programmers handle instance variables before 2012? How are
they handled now? What got easier and what got obscured?

They used to create a list of instance variables inside the interface .h file, usually preceeded with a leading underscore. The @property and @synthesize replaced that. It's easier because you don't have to set all of your instance variables explicitly. The variables and accessor methods are done automatically. You don't even have to add the @synthesize keyword any more. It's all done automatically. If you still want variables that are only accessible inside the class, just define them in implementation file. If you define it in the interface file, it won't be obvious that it is only accessible inside the class. 

[7.4] Defining initializers (12:30)
-----------------------------------
What are initializers and why do we need to use them? Describe a situations when
you can rely on the standard `init` method and when you have to create your own
custom initializer.

Initializers create instances of classes (objects). You can use them when you want to create an object that's already filled with a useable value. You can use a standard init when you want to create a date value of now. You can use a custom init when you want to calculate time between now and when you last used the app. 

[7.5] Using dealloc (5:33)
--------------------------
Why can we have a dealloc method in a class when using ARC, but we can't call
dealloc manually oursevles when using ARC?

ARC is what actually deallocs the object. You could write a customer dealloc method for a class, even when using ARC, to do other clean up work, such as closing open database connections, but you can't have the dealloc destroy the object explicitly, as ARC will do that. 


Section 8: Collections
======================
[8.1] Working with C-style arrays (7:12)
----------------------------------------
What are the three constraints when using C-style arrays? Create a C-style array
that holds the days of the week.

There's no bounds checking, meaning that you can call a value for a place that doesn't explicitly exist. Arrays are also fixed in size, so if you explicitly create one with five values, you can't shrink that down to four or increase it up to six. In addition, you can't mix types. You can't mix ints and strings, for example, in the same array.

NSString *daysOfWeek[7] = {@"Sunday", @"Monday", @"Tuesday", @"Wednesday", @"Thursday", @"Friday", @"Saturday"};
        NSLog(@"Today is %@",daysOfWeek[1]);

[8.2] Working with Objective-C array objects (8:00)
---------------------------------------------------
What is the difference between a mutable and an immutable array?

An immutable array is fixed in size. You cannot add or subtract objects from it. C-sytle arrays are immutable. Mutable arrays are more flexible. You can add and subtract objects from them. 

**Challenge!**
Create an immutable array containing the days of the week. Create a mutable
array that contains the days of the week that you will be at Mobile Makers. Add
the days of the week from the immutable array to the mutable array.

NSArray *daysOfWeek = [NSArray arrayWithObjects: @"Sunday", @"Monday", @"Tuesday", @"Wednesday", @"Thursday", @"Friday", @"Saturday", nil];
        NSMutableArray *mobileMakersDays = [NSMutableArray arrayWithObjects: @"Monday", @"Tuesday", @"Wednesday", @"Thursday", @"Friday", nil];
        
        [mobileMakersDays addObject:daysOfWeek[0]];
        [mobileMakersDays addObject:daysOfWeek[1]];
        [mobileMakersDays addObject:daysOfWeek[2]];
        [mobileMakersDays addObject:daysOfWeek[3]];
        [mobileMakersDays addObject:daysOfWeek[4]];
        [mobileMakersDays addObject:daysOfWeek[5]];
        [mobileMakersDays addObject:daysOfWeek[6]];
        NSLog(@"The total number of days is %lu", [mobileMakersDays count]);
          

[8.3] Using dictionaries (5:55)
-------------------------------
Create a dictionary that lists five or more events in your life and the
accompanying year (or date if you want to get fancy) of the event.

NSMutableDictionary *myLifeEvents = [NSMutableDictionary dictionaryWithObjectsAndKeys:
                                           @"6/12/1983", @"Born",
                                           @"5/30/2001", @"HS Graduation",
                                           @"6/11/2005", @"College Graduation",
                                           @"9/1/2005", @"Moved to Texas",
                                           @"7/20/2012", @"Moved to Chicago",
                                           nil];
      NSLog(@"Matt Graham moved to Texas on %@", [myLifeEvents objectForKey:@"Moved to Texas"]);

[8.4] Fast enumeration (3:27)
-----------------------------
Use fast enumeration to log the timeline of the life events you described above
to the console.

NSMutableDictionary *myLifeEvents = [NSMutableDictionary dictionaryWithObjectsAndKeys:
                                        @"6/12/1983", @"was born",
                                        @"5/30/2001", @"graduated high school",
                                        @"6/11/2005", @"graduated college",
                                        @"9/1/2005", @"moved to Texas",
                                        @"7/20/2012", @"moved to Chicago",
                                        nil];
   
   for (NSString *myEvents in myLifeEvents)
   {
       NSLog(@"Matt Graham %@ on %@",myEvents, [myLifeEvents objectForKey:myEvents]);
   }

Section 9: File Management
==========================
[9.1] Introduction to file management in Objective-C (6:44)
-----------------------------------------------------------
What can you do with files using the methods you are aware of that are available
in Objective C’s Foundation class?

Read, write, move, copy, get attributes, rename.

[9.2] Working with paths and URLs (7:17)
----------------------------------------
What are the three parts of a URL? What are the advantages to using NSURL?

Scheme, domain, and path. Scheme describes the transfer method. Domain is a high level address of the file location. Path shows where exactly the file lives within the domain. NSURL is a best practice from Apple. Using NSURL is faster, allows the user to trap errors, and is used by more classes. 

[9.3] Reading and writing strings (4:38)
----------------------------------------
What would be a reason you would want to write a string to disk instead of just
keeping it memory?

To keep the contents available even after the memory is released. 

[9.4] Archiving objects (12:41)
-------------------------------
Why would you want to archive an object instead of writing the data to disk
using the techniques discussed previously?

Archiving saves it as an object. It therefore saves all the information about the object, instead of just its raw data. 


Section 10 - More Complex Classes
=================================
[10.1] Inheritance and NSObject (8:13)
--------------------------------------
How can you determine what methods you're inheriting from a super class? How do
you overide a method inherited from a super class?

To find out what methods you're inheriting from a super class you can look at the super class' class reference. To override a method inherited from a super class, just write your own method in your own class with the same signature as the method in the super class. 

[10.2] Extending classes with categories (6:31)
-----------------------------------------------
What is the difference between a category and an inheritance? What are the
limitations of using a category?

An inheritance creates a new class that has all the same properties and methods of the existing class. However, you would have to replace the superclass in your code with the new subclass every time you wanted to use the new methods. With a category, you're just adding functionality to an already existing class, so you don't have to recode. You cannot add new instance variables when using categories. 

[10.3] Defining protocols (5:14)
--------------------------------
How are protocols useful?

They don't care what classes they're acting on. As long as the class conforms to the protocol, the protocol will perform the actions it is required to do. 

[10.4] Dynamic typing (11:33)
-----------------------------
What are the advantages and disadvantages to dynamic typing?

Dynamic typing allows you to write code when you don't know what type of class to expect. The disadvantage is, since Objective-C isn't checking the classes at compile time, it may give errors you weren't able to see in the interface. 
