# README #

###CS322 Project 3: Ajax Vocabulary Game###
###Author: Marc Leppold###

##Project Notes

The third project of CS322. An online vocabulary game designed for elementary school students. Creates a list of words, shows the user a bunch of random letters, then asks them to construct 3 of the shown words with their letters. In short, they're prompted to find anagrams. The user can freely enter the letters into a dynamic field that automatically checks if they construct a word, no need to submit the letters manually.

Once three words have been completed, the game goes to a victory screen and prompts the user to play again. Though scalable to large, random sets of words and letters, it's currently configured to give the same words each time. Systems are in place to ensure the user can construct at least 3 words.

Utilizes ajax, but also click, Flask, guincorn, itsdangerous, Jinja2, MarkupSafe, nose and Werkzeug. All of them are supplied with the configure script.


### USAGE ###

Execute flask_vocab.py, then enter 
```
HOST:PORT
```
into an internet browser, where HOST matches the IP address of the host computer and PORT matches the port the server is running on (default 5000). Note that there are various dependancies that will likely require executing the configure script first, notably Flask and Jinja2.

Can be executed via automated configure and makefile scripts as well:
```
git clone https://github.com/zenranda/proj3-anagrams InstallDirectory
cd InstallDirectory
make configure
make run
```
where InstallDirectory is the directory you cloned the files to.