# Create a pipeline that takes an action only if a condition is met
1.	Click on pipelines
2.	Click on plus sign
3.	Click on add stage 
4.	Select type Wait
5.	Stage Name Deploy Oregon
 
6.	Set Wait time to 2 seconds
7.	Check Conditional on Expression
8.	Set expression equal to ${ 'parameters.REGION' } == 'Oregon'
9.	Click on Configuration stage
10.	Click on add a stage
11.	Stage Name Deploy Virginia
12.	Set Wait time 2 seconds
13.	Check Conditional on Expression
14.	Set expression equal to ${ 'parameters.REGION' } == 'Virginia'
 
1.	Click Save in bottom right hand corner
2.	Run Pipeline – Notice the execution now prompts you for a region to choose
