## Program Development Life Cycle
- These stages include: ANALYSIS, DESIGN, CODING and TESTING

### Analysis
- This stage involves looking at the problem and the system that it needed. Decomposition is used to split the problem into subproblems. Subproblems allow the developer to identitfy the requirements for each component part and tackle them sepertely. 
- Subproblems can be made as a subprogram.

### Design
- This where how the program works will be planned.
- This can include:
	1. An overview of the program using a structure diagram
	2. Designing the algorithm using flowcharts and pseudocode

#### Structure Diagrams
- This is a hierarchal diagram that shows the decomposition of a system.
- Examples

##### Calculator

| Calculator  | Input                                        | Process                | Output |
| ----------  | -------------------------------------------- | ---------------------- | ------ |
|             | Input number1 + Input symbol + Input number2 |        Number1 Symbol Number2                |   Output answer      |
- Tip :  Split it to the smallest instruction.

##### Chess

| Chess | New Players                   | New Game                           | Make move                                                                       | Check won                                             |
| ----- | ----------------------------- | ---------------------------------- | ------------------------------------------------------------------------------- | ----------------------------------------------------- |
| ---   | Input Player1 + Input Player2 | Assign Colours + Display New Board | Output player's turn + Input piece + Input move + CHeck move valid + Move piece | Check player move check + Check player move checkmate |

- These algorithms should come together to make a whole system.

#### Quiz (page 149)
1. This is the process of making smaller subprograms from a program. These subprograms can be made even smaller.

#### Flowcharts
- This is a diagrammatic representation of an algorithm.
- It shows each step of a  process in the order they are meant to be performed in.
![[Pasted image 20230328003257.png]]

- The statements inside flowcharts can be written as pseudocode or simply just words.

#### Pseudocode
- Refers to code that is not written on a computer to run. 
- How to write good pseudocode:
	- Capitalise commands e.g IF , THEN , INPUT , OUTPUT , FOR
	- Write **one** statement **per** line
	- Use indentation
	- Be specific
	- Keep it simple
- Pseudocode can be written similar to a programming language.

### Coding
- Once you've decomposed your problem into subproblems, designed the algorithms using flowcharts and peusocode, you may write the code. 
- Make sure you test it on each step before moving on.

### Testing
- You need to make sure your code:
	- Fully works
	- Does not crash
	- Meets all requirements
- There are 4 kinds of data tests used to test a program (example is a program that needs a user to input a password that has 8 characters):
	1. Normal - Data that the program should accept e.g "abcdefgh" , "0hduPeljf$hu0"
	2. Abnormal - Data that the program shouldn't accept e.g "1234567" , "seven"
	3. Extreme - Data that is at the edge of what is allowed e.g "12345678" , "wEg6!dh0"
	4. Boundary - Data that is on the edge of being accepted and being rejected (either side of the limits) e.g "12345678" , "1234567"
