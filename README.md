This is forked from the Odin Project Tic Tac Toe program I found on another website. I noticed some bugs and unoptimized
so I took it and made some improvements to it. It now keeps score (the old one didn't), variable assignment is cleaner as well.

I plan on making some additional improvements as well once I have some free time. ORRRRRR, feel free to fork it and
make your own! :)

# The Odin Porject - Section 3: Ruby Programming
# Project OOP With Ruby, No. 1 Tic Tac Toe
#
# NOTE: Heavy use of comments intended for fellow students of The Odin
# Project who may be seeking insight into another's thought process.
#
#
# This in an implementation of the classic game Tic Tac Toe. I went a bit above and
# beyond the bare-bones solution to this problem, trying to create a more game-like
# experience with a user interface and some feedback. I use calls to clear the console
# and re-draw the screen often to achieve the illusion of a static game environment.
# The game keeps score of how many rounds each player has won, and automatically
# toggles between p1 or p2 going first, to make sure the starting advantage is
# spread out evenly. I implemented a very simple and rather dumb solution/winner
# analysis - the design right now only recognizes a draw when there are no more
# possible moves to make. Ideally it should be recognizing drawn games that can happen
# prior to a full board.
#
# I decided to separate the structure into four classes:
#
#  - The Game class is the primary loop class, it is the entry point and conductor.
# It controls the game-state, loops to progress through turns, and defines the
# overall program flow. Game score/stats are also tracked here.
#
#  - The GameBoard class contains everything needed to set up the board, keep track
# of the board-state, place markers on the board, and check itself for a win or
# a stalemate.
#
#  - The View class mostly holds a bunch of screen output for the user that I did not
# want cluttering up the Game class.
#
#  - The Player class keeps track of simple player info, like their name and symbol.
