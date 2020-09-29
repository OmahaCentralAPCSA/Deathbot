# :robot: Deathbot
generate a set of commands for the pleasantbot to obliterate the deathbot.  

Quick, enter the location of the evil deathbot.  Our software will then generate the best set of commands for our own pleasantbot that will allow it to obliterate the deathbot.

Your job is to provide the program that will read the coordinates of the deathbot and then output the appropriate commands.  Our pleasantbot understands only these commands:  
•	TL	pivot 90 degrees to the left
•	MV  move one robounit forward
•	SH  shoot, obliterating anything directly in front of us

We want the shortest list of commands so we can eliminate the evil deathbot before it can move or do something dastardly. If there is more than one shortest list don't quibble: any shortest list that will rid the world of the deathbot is fine. Warning: if you move onto the spot where the deathbot is, your pleasantbot will be destroyed. :boom:

## Input
Create a method called `pleasantBot` that takes in 2 integers and a letter.  

The two integers represent the Eastward :arrow_right: and Northward :arrow_up: distances (robounits) from our pleasantbot to the deathbot.  They are between -10 and + 10 and will not be 0.  A negative distance eastward represents westward :arrow_left: and a negative distance northward represents a southward :arrow_down: distance.  

The letter is E, N, W or S, indicating the initial direction that the pleasantbot is facing.  

## Output 
Output the commands in order on the same line. 

## Examples 

```
pleasantBot(-10, 0, W) should output: SH
```
We (the pleasantBot) are facing West and the deathbot is 10 units ahead of us.  Since we are already facing West, we shoot.  

```
pleasantBot(10, 0, N) should output: TL TL TL SH
```
We are facing north, so at (10, 0), the deathbot is directly to our right, so we turn left 3 times and then shoot.

```
pleasantBot(3, 7, W) should output: TL TL MV MV MV TL SH
```
We are facing west and the deathbot is east by 3 and north by 7 robounits.  Thus, it is better to turn east and then move 3 units, then face north and shoot.  

```
pleasantBot(-5, -3, E) should output: TL TL TL MV MV MV TL TL TL SH
```
We are facing east and the deatbot is west by 5 and south by 3.  Thus we want to turn south, move 3 units and then turn west and shoot. 
