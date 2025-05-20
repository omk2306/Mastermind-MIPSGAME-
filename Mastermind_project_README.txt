# Mastermind Game in MIPS Assembly

## Overview
This is an implementation of the classic Mastermind game in MIPS Assembly language, designed to run on the MARS (MIPS Assembler and Runtime Simulator) environment. The game features a colorful ASCII interface, custom graphics, and all the gameplay elements of the traditional Mastermind board game.

## Game Description
Mastermind is a code-breaking game for two players. One player becomes the codemaker, the other the codebreaker. The codemaker creates a secret pattern of four color pegs, and the codebreaker tries to guess the pattern within a certain number of attempts. Each guess is made by placing four color pegs on the board. The codemaker provides feedback by indicating:
- How many pegs are the correct color and in the correct position
- How many pegs are the correct color but in the wrong position

## Features
- Customizable number of guess attempts
- Player name input for codemaker and codebreaker
- ASCII art graphics for game logo, win/lose screens, and trophy
- Color visualization using ASCII characters
- Detailed feedback for each guess
- Position-specific feedback for correct guesses

## How to Play
1. Enter names for the codemaker and codebreaker
2. Specify the maximum number of allowed guesses
3. Codemaker enters a secret 4-color code (not visible to codebreaker)
4. Codebreaker makes guesses until they either:
   - Correctly guess the code (win)
   - Run out of guesses (lose)

## Controls
- Input is via keyboard
- The game uses the following color codes:
  - `r` = Red [R]
  - `g` = Green [G]
  - `b` = Blue [B]
  - `y` = Yellow [Y]
  - `p` = Purple [P]
  - `c` = Cyan [C]

## Technical Details
- Written in MIPS assembly language
- Designed for the MARS simulator
- Makes use of system calls for input/output operations
- Implements arrays and string manipulation
- Uses memory management for game state

## Running the Game
1. Download and install the MARS simulator from [Missouri State University](http://courses.missouristate.edu/kenvollmar/mars/)
2. Open the Mastermind game file (`mastermind_enhanced.asm`) in MARS
3. Assemble the program (F3 or "Run" -> "Assemble")
4. Run the program (F5 or "Run" -> "Go")

## Game Algorithm
The game implements the classic Mastermind algorithm for determining:
1. Position matches (right color in right position)
2. Color matches (right color in wrong position)

Care is taken to ensure each peg in the secret code matches at most one peg in the guess.

## License
This game is free to use, modify, and distribute for educational purposes.

## Credits
Developed as a MIPS assembly programming exercise.

## Screenshots( In the Project report)


```
 __  __   _   ___ _____ ___ ___ __  __ ___ _  _ ___  
|  \/  | /_\ / __|_   _| __| _ \  \/  |_ _| \| |   \ 
| |\/| |/ _ \\__ \ | | | _||   / |\/| || || .` | |) |
|_|  |_/_/ \_\___/ |_| |___|_|_\_|  |_|___|_|\_|___/ 
```

Enjoy the game!