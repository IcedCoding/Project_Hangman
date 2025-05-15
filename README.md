# Hangman Game (Angela Yu 100 Days of Python)

This project is a simple implementation of the classic Hangman game, inspired by the curriculum of Angela Yu's 100 Days of Python Bootcamp. It demonstrates basic Python programming concepts, including variables, lists, loops, conditionals, functions, and importing modules.

## Features
- Random word selection from a word list
- ASCII art for game stages and logo
- User input for guessing letters
- Tracks correct and incorrect guesses
- Displays remaining lives and game status
- Reveals the correct word if the user loses

## File Structure
- `main.py`: Main game logic
- `hangman_words.py`: Contains the list of possible words
- `hangman_art.py`: Contains ASCII art for the logo and hangman stages
- `README.md`: Project documentation

## How to Play
1. Run `main.py`.
2. The game will display a logo and select a random word.
3. Guess one letter at a time.
4. If the letter is in the word, it will be revealed in its position(s).
5. If the letter is not in the word, you lose a life and the hangman art updates.
6. The game ends when you guess all letters or run out of lives.

## Concepts Demonstrated
- **Variables**: Used for tracking lives, chosen word, placeholders, and correct guesses.
- **Lists**: Used for the word list and hangman stages.
- **Loops**: The main game loop continues until the game is over.
- **Conditionals**: Used to check guesses, update the display, and determine win/loss.
- **Functions**: (If extended) Could be used to modularize code (e.g., for checking guesses, updating display).
- **Modules**: Demonstrates importing custom modules (`hangman_words`, `hangman_art`).
- **String Manipulation**: For updating the display and handling user input.

## Example Code Snippets

**Selecting a random word:**
```python
import random
import hangman_words
chosen_word = random.choice(hangman_words.word_list)
```

**Displaying the hangman art:**
```python
import hangman_art
print(hangman_art.logo)
print(hangman_art.stages[lives])
```

**Main game loop:**
```python
while not game_over:
    guess = input("Guess a letter: ").lower()
    # ... check guess, update display, lives, and game status ...
```

## Angela Yu's 100 Days of Python - Key Learnings Used
- Day 1-5: Variables, Data Types, Input/Output, String Manipulation
- Day 6-10: Loops, Conditionals, Functions, Lists
- Day 11+: Modularization, Importing Files, Project Structure

## How to Extend
- Add functions to modularize code (e.g., `def check_guess()`, `def update_display()`)
- Add support for phrases or longer words
- Add a scoring system
- Add a graphical interface (Tkinter or Pygame)

## Credits
- Inspired by Angela Yu's [100 Days of Code: The Complete Python Pro Bootcamp for 2023](https://www.udemy.com/course/100-days-of-code/)

---
Happy coding and keep practicing Python!