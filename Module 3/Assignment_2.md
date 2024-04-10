## Assignment 2
Sudoku is a mathematical puzzle game. In Sudoku, we have a 9x9 grid with numbers (from 1 to 9). Additionally, this grid is divided into 9 3x3 small grids. The initial grid is filled in with some numbers, and the final solution is a grid full of numbers. See figure 1 as an example. You have the following restrictions:
- A number will appear once in each column.
- A number will appear once in each row.
- A number will appear once in each 3x3 small grid


<img src="https://github.com/johanhjorth/DVA264/blob/main/assets/sudoku.png?raw=true" alt="Sudoku Puzzle" style="height: 250px; width:553px;"/>

**Figure 1**: (left) Initial grid. (right) Solution of the Sudoku.

The different Sudokus are given in the file “assignment 2 sudoku.txt”. The Sudoku from the picture would be given in the file with the following format:

SUDOKU N

530070000

600195000

098000060

.....

000080079

The empty positions are represented with zeros in the file.

**What to do:** Your assignment now is to apply Backtracking to search for a solution of the 10 Sudoku. You need to present the code to the teacher. **(2 Points)**

### Your report has to cover the key parts as follows:
1. Explanation of the problem. **(3 points)**
    1. Give the representation of a solution (answer) of the problem, as explained during the course. **(1)**
    2. Give the equation for the restriction(s) of the problem. **(0.5)**
    3. What is consider as a state? In addition, explain why. **(0.5)**
    4. Which is the initial state? In addition, explain why. **(0.25)**
    5. Which is/are the possible action(s)? In addition, explain why. **(0.25)**
    6. What is the maximum branching factor of the tree (b)? In addition, explain why. **(0.25)**
    7. What is the maximum depth of the search tree (m)? In addition, explain why. **(0.25)**
### Pre-conditions in order to present your code:
- The code should run under 1 second. If you cannot get it faster, talk to the teacher. The reason could be your computer.

### Conditions to approve the assignment 2
In order to receive the points for the code, you need to submit the report and have more than half of the points. Example: If a report have 1 point, then you need to have a minimum of 0.5.
- Minimum score to pass assignment 2: 3 points.

**SCORES 3-5**
- Your score < 3: U
- 3 <= your score <= 3.75: 3
- 3.75 < your score < 4.75: 4
- 4.75 <= your score: 5

**SCORES A-F**
- Your score < 3: F
- 3 <= your score < 3.4: E
- 3.4 <= your score < 3.8: D
- 3.8 <= your score < 4.2: C
- 4.2 <= your score < 4.6: B
- 4.6 <= your score: A

SUBMISSION DETAILS

Maximum Score: 5 points.
Time to submit: 4 April – 4 June & 27 June & 14 August

I will not consider a submission without the following format:

File names for the submission:

StudentName_StudentLastName_Assignment2_Code.zip (Only by email)

StudentName_StudentLastName_Assignment2_Report.pdf (Only in canvas)


Email subject for the submission:

[DVA251] StudentName StudentLastName Assignment2 Code

### ADDITIONAL INFORMATION!
You are allowed to send each assignment a maximum of three times. When you approve the
assignment, you are not allowed to submit the assignment again.

Before defending the code to Miguel Leon, you have to send the code by email to johan.hjorth@mdu.se or jonatan.tidare@mdu.se.

Before submitting the report, you should present this assignment first to a lab assistant. After that, and only if everything is correct, you are able to submit the report in canvas.

You cannot get the points of the report without presenting the code first.
