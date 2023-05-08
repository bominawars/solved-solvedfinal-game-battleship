Download Link: https://assignmentchef.com/product/solved-solvedfinal-game-battleship
<br>
BACKGROUND

The game Battleship was produced as a board game in 1967 by Miltonn Bradley and has sold over 100 million copies, according to Wikia. For this final alternate project, you must write Battleship.

For the purpose of this game, there are two players: player[0] which represents the computer’s playing board and player[1] which represents the human’s.

WHAT YOU ARE GIVEN

1. You get to play the game at http://kortaggio.github.io/battleboat/. There is no code in this website.

2. You are given the following files (in CISP401V9AlternateFinal.zip), which you can use for this program.

a. Main.java (used for setting up the display)

b. Point.java (has x, y coordinates)

c. Ship.java (has a name, length, etc., and it’s not good if your Ships get hit during the game)

d. Grid.java (knows how to place ships and keep track of them; also keeps track of where it has been fired upon)

e. Player.java (has a Grid field; could be improved to include scoring and other things that are independent of a grid)

f. Display.java (handles mouse events, display code, etc.; this could be where most of the code will go)

g. Utilities.java (contains method between(); if you feel the need to add general purpose helper functions, this is a good place for them)

OBJECTIVE

You are to write the game Battleship application for two players at one computer. It should behave pretty much like what you see at the http://kortaggio.github.io/battleboat/ web site except that it will be in a Java application. The human player will set ships manually by clicking on squares on the grid. The computer will set its ships randomly. The human will fire on the computer ships by clicking on the grid. The computer will fire at human ships randomly until it hits a ship, at which it will focus on that ship until it is killed. (You will need to think about how that works when more than one ship is hit in a sequence of attacks.)

There are several guide lines for this project:

1. Randomize placement of the computer ships in the initComputerShips() method. (The code you received places the ships in fixed locations; that makes for a horribly boring game.) Ships need to be placed legally.

2. Play a game. The human always gets to go first.

a. Until someone has destroyed all of the opponent’s ships, do:

i. Human fires on computer by clicking on computer grid; there is a fireOnComputer() method in the Display class that is empty that you must fill in.

ii. Computer fires on human; there is a fireOnHuman() method in the Display class that you must fill in.

1. fireOnHuman() results in the Human grid being attacked.

2. The computer should have a strategy that minimizes the number of attack attempts. The quality of the strategy and whether it works is what matters.

b. This needs to be initiated in the mouseReleased() method.

3. You are not allowed to change any existing methods no matter how horribly written you might think they are unless given permission to do so. Those methods are to be treated as library routines. The methods you can change (and must change) are:

a. initComputerShips()in the Display class

b. fireOnComputer() in the Display class

c. fireOnHuman() in the Display class (You may wish to consider adding parameters, too.)

d. mouseReleased() in the Display class (In case you want to send arguments to fireOnHuman()…)

e. paint() so you can show when the game is over

4. You can decide whether to create a Computer class that extends Player and contains the strategy for the computer (which makes the most sense object-wise) or just to write that code as additional methods in the Display class. I personally think that it will be easier to think about this problem in an object-oriented manner, meaning that I would create a Computer class, but whatever works for you is fine.

5. You may write whatever helper methods you want.

The game Battleship project will be graded generally on the following criteria:

1. A proper runnable program with all the expecting results(600 points):

1. Are the computer’s ships randomly placed?

2. Can you click on the computer’s board to attack?

3. Can the computer attack your board?

4. Once the computer has hit a ship, does it continue to try to find that ship until it is destroyed?

5. If none of the human’s unsunk ships has been hit, can the computer use a good strategy to form attacks?

6. Can you detect when the game ends?

2. Proper documentation(400 points) and place all the program files in When you are ready to submit, please zip all your files into a proper named (If your name is Charles Janewell, the file name for spring 2016 final program should be JanewellCAltFPCISP40116S.) zip file.