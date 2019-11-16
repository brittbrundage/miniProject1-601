**1.	How python uses the Indentation to control Flow**
<br>

Python uses indentation to the control the flow of code. Each block contains a group of code to be run together. Once a 
separate indentation is made, python will read it as a separate group of code. 
Note that the block must all contain the same amount of indentations to be read together.
<br>

Example layout:

![Blocks](/images/blocks.png)

**2.	Don’t repeat yourself**
The Don’t repeat yourself (DRY) principle in python is necessary in avoiding unnecessary repetition with the code. 
It allows for the code to have a better flow and be easier to read. Another benefit is that if the code needs to be update, 
it will help in reducing additional work needed. 

Example: 
Rather than listing the following separately it could be combined into one listing. 
Original
print(test1)
print(test2)
print(test3)
	DRY Applied
	print(test1,test2,test3)
