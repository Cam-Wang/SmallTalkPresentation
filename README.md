# Smalltalk
## History
- Smalltalk was developed at Xerox Palo Alto Research center in 1980, and is actually Smalltalk-80, although there are many variants of the language
- Earlier versions were passed around for peer review to Hewlett Packard, Apple, UC Berkeley among others
- Squeak is an implementation of Smalltalk-80 that’s open source, VisualWorks is another
- Two CA based organizations, ParcPlace Systems and Digitalk sold Smalltalk environments and support during the end of the 1980s to the middle of the 1990s
- ParcPlace gave support for Unix systems and Digitalk focused on Microsoft Windows computers
- Originally, Smalltalk was expensive, needed a lot of memory, and was only available to sizeable organizations, although Sigitalk tried to reduce the pride to sell more
- In 1995, the two competing companies became ParcPlace-Digitalk and later in 1997 became ObjectShare it didn’t last past the millenium 
Squeak has the most active community around it, since it is open source
## Tasks Small Talk is suitable for
- Smalltalk was designed to be easy to use by not only computer scientists, but also by people without an extensive technology background
- Messaging is the central idea of Smalltalk-good for programs that require a lot of communication between objects
- Primitive types are also used as objects, a class derived from a primitive type can extend it's functionality
## Why consider Small Talk?
- The language can do the same amount of work as other languages, while using about a third of the code
- With less code to write, test, and maintain, there is a lower cost to develop, along with the fact that is closer to spoken sentences than dense than other low level languages, means more, less trained people can understand it
- Many modern languages are derived or their design was influenced by SmallTalk including Java,PHP,Python,Ruby
## Syntax of Small Talk
- **Characters** are reprsented with a '$' before them such as `$A`
- **String** are represented with single quotes such as `'foo bar'`
- **Symbols** are indicated by `#`
- **Arrays** can be declared with '()' or '[]' 
  - '()' declares a typed array for example an int array would be declared as `#(1 2 3 4)`
  - '[]' declares a byte array such as `#[1 2 3 4]`
- **Variables** are declared by '| |' and are asssigned with ':='
  - `| var |`
  - ` var := 'foobar'`
- **Messages** are the most important aspect of coding in Small Talk where every object to even control structures use messages
  - Messages have two aspects the receiver and selector
  - In the following code 'var' is the reciever and 'func' is the selector
  - `var func`
  - You can pass arguements for the selector by using assignment such as passing `$A` into a selector that finds the index of a     char
  - `Answer indexOf: $A`
  - This is helpful for making code less ambigious such as the constructor `Circle(radius,center)` in other languages would be written as `Circle(5,10)` where as in Small Talk you would write it as `Circle radius: 5 center: 10`
 - **Expressions** build upon messages and allows the inclusion of multiple messages in a single line
  - For example the line `1 plusOne + 3 plusOne inRange: 5 and: 10` reads as 3 seperate messages and runs as follows
    - First 1 receives the message `plusOne` and returns 2
    - 3 receives the message `plusOne` and returns 4
    - 2 recieves `+` 4 and returns 6
    - 6 recieves `inRange: 5` `and: 10` and will return `true`
  - Expressions are proccessed from left to right and no message holds precedence over others
 
 

