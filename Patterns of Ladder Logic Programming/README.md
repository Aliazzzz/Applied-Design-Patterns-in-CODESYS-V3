The 'Patterns of Ladder Logic' translated to CODESYS 3 LD Function Blocks

Original Poster: Scott Whitlock

http://www.contactandcoil.com/patterns-of-ladder-logic-programming/

If you’re familiar with PC programming in languages like Java or C#, then you’ll probably know about the books Design Patterns: Elements of Reusable Object-Oriented Software and Patterns of Enterprise Application Architecture. These books are about Software Design Patterns.

This list of ladder logic programming patterns serves two purposes: 

* First, each pattern is a tool for solving a common problem using ladder logic, and having these patterns in your toolbox will allow you to program faster and spend more time focusing on the higher level structure of your program. 

* Second, since these are common patterns, you’ll start to find it easier to read other people’s ladder logic, and other experienced programmers will find it easier to follow your logic.

        The Sealed in Coil pattern              
        The State Coil/Fault Coil pattern               
        The Start/Stop Circuit pattern                          
        The Set/Reset pattern                   * Recommend use of SR / RS from standard.library instead
        The Flasher pattern                     * Recommend use of BLINK from util.library instead
        The Debounce pattern
        The Input Map pattern                   * Pattern obselete in CODESYS V3 due to IO Mapping features
        The Step pattern
        The Mission pattern
        The Five Rung pattern
        The Mode pattern


# Simple, elegant and easy to pick up!
IMHO, Ladder (LD) certainly has it's specific purpose. It's visual, simple, elegant and easy to pick up by personell with less PLC experience. It is always a good startingpoint. 
Just do not try to use LD language for tasks it isn't intended for. So, over time, when programming experience and confidence grows, the programmer will inevitably outgrow LD and is able to see LD's limitations. This does not mean that LD itself is limited as by nature LD it is visual, simple and elegant. Thus the circle is complete. 

# LD Do's!
Higher decisionmaking (Boolean operations) or I/O handling i.e. reading and writing binary and or analog in/outputs.

# LD Don'ts!
Looping (FOR TO DO, WHILE) math / calculations or string operations. 
These kind of “problems” could be programmed more a suitable language: Structured Text (ST).

# In general
Be aware that wrong/incorrect usage of LD will send your code down in a one way street of poor maintainability, poor readability and poor extendability. 

Try to compartmentalize your solutions as much as you can in small, single task oriented solutions. I.e. write your code in functions and/or function blocks for every piece of code that you need more then once (re-useabilty matters).

Neither CFC or FBD languages are capable of programming FOR TO DO or WHILE decision loops well. However, math and string operations can be programmed in CFC or FBD. This said, solving math and string operations and doing loops in ST takes (almost) no effort. So, in general it's easier to tackle all problems in ST, but takes some programming experience. Ultimatly, if you wish to solve your problems in another language like CFC, LD, FBD, IL you are free to do so. Just be aware of the language specific limitations.


All patterns are implemented for academical and self study purpose. 
Recommended usage of IEC 61131-3 alternatives apply for specific design-patterns.
