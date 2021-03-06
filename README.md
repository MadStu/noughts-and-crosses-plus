# Noughts and Crosses

This is a fun website for visitors who want to play the fun and addictive game of Noughts and Crosses (also known as Tic-tac-toe or Xs and Os). The website's target audience are people that enjoy quick strategy games. The varying difficulty levels make it suitable for all ages and abilities.

The key project goal is to provide the user with a trouble free game of Noughts and Crosses that has user controllable difficulty levels and which tracks the score accurately. The user should expect to intuitively know how to interact with the game and the feedback given should illicit a postive emotional response.

The live link can be found here - https://madstu.github.io/noughts-and-crosses/

It is designed to be responsive and accessible on a range of devices, making it easy to navigate for all users.

![Responsive Mockup](https://raw.githubusercontent.com/MadStu/noughts-and-crosses/main/assets/images/readme-images/responsive-website-mockup.png)

## Features 

### Existing Features

- __Typography__

  - For the main heading, scoreboard and the noughts and crosses themselves I chose the "Edo" font from [1001 Fonts](https://www.1001freefonts.com/edo.font).
  - This font is in a hand drawn, brushed ink looking style which users will appreciate and help them to feel like they're playing it by hand with a friend.  - I also styled the hard mode toggle switch with the same Edo font.

- __Colour Scheme__

  - I looked at a lot of background colours and felt the darkslategray (#2F4F4F) colour provided good contrast between the text, the gameboard and the background. And it's also nice and comfortable to look at, not being too bright or too dark.
  - The difficulty toggle switch has a background with the same shade of pink that the modal has (#FFC2C7) and is there to stand out and invite the user to change modes.
  - I wanted to use black and white colours for the game, as when we played as children it was mostly black ink on white paper, so I have a slightly off-white colour called whitesmoke (#F5F5F5) to represent a piece of paper.
  - The game lines were created with black and slightly fuzzy, again to make it feel to the user that it's hand drawn and they're playing with a friend.
  - The noughts and crosses on the game are not quite the blackest of black (#202020) but it matches the drawn lines colour and provides a high contrast to represent black ink.
  - The text colour is floralwhite (#FFFAF0) which is another off-white colour to just soften the brightness of a hard bright white a little and allows the user to keep playing without it becoming a strain.
  - The background colours do change depending on the outcome of the game. If the game is a draw, the background transitions into black. If the computer wins it turns bright red for a moment. But if the user wins it briefly becomes a kaleidoscope of bright and contrasting colours to celebrate.

![Colour Scheme](https://raw.githubusercontent.com/MadStu/noughts-and-crosses/main/assets/images/readme-images/colour-scheme.png)

- __The Title Area__

  - The title area has a bold title of the website/game name in the Edo font.
  - The text below tells the user how to win the game.

![The Title Area](https://raw.githubusercontent.com/MadStu/noughts-and-crosses/main/assets/images/readme-images/title-area-screenshot.png)

- __The Gameboard__

  - The Gameboard area is where you play the game.
  - On top of the gameboard it displays who's turn it is and also whether the hard mode is ON or OFF.
  - The hard mode can be toggled on or off by clicking or tapping the ON/OFF text.
  - The ON/OFF toggle is using the Edo font.
  - The game will reset if the user toggles the hard mode.
  - The user can click or tap on whatever square they'd like to take their turn.
  - The gameboard will shake to provide feedback to the user when they try to take a turn but the square is already occupied, or if they try to place their nought but it's not their turn.
  - The gameboard will also shake when it's resetting itself.
  - The gameboard has rounded edges to provide a more visually comfortable playing area.

![The Gameboard](https://raw.githubusercontent.com/MadStu/noughts-and-crosses/main/assets/images/readme-images/gameboard-screenshot.png)

- __The Modal__

  - The modal displays a brief message to provide feedback to the user about the conclusion of each game.
  - There are 3 game outcomes. If the user wins the game, they're shown a message that reads "WINNER!". If they lose, the message reads "LOSER" and if there is no winner the message reads "DRAW".
  - The modal message uses the Edo font and is the same colour as the main  background, darkslategray.
  - The modal itself has a pink background, black outline and rounded edges.
  - The modal removes itself automatically within a few moments of displaying, but you can also click anywhere outside of the modal, or on the cross to close the modal if required.

![The Modal](https://raw.githubusercontent.com/MadStu/noughts-and-crosses/main/assets/images/readme-images/modal-screenshot.png)

- __The Scoreboard and Footer__

  - This Scoreboard area shows the user their current score, the computer's current score and the number of draws they've had.
  - The scores update once each game has reached it's conclusion and a winner or draw has been declared.
  - The scores reset to 0 if the player changes difficulty.
  - The footer provides links to the author's linkedin page and also the project's GitHub page. The links open in new tabs.

![The Scoreboard and Footer](https://raw.githubusercontent.com/MadStu/noughts-and-crosses/main/assets/images/readme-images/scoreboard-and-footer-screenshot.png)

### Features Left to Implement

- Add sound effects.
- ~~Add another difficulty level.~~
- Take turns with the computer at who goes first.
- Allow user to choose to play as noughts or crosses.

## Testing 

I tested the website on a number of browsers and devices and all is working as intended.

I also asked a number of my fellow students to test it's functionality and try to break it. Any bugs found are listed in the [Unfixed Bugs](#unfixed-bugs) area

The responsive design allows for different screen sizes as proven by using [Responsinator](http://www.responsinator.com/?url=madstu.github.io%2Fnoughts-and-crosses%2F)

### Validator Testing 

- HTML
  - No errors were returned when passing through the official [W3C validator](https://validator.w3.org/nu/?doc=https%3A%2F%2Fmadstu.github.io%2Fnoughts-and-crosses%2F)
- CSS
  - No errors were found when passing through the official [(Jigsaw) validator](https://jigsaw.w3.org/css-validator/validator?uri=https%3A%2F%2Fmadstu.github.io%2Fnoughts-and-crosses%2F&profile=css3svg&usermedium=all&warning=1&vextwarning=&lang=en)
- JS
  - No errors were found when passing through [JSHint](https://jshint.com/)
- Other Tests
  - No problems were discovered when testing with the [WAVE tool](https://wave.webaim.org/report#/https://madstu.github.io/noughts-and-crosses/)
- Accessibility
  - I confirmed that the colours and fonts chosen are easy to read and accesible by running it through lighthouse in devtools.

![Lighthouse Score](https://raw.githubusercontent.com/MadStu/noughts-and-crosses/main/assets/images/readme-images/lighthouse-results.png)

### Unfixed Bugs

- ~~When the human player has won a game and there's still free spaces available, the computer takes a turn and records itself as having won before resetting the board.~~
- ~~When the human player has won a game and there's still free spaces available, the computer takes another turn before resetting the board.~~
  - Fixed the 2 above by moving a function call for the computer to take a turn which was in the wrong place.
- ~~The computerSquareHard() function does not loop through the eligibleNumsArray.~~
  - I changed to a for loop which fixed the problem.
- ~~The number returned from computerSquareHard() is the square number but is interpreted as the array index number.~~
  - This led to the computer placing it's X in the wrong square which wasn't intelligent, but an easy fix to return the array value instead of the index.
- When the user toggles the difficulty level very quickly after placing their nought, the computer takes the first turn on the freshly reset board.
  - I haven't fixed this yet but I plan to create a global variable whose value is a unique ID for each game, probably based on the Epoch Unix Timestamp and each move is checked against the timestamped game ID. With Each newly reset board comes a new and unique game ID.

## Deployment

- The site was deployed to GitHub pages. The steps to deploy are as follows: 
  - In the GitHub repository, navigate to the Settings tab 
  - Then navigate to the Pages section 
  - From the source section drop-down menu, select the Master Branch
  - Once the master branch has been selected, the page will be automatically refreshed with a detailed ribbon display to indicate the successful deployment. 

The live link can be found here - https://madstu.github.io/noughts-and-crosses/


## Credits 

### Content 

- The "Edo" font was used from 1001 Free Fonts https://www.1001freefonts.com/edo.font
- The README.md file structure is based on the template provided by the Code Institute.
- I often used W3Schools and MDN web Docs as a guide for finding the best solutions and using the code in the correct format.
- I'd also search google which more often than not would show solutions written on stack overflow https://stackoverflow.com/
- My mentor has kindly shown a better way to listen for the click events in JS than I'd originally coded, which I've taken and used.

### Media

- The responsive mockup image at the top of the README.md was created at https://websitemockupgenerator.com/
- I used [photopea](https://www.photopea.com/) to draw the grid. 
- I also used [favicon-generator.org](https://www.favicon-generator.org/) to create the favicon. 