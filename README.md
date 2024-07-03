# PYTHON_RPS_Game
# HW5: Rock, Paper, Scissors

---

### Policy of Due Dates

If you need additional time to complete this assignment, please contact me before the due date. **No excuses or extensions will be accepted after the due date.** You are allowed up to two extensions: the first extension grants an additional two days, and the second extension grants one extra day. After these two extensions, no further extensions will be permitted, and you must submit whatever work you have completed.

---

### Grading Policy for Uncovered Topics

Avoid incorporating advanced topics or functions that haven't been covered in our studies. The use of uncovered/unfamiliar topics or functions like ChatGPT answers may result in a deduction of points.

---

**You are to write a program where the user plays Rock, Paper, Scissors against the computer. To play this game, each player chooses one of three options: Rock, Paper, or Scissors. The winner is determined based on the following rule:**

- Rock vs Scissors : Rock wins (Rock smashes Scissors)
- Scissors vs Paper : Scissors win (Scissors cut Paper)
- Paper vs Rock : Paper wins (Paper covers Rock)

---

## Objectives

- Designing a solution with selection structures
- Continued practice with functions
- Work with random numbers

---

## **User Interface Specifications**

### INPUT

After displaying a user introduction,

- The program prompts the user for their choice (rock, paper, or scissors). Instruct the user to enter just the first letter: **r**, **p**, or **s**. Accept either a lower or upper case letter. < Or 0 for rock, 1 for paper, and 2 for scissor with menu driven program.>

### OUTPUT

The program then outputs

- The user's choice, as a complete word (rock, paper, or scissors).
- The computer's choice, as a complete word (rock, paper, or scissors).
- The winner. The game is a draw, no winner, if both choices are the same.

---

## **Code Specifications**

- If the user does not enter a valid option of **r**, **p**, or **s**, (lower or upper case), the program should display a helpful error message and then terminate (in other words, don't execute the rest of the program). Please see how this occurs in the tip calculator example this week. Do not use sys.exit() or any other built-in function to terminate the program. The program should end when main() ends. Any function ends either when it reaches the end of its block or it returns.
- You will need to use the random module to generate the computer's selection. You will find [documentation for that module here](https://docs.python.org/3/library/random.html?highlight=random#module-random) There are several approaches you can take. One would be to generate a random integer, such as 1, 2, or 3, using the randint() method. Then you would have to implement code to translate the numeric value to a game option (rock, paper, scissors). Alternately, you can try using the choice() method (though this uses sequences, which you'd have to investigate on your own).
- You must come up with a design that **uses decomposition**. You must make at least 4 functions.
    1. “***compChoice***” function : You should have a function that creates the random choice (string or character) to the game option. 
    2. “***userChoice***” function : You should write a function that is passed in the user's choice by your menu and returns the complete string (or integer number by your design) for that choice, "Rock", "Paper", or "Scissors". The return value should be used in the ***game*** function (i) to decide who win and (ii) to display what the user chose. 
    3. “***game***” function : You should have a function that implements the rules of the game: pass in the 2 choices (user and computer) and return the winner. 
    4. “***main***” function : Don't forget your main() function to call other functions. 

NOTE ****: Your solution is limited to the topics covered so far this quarter: chapters 1, 2, 3, and 5.  **Do not use any type of repetition or data structure.**

---

## Documentation and Other Style Issues

You should follow the course Documentation and Style Guidelines, including

- program description at the top of the file
- descriptive **variable** and **function names**
- comments at the top of each function definition, as well as algorithm comments inside.

---

## **Testing**

Test your program to make sure everything works.  This includes testing that invalid input is handled correctly.

Though it may not make sense to have test cases in a program with random data, make sure to include the rules of the game somewhere in the documentation.

---

## **Written Report**

Please type up the answers to the following questions and include as a comment at the bottom of your .py file:

1. How did you approach this assignment? Where did you get stuck, if at all, and how did you get unstuck?
2. How did you test your program? What doesn't work the way you might like, such as features you'd like to add once you know more?
3. What did you learn from this assignment? What would you do differently next time?

---

## **Grading**

The following table shows the rubric of grading HW 5. 

| Criteria | Rating | Points |
| --- | --- | --- |
| Program runs correctly.
 | Issue from function/playing-game  : 3 pt / issue

1. Make 4 Functions 
2. Correct parameters/return values
3. Use of if statement
4. Boolean (Conditional) Expression | 12pts |
| Control structure
 | Completed control structure - Use of if statement

1. if statement format
2. Boolean (Conditional) Expression
3. Consider possible cases | 4pts |
| Documentation | 2pt : Completed
1pt : Basic comments
0pt : No comments on your program | 2pts |
| Written report | 2pt : Completed
1pt : At least, 1~2 sentences
0pt : No written report | 2pts |
|  |  | 20pt |
