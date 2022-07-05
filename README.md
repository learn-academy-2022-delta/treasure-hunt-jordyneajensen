# 💰 React Treasure Hunt Game

### 🤔 Remember
- Pseudocode!!
- Ask clarifying questions

### 📚 User Stories
x As a user, I can see a page with a 3 by 3 grid board game with a question mark in each square.
 - Branch: grid
    -added an empty dice to Square component, Styled in css to have height, width, border
    -Imported and called component in App.js
x As a user, when I click on one of the question marks an alert appears with the index position of that question mark in the array.
  -Mapped over board array in state to display Square component for each iteration
    - Added styling on a div that surrounds our mapped squares
    -Used flex and wrap, along with setting a width
    -centered both gameboard and header
    -passed the v alue of board to our square component to show question mark
    -passed index into square component
    -made on onClick method that alerts user to what index of the box
    -made a method in app.js to pull the information upstream from our child component. passed the method down to square to be involved when onClick is clicked.
x As a user, when I click on one of the question marks instead of the alert the question mark turns into a tree emoji.
    -destructured board from state so that we could update a single instance to a tree emoji when clicked
    -set state once update

x As a user, if I select the winning square the question mark will become a treasure emoji and if I select the losing square the question mark will become a bomb emoji.
 - setup componentdidmount to randomize a treasure location and set to state
 -checked if index is treasureLocation
 -if so emoji is a diamond, if not our emoji is a tree
 - repeated process to account for bombLocation 

- As a user, I can click on a “Play Again” button that will restart the game.

- As a user, I can see a counter that shows how many guesses I have left. The counter starts at 5 and decrements one every time I click on a square that is not the treasure nor the bomb.
- As a user, I can see a message informing me that I won the game if I select the square that contains the treasure.
- As a user, I can see a message informing me that I lost the game if I select the square that contains the bomb.
- As a user, I cannot continue to play the game after I win or lose.
- As a user, I can see a message informing me that I lost the game when I run out of turns (the counter reaches zero).


### 🏔 Stretch Goals
- Consider how to handle a situation where the bomb and the treasure are at the same index.
