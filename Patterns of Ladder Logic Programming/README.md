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
IMHO, Ladder certainly has it's specific purpose.
Its simple, elegant and easy to pick up by personell with less PLC experience, so it's always a good startingpoint.

# LD Do's
Higher decisionmaking and or I/O handling i.e. reading and writing binary and or analog in/outputs.

# LD Don'ts
Looping and maths (or string) operations. These kind of “problems” can be programmed more suitable languages like Structured Text (ST).

# In general
Be aware that wrong/incorrect usage of LD will send your code down in a one way street of poor maintainability, poor readability and poor extendability. Try to compartmentalize your solutions as much as you can in small, single task oriented solutions. I.e. write your code in functions /function blocks for every piece of code that you need more then once (re-useabilty matters).


All patterns are implemented for academical and self study purpose. 
Recommended usage of IEC 61131-3 alternatives apply for specific patterns.
