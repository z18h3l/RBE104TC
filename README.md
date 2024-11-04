java c
RBE104TC C/C++ Programming Language Assignment 2
Contribution to the Overall Marks
70%
Issue Date

Submission Deadline
3rd November 2024
Assignment Overview:  This  assignment is geared towards  assessing  fundamental  coding  concepts  in  C/C++  and initiating the process of code development using the software development process (SDP) discussed in relevant lectures.
In composing the SDP report [in English], werequest you to fulfil the following criteria:
• Design: Clearly explain your understanding of the given problem and specify a sequence of steps necessary to accomplish the task (illustrated through flowcharts).
• Coding Progress: Attach 3-5 screenshots that show the code and running results as evidence, particularly highlighting any errors or situations you believe are valuable to document. The corresponding  3-5  versions  of  the  C  code  should  also  be  saved.  All  files  must  clearly demonstrate the progression of your programming task from the initial stage to the final version. (Multiple versions of C code are only required for the individual project)
• Analysis: Describe the files submitted in the Coding Progress section. Discuss the expected results, any encountered or unexpected errors, and your solutions to those issues.
• Implementation: The C code must be submitted in a separate file. Please specify the file name and provide instructions for user operation.
• Testing: Describe how you tested and validated your code for required functionalities, as well as its robustness.
Exercise 1 (30%):
Design a new class to represent a fraction (a combinationof two integer values). The data members of the class Fraction are two integers, top and down, denoting the  numerator and denominator, respectively. 
Part 1: Fundamental requirements for the class Fraction.1. Fractional numbers can be declared with both a numerator and denominator, or simple
numerator: 
2. Fractions should be able to act just like other numbers. Add, subtract, multiply, and divide;
Compare based on values; Input and output.
Part 2: Advanced requirements
3. Fractional number is normalized to ensure that only the numerator can be negative and the value is in the least common denominator form.	
• 2/-3 would be converted into -2/3 automatically;
•  15/21 would be converted into 5/7 automatically.
4. Write methods to convert between decimals and fractions.
Exercise 2 (35%):
You're now a baseball game point recorder.
Given a list of strings, each string can be one of the 4 following types:
• Integer (one round's score): Directly represents the number of points you get in this round.
•  "+" (one round's score): Represents that the points you get in this round are the sum of the last two valid round's points.
•  "D" (one round's score): Represents that the points you get in this round are the doubled data of the last valid round's points.
•  "C" (an operation, which isn't around's score): Represents the last valid round's points you get were invalid and should be removed.
Each round's operation is permanent and could have an impact on the round before and the round after.
You need to return the sum of the points you could get in all the rounds.
Note:
• The size of the input list will be between 1 and 1000.
• Every integer represented in the list will be between -30000 and 30000.
Example:
• Input: ["5","2","C","D","+"] Output: 30 Explanation:
• Round 1: You could get 5 points. The sum is: 5.
• Round 2: You could get 2 points. The sum is: 7.
•  Operation 1: The round 2's data was invalid. The sum is: 5.
• Round 3: You could get 10 points (the round 2's data has been removed). The sum is: 15.
• Round 4: You could get 5 + 10 = 15 points. The sum is: 30.
Exercise 3 (35%):
This is a Group Project!!!
You are asked to program a game called Monopoly inC++. This game is played by two players (you and computer in this assignment). The game and its rules are described as the follows.
• Account Setup:Each player must establish an account with a positive balance, starting with a deposit of 5000 units. This means that you have to set up a database (a file) which records the players ’ information, for example, name, gender and account balance etc. and the program is supposed to be able to track the balance changes as the game is going.
• Game Board:This game is played on a game board as shown in Fig. 1, consisting of 38 squares. Each square, except for the four corner squares (the "GO" square, two "CASSINO" squares, and the "JAIL" square), has a price tag for ownership, with prices randomly generated within the range of 10 to 300. All players begin at the "GO" square, and each time a player passes the "GO" square, their account balance is increased by 200 units.
• Gameplay Mechanics:You and the computer take turns to roll a dice. The outcome of each rolling (a random number within the range of 1 to 6) decideshow many squares you/computer can advance in a clockwise direction on the board. After you have landed on a square:
- if this square is unoccupied (so this means each square except  “GO ” and  “JAIL ” has an ownership attribute): you can decide whether or not you should buy it;
- if this square is occupied by you (you’ve a代 写RBE104TC C/C++ Programming Language Assignment 2C/C++
代做程序编程语言lready bought it), then nothing needs to be done;
- if this square is occupied by your opponent and the adjacent squares are unoccupied or occupied by you: you will be fined by 10% of the square price;
- if this square and one of its adjacent squares are both occupied by your opponent (which means you opponent has purchased 2 consecutives squares): you will be fined by 20% of the square price;
- The fine is topped at 20% of the square price even if more than 2 consecutive squares have been occupied by your opponent.
•  Special Squares:
Landing on the "JAIL" square requires the player to wait for one round before moving again;
Landing on a "CASSINO" square prompts the player to decide whether to gamble. If the player declines, nothing happens. If the player accepts, they must place a bet, and the casino rolls a dice. The player must predict if the outcome will be greater than 3 or not. A correct prediction results in a reward of twice the bet, while an incorrect prediction results in the loss of the bet;
•  Game End Conditions:
The game ends under three scenarios:
- A player declares bankruptcy (balance is less than or equal to 0);
- A player's account balance exceeds 15,000 units;
- The player chooses to quit the game.

Fig. 1 Game Board
Hint:
1.    The computer's logic can be straightforward. For example, it could continuously purchase squares until it runs out of funds. Additionally, when landing on  a "CASSINO" square, the computer could gamble a fixed amount,  such as  100  points, each time. Alternatively, the computer 's actions could be determined by pre-defined probabilities to introduce variability in its behavior.
2.   Employ the concept of Object-Oriented Design (OOD) to structure your game development. This involves utilizing distinct classes to encapsulate various aspects of the game. For instance, a Player class to manage player attributes and behaviors; a Map class to represent the game board and its properties, etc.
What should be submitted?    
• You should submit the followings two:
1.    A concise report (with text spanning a few pages) accompanied by C source codes. This report should delve into the specifics for each question:
- Detail  SDP steps  1  to  3 within the report  (Design +  Coding Progress  + Analysis), accounting for 30% of the evaluation.
- Encompass SDP step 4 (Implementation + Robustness) with your source code. Your code should correspond with the final screenshot provided in the Coding Progress section and include appropriate comments. Implementation contributes 35% while Robustness adds 5%.
-  Elaborate  on  SDP  step  5  (Testing),  elucidating  how  you  validated the  correctness, robustness, and thoroughness of your codes. Employ screenshots and ample explanations as verification, encompassing 20% of the evaluation.
- The overall quality of the report accounts for 10% of the evaluation.
2.    All C/C++ source code files, including files from different stages corresponding to the screenshots.
• For a comprehensive grading scheme, please consult the Marking Guidelines available on the Learning Mall system.
• The report must be saved in PDF format. Place the report in the same folder with source code files and compress the folder into a single zipped file. Your final submission should include:
- Zipped file containing:
- The report
- The source codes
• The naming convention for the submitted Report and source code files should adhere to the subsequent format:
- StudentID_LastName_FirstName_AssignmentID.pdf
- StudentID_AssignmentNumber_ExerciseID_SSScreenShotNumber.c/cpp
- StudentID_LastName_FirstName_AssignmentID.zip
What should be submitted for Group Projects?
1.    A concise report, similar to the individual project report, to demonstrate their individual work to the group project.
2.    Since different group members maybe responsible for different code components, it is not required to submit multiple versions of the code. However, all code components, including ‘ .c’, ‘ .cpp’, ‘ .h’, or ‘ .hpp ’ files created by the entire group, should be placed in a single folder for submission. The folder should be named as follows:
- StudentID_AssignmentNumber_ExerciseID
3.    An introduction file, saved in PDF format, that explains how to compile the submitted
source code. This guide will be used to compile your source code for testing, and the testing results will be used to assess the 'Implementation  Robustness' of the group project.
4.    A contribution statement signed by all group members. The format for this statement can be found in the Marking Guidelines. It looks like:

As an illustration:  
The report and C source files for individual projects, along with the folder for group projects, should be placed together in the same directory as follows:

This directory should then be compressed into a final zipped submission file, named as follows:
•  1234567_Albert_Einstein_2.zip
How the work should be submitted?  Submission should take place electronically through the Learning Mall system, enabling us to execute your software during the assessment. Additionally, feedback will be provided via the same Learning Mall system.

         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
