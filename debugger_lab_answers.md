## Debugger Lab Answers
###Date:1/29/15
Concepcion Sosa

**Question 1:**
The reason why `cutoff` is not a parameter to the method `playTurn` in the `PigGame` class is because `cutoff` is the constructor.

**Question 2:** 
The following code would print out 0.0.

**Question 3:** 
This statement can be moved to the playTurn method. In the playTurn method, the statement would go within the` if` statement that is within the `while` statement. 

**Question 4:**
Based on my current understanding, I think that the problem(s) might be located in the Die class. i think everything else should be normal and run properly. 

**Question 5:**
The problem was within the Die class. Under the `public void roll()`, the upValue was `((int)Math.random()*6)+1` which was causing a problem.  It would change the number into an integer. However, using the random function, the number it gives us is between 0 & 1. So changing that decimal into an integer would not be helpful because it rounds down. (Random function gives me .09, changes it into an integer which would be 0 +1, which would always be 1.) Solution, I decided to re-write it as `(int)((Math.random() * 6) + 1)`, which allows the math random function to be multiplied by 6 and added together with 1, which then finally gets changed into an integer. 

**Question 6:**
For the number 10: 100, 14, ~7.1425.
For the number 15: 104, 15, ~6.933334. For the number 20: 103, 12, ~8.583334. For the number 25: 101, 9, ~11.22221.
