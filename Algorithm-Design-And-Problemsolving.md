# Program Development Life Cycle
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

#Common Algorithms
- A search algorithm is a set of data used t identify whether a specific vlaue of data exists or not. Example : 
	- Linear search
- A sorting algorithm takes a set of data and rearranges it to be in a specific order (ascending to descending, A to Z). Example:
	- Bubble sort

## Linear Search
- Linear search checks for an item one at a time, starting with the first item and continuing until the last value.
- Example:
	- Search this set of data for the number 4.
| 5   | 3   | 9   | 4   | 2   | 1   | 8   |
	| --- | --- | --- | --- | --- | --- | --- |


1. Compare if the first value(5) matches the search value(4). It does not. 
2. Compare if the second value(3) matches the search value(4). It does not. 
3. Compare if the third value(9) matches the search value(4). It does not. 
4. Compare if the fourth value(4) matches the search value(4). It does. It has been found.

## Bubble Sort
- This is used to sort data on a specific order. 
	- Bubble sort takes the first 2 values, 1 & 2 and compares thwm. 
	- If they are the wrong way around, it'll swap them. 
	- It continues and takes the next two values, 2 & 3 and compared them. 
	- If they are the wrong way around it swaps them. 
	- This process is repeated until it has worked through all the items on the list once. 
	- It then starts again from the first two values.


