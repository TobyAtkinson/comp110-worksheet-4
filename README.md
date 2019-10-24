# COMP110 Worksheet 4

##Question 1  
###a.  
A	B	C	A AND B AND NOT C  
1	1	1	0	  
0	1	1	0  
1	0	1	0  
1	1	0	1  
0	0	1	0  
0	1	0	0  
1	0	0	0	  
0	0	0	0  
  
###b.  
A	B	C	A AND NOT (B AND NOT C)  
1	1	1	1  
0	1	1	0  
1	0	1	1  
1	1	0	0  
0	0	1	0  
0	1	0	0  
1	0	0	1  
0	0	0	0  
  
###c.  
A	B	C	(A OR NOT B) AND (A OR C)  
1	1	1	1  
0	1	1	0  
1	0	1	1  
1	1	0	1	  
0	0	1	1  
0	1	0	0  
1	0	0	1  
0	0	0	0  
  
###d.  
A	B	C	D	A AND NOT (B OR NOT C) AND (NOT A AND D)  
1	1	1	1	0  
0	1	1	1	0  
1	0	1	1	0  
1	1	0	1	0  
1	1	1	0	0  
0	0	1	1	0  
1	1	0	0	0  
0	1	1	0	0  
1	0	0	1	0  
1	0	0	0	0  
0	1	0	0	0  
0	0	1	0	0  
0	0	0	1	0  
0	0	0	0	0  
0	1	0	1	0  
1	0	1	0	0  

##Question 2  
  
###a  
![Question2a](https://raw.githubusercontent.com/TobyAtkinson/comp110-worksheet-4/master/2a.PNG)  
###b  
![Question2b](2b.png)  
###c  
![Question2c](2c.png)  
###d  
![Question2d](2d.png)  
 
##Question 3  
###a.  
A	B	NOT (A OR B)	  
1	1	0  
0	1	0  
1	0	0  
0	0	1  
  
A	B	NOT A AND NOT B  
1	1	0  
0	1	0  
1	0	0  
0	0	1  
  
###b.  
A	B	NOT (A AND B)	  
1	1	0  
0	1	1  
1	0	1  
0	0	1  
  
A	B	NOT A OR NOT B  
1	1	0  
0	1	1  
1	0	1  
0	0	1  
  
###c.  
A	B	C	(A AND B) OR (A AND C)  
1	1	1	1  
0	1	1	0  
1	0	1	1  
1	1	0	1  
1	0	0	0  
0	1	0	0  
0	0	1	0  
0	0	0	0	  
  
A	B	C	A AND (B OR C)  
1	1	1	1  
0	1	1	0  
1	0	1	1  
1	1	0	1  
1	0	0	0  
0	1	0	0  
0	0	1	0  
0	0	0	0	  
  
###d.  
A	B	C	(A OR B) AND (A OR C)  
1	1	1	1  
0	1	1	1  
1	0	1	1  
1	1	0	1  
1	0	0	1  
0	1	0	0  
0	0	1	0  
0	0	0	0  
  
A	B	C	A OR (B AND C)  
1	1	1	1  
0	1	1	1  
1	0	1	1  
1	1	0	1  
1	0	0	1  
0	1	0	0  
0	0	1	0  
0	0	0	0  
  
##Question 4  
###a.  
The first program and the second program are the same as the first program   
is using an AND logic gate to check if both files  
are there, but as it is in the NOT bracket it reverses it to trigger the   
print if both files aren't there. On the other hand, the second program does the same but  
does it by just using a NOT and OR logic gates to check if either file  
is missing.  
  
We can use the truth table above from question 3 b. to see that NOT (A AND B), which  
is what the first program does, is the same as NOT A OR NOT B, which is what the   
second program is doing.  
  
###b.  
Both programs are equivalent again,  as the first program uses an OR logic gate  
to check if the variable x is an integer or float and then uses an AND logic gate  
to check if the variable is greater than 7 both times. Whereas the second program uses an OR  
logic gate to first check the type of variable x is before then checking if it  
is greater than 7 no matter what variable it is.  
  
We can use the truth table above from question 3 c. to explain this.  
If we replaced the A as x being greater than 7, as well as replacing  
B and C for x being either an integer or float we can see that the first program  
uses the same logic as (A AND B) OR (A AND C), whereas the second program  
uses the same logic as A AND (B OR C) which outputs the same results.  
  
###c.  
For this question we can use once again use truth tables to explain why both programs  
are equivalent. In the first program it is the same  
as A AND B, we can create the truth table here to show what that results in.  
  
A	B	Result  
1	1	1  
1	0	0  
0	1	0  
0	0	0  
  
Now looking at the second program we can see that it uses the logic of  
NOT(A OR B) which results in the truth table below.  
  
A	B	Result  
1	1	0  
1	0	0  
0	1	0  
0	0	1  
  
These truth tables show that both programs are equivalent where both A and B have to  
match for the output to line up, but they are just swapped as program one only outputs true  
if both are set to 1, or true, and the second program only outputs true if both are set to 0,  
or false.  
  
###d.  
We can make another truth table to show how program 1 and 2 are equivalent this time   
with A, B and C. A represents if x > 10, B represents if x > 0 and C represents if y > 0.  
Program 1 represented in a truth table is.  
(if A is true then B will always be true as x > 10 being true means X > 0.)  
A	B	C	Result  
1	1	1	1  
1	1	0	1  
0	1	1	1  
0	1	0	0  
0	0	1	0  
0	0	0	0	  
  
Here is the truth table for the second program.  
  
A	B	C	Result  
1	1	1	1  
1	1	0	1  
0	1	1	1  
0	1	0	0  
0	0	1	0  
0	0	0	0	  
  
Although the programs are written differently using the logic gate truth  
table we can see all possible outcomes are the same with both programs  
no matter the values of x and y.  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
