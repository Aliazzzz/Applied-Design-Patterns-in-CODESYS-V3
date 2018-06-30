The 'Patterns of Ladder Logic' in CODESYS 3

# Remember kids!
Never write complex software solutions in Ladder! 
IMHO, some of the patterns shown in the example are pretty "complex" allready.

Ladder certainly has it's specific purposes, its simple and easy to pick up by personell with less PLC experience, so its a good start.
The drawback however is that ladder cannot compete with a higher abstraction language like ST. Even experienced programmers can encounter trouble in trying to understand the complexity of a patchwork in rungs. Wrong/incorrect usage of ladder will send your code down in a one way street of poor maintainability, poor readability and poor extendability. So, use with caution.

Typical usecases for implementation in Ladder cover mostly Simple decisionmaking or I/O handling i.e. reading and writing binary and or analog in/outputs. 


Original Poster: Scott Whitlock

http://www.contactandcoil.com/patterns-of-ladder-logic-programming/

If you’re familiar with PC programming in languages like Java or C#, then you’ll probably know about the books Design Patterns: Elements of Reusable Object-Oriented Software and Patterns of Enterprise Application Architecture. These books are about Software Design Patterns.

This list of ladder logic programming patterns serves two purposes: 

* First, each pattern is a tool for solving a common problem using ladder logic, and having these patterns in your toolbox will allow you to program faster and spend more time focusing on the higher level structure of your program. 

* Second, since these are common patterns, you’ll start to find it easier to read other people’s ladder logic, and other experienced programmers will find it easier to follow your logic.

        The Sealed in Coil pattern
        The State Coil/Fault Coil pattern
        The Start/Stop Circuit pattern
        The Set/Reset pattern
        The Flasher pattern
        The Debounce pattern
        The Input Map pattern
        The Step pattern
        The Mission pattern
        The Five Rung pattern
        The Mode pattern
     
