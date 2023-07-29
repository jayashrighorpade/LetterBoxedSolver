# LetterBoxedSolver

## Overview
The Letter Boxed Solver is a web application built with Flask that helps users find solutions for the game "Letter Boxed" from The New York Times.

## How It Works
The web app allows users to input the letters they have from the game. Based on user preferences, the app looks for 1, 2, or 3-word solutions, as searching for solutions with 4 or more words can result in too many permutations and slow down the process. The solutions consist of words that can be formed using the letters in the box but are not adjacent to each other on the sides of the box. The key criteria for a solution is that it must use all the letters provided by the user.

### Word Lists
To find solutions, the app iterates through two word lists:

1. `words_easy.txt`: This list contains around 84,000 words with repeated letters removed. The app uses this list first to search for solutions.
2. `words_hard.txt`: If no solutions are found in the first word list, the app switches to this longer list, which contains around 286,000 words with repeated letters removed.

### Error Handling
If no solutions are found for the given letters, or if the user inputs incorrect letters, an appropriate error message is displayed.

### Interactive Feature
When a solution is found, an interactive "scratch-off" board appears on the right side of the app. Users can use their mouse to scratch and reveal the solutions, making the experience more enjoyable on non-mobile devices.

The Letter Boxed Solver is a handy tool for players of the game, offering quick and accurate solutions to the challenging puzzles presented in Letter Boxed from The New York Times.

