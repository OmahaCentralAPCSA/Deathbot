# :robot: Deathbot
generate a set of commands for the pleasantbot to obliterate the deathbot.  

Quick, enter the location of the evil deathbot.  Our software will then generate the best set of commands for our own pleasantbot that will allow it to obliterate the deathbot.

Your job is to provide the program that will read the coordinates of the deathbot and then output the appropriate commands.  Our pleasantbot understands only these commands:  
•	TL	pivot 90 degrees to the left
•	MV  move one robounit forward
•	SH  shoot, obliterating anything directly in front of us

We want the shortest list of commands so we can eliminate the evil deathbot before it can move or do something dastardly. If there is more than one shortest list don't quibble: any shortest list that will rid the world of the deathbot is fine. Warning: if you move onto the spot where the deathbot is, your pleasantbot will be destroyed. :boom:

## Input
Create a method called `pbotCommands` that takes in 2 integers and a letter.  

The two integers represent the Eastward :arrow_right: and Northward :arrow_up: distances (robounits) from our pleasantbot to the deathbot.  They are between -10 and + 10 and will not be 0.  A negative distance eastward represents westward :arrow_left: and a negative distance northward represents a southward :arrow_down: distance.  

The letter is E, N, W or S, indicating the initial direction that the pleasantbot is facing.  

## Output 
Output the commands in order on the same line. 

## Examples 

```
pbotCommands(-10, 0, W) should output:

pbotCommands(10, 0, N) should output: 

pbotCommands(3, 7, W) should output:

pbotCommands(-5, -3, E) should output: 
```
