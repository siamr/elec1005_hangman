# Hangman

Simple hangman game implemented with Flask

# Installation

## Option 1: Ubuntu packages

    sudo apt-get install python-flask python-flask-sqlalchemy

## Option 2: pip

[Install pip](https://pip.pypa.io/en/stable/installing/), then:

    pip install Flask Flask-SQLAlchemy

# Run

    python hangman.py

Create dabase with:

    python -c 'from hangman import db; db.create_all()'

# Links

* Hangman github repository: https://github.com/vlopezferrando/hangman
* Slides: https://slides.com/victorlf/flask
* Flask: http://flask.pocoo.org
* Jinja2: http://jinja.pocoo.org/docs/dev/
* Bootstrap: http://getbootstrap.com
* JQuery: https://jquery.com

# User Manual

Objective
The overall objective of the Hangman Game is to correctly guess the word randomly picked by the program, and avoid getting ‘hanged’ (making 6 wrong guesses). 

Introduction
Double click on the executable file, titled ‘Hangman Game.’
The game will open on the Home Page, and prompt you to enter your name. 
Click ‘Play!’ to commence game-play. 

Game-play
The game opens with the gallows drawn, and a row of dashed lines. The number of dashed lines corresponds to the number of letters in the word. 
Guess a letter that you believe to be in the given word by typing it in the blank box, then pressing ‘Try letter.’
If the letter guessed is in the word, it will appear in its correct place in the word. You can then continue to guess other letters. 
If the letter guessed is not in the word, a body part will be added to the figure. Points will also be deduced from your final score.  
Repeat step 1. 
The round ends whenever the user correctly guesses the word, or makes 6 incorrect guesses - whichever occurs first. 
When the round ends, a pop up message will appear depending on whether you guessed the word (“You won!”) or didn’t guess the word (“You lost :-(“). 
You will then be given the option to play again, or return to the home page where you can view your score. 

Things to keep in mind!
Take note that not all incorrect letter guesses are afforded the same weight! Whilst every incorrect consonant guess will only deduct 1 point from your total score, an incorrect vowel guess will deduct 5 points from your score!
