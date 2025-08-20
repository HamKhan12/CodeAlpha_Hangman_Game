# Hangman Game in Python

A simple yet engaging command-line implementation of the classic Hangman game built with Python. Guess the word one letter at a time before you run out of attempts!

## 🎮 How to Play

1.  The game randomly selects a secret word from a predefined list.
2.  You guess one letter at a time.
3.  If the letter is in the word, it is revealed in its correct position(s).
4.  If the letter is not in the word, you lose one attempt.
5.  You have **6 attempts** to guess the complete word correctly.
6.  Win by guessing all the letters before your attempts run out!

## ✨ Features

-   **Clean Command-Line Interface:** Easy-to-follow text-based gameplay.
-   **Dynamic Word Display:** Watch the word get revealed with each correct guess (e.g., `_ _ _ _ _ _` becomes `p y t h o n`).
-   **Input Validation:** Handles repeated guesses gracefully.
-   **Case-Insensitive:** Your guesses are not case-sensitive.
-   **Limited Attempts:** Classic 6-attempt (lives) challenge.

## 🚀 Getting Started

### Prerequisites

-   **Python 3.x:** Make sure you have Python installed on your system. You can download it from [python.org](https://www.python.org/downloads/).

### Installation & Running the Game

1.  **Clone or Download the Script:**
    ```bash
    # If you have git, you can clone the repository.
    # Or simply copy the `hangman.py` file to your local machine.
    git clone <your-repo-url>
    cd hangman-game
    ```

2.  **Run the Game:**
    Navigate to the directory containing the script and run it using Python.
    ```bash
    python hangman.py
    ```

## 📁 Code Overview

The game is contained within a single Python file (`hangman.py`) with three main functions:

-   `choose_word()`: Selects a random word from a list.
-   `display_word(word, guessed_letters)`: Formats the word, showing guessed letters and hiding others.
-   `play_hangman()`: Contains the main game loop, logic for handling guesses, and tracking attempts.

### Customization

You can easily customize the game by modifying the `words` list in the `choose_word()` function. Add your own words to change the difficulty!

```python
def choose_word():
    words = ["python", "hangman", "programming", "developer", "openai", "challenge", "algorithm"] # Add more words here!
    return random.choice(words)
