![zQuestion 5](https://github.com/Boilermaker74/Quiz-Bootcamp/assets/135560995/750636ab-aff0-414c-a581-8072b78cae75)
![zQuestion 4](https://github.com/Boilermaker74/Quiz-Bootcamp/assets/135560995/fb86e1b2-b8f9-4842-9f60-d2a7cf63c4f4)
# 📖 Quiz Bootcamp
This project was a quiz which is composed of five questions.  The user is given a choice of four answers. A timer countdown of 75 seconds begins when the first question is displayed. 

I got the code for the timer at:  Youtube : “Very simple JavaScript timer [setInterval()]” https://www.youtube.com/watch?v=4piMZDO5IOI.

This is the Start Screen of the quiz.

![zfinal screen](https://github.com/Boilermaker74/Quiz-Bootcamp/assets/135560995/31c59799-1cd8-457e-b9de-a65660455420)

These are the five qustions with the corresponding answer cards

![zQuestion 1](https://github.com/Boilermaker74/Quiz-Bootcamp/assets/135560995/614519ed-03dc-4462-9a09-15ad2e67767d)
![zQuestion 2](https://github.com/Boilermaker74/Quiz-Bootcamp/assets/135560995/fa19bb78-8309-4f95-bdfc-0e2e7821bab1)
![zQuestion 3](https://github.com/Boilermaker74/Quiz-Bootcamp/assets/135560995/48afce03-572f-460f-ad5f-2294f7eeb9b4)
![zQuestion 4](https://github.com/Boilermaker74/Quiz-Bootcamp/assets/135560995/53f4e29a-7f25-4fd1-b948-ba96a94534e2)
![zQuestion 5](https://github.com/Boilermaker74/Quiz-Bootcamp/assets/135560995/12ec8d29-2ed3-4a5e-a60f-3da575ca7d2b)

 If the time reaches zero or the player answers all the questions, a final score is displayed and the user is allowed the option of adding their initials to the final score list. 

Add “Enter initial first player”.

The player is kind of penalized 10 seconds off the timer for every incorrect response. The final score is the seconds left on the timer after the quiz is completed.
These are the four question pictures with their corresponding answers. 

Add four screen pictures of the questions.
At the bottom of the answers in the footer is the displayed correction to the response either wrong or correct.
Add “wrong”
Add “correct”


The footer with the wrong or correct response to the user’s response stays visible until the user removes the pointer from an answer button and returns the pointer back to the answer button.
Add wrong
Add correct
When the timer expires the header displays game over.   Added an if statement so the timer can never drop below zero.
When the player completes the quiz, the quiz displays the message all done and displays the final score and provides a form box for the user to enter their initials.
Add Game over screen time over

If the user tries to enter more or less then 2 symbols for their initials, the quiz responds with a  message telling the user to enter only two initials and displays the initials the user tried to enter.

Add “All done screen with initials too long”

Once user enters their initials a high score list is generated and each time a user enters your initials they are placed at the top of the list. 
Add “High scores 1 score.png”
Add “High scores 1 score.png”
The list is limited to 10 users. If the high score list has more than 10 users and the player enters their initials, the last user is removed from the list and the new user is placed at the top and the list remains with 10 users until the list is cleared.
Add “fullist 1”
Add “fullist 2”
Add “fullist 3”
The players initials and scores are saved in local storage under the values dog show and score show because I couldn't think of a better name.
Add “local memory”

All buttons change color when they are hovered over.
The “Clear high score” button removes the scores from the list and local memory.

Add “Cleared High score”

The view high score button at the top left of this screen returns the player to the “high score list”












First created a timer

Next created a start button to begin game

Next worked on layout for game with buttons

Started with button boxes

Made headlines "timer and view high scores

Made them display in one line with timer floating left

Made card for question and added buttions

Started process of adding question to card via javascript

Trying to make a function to tally correct and wrong responses

Added text from quiz to my strings

I changed the answers on the quiz because choice 1 and 2 were never correct. Now for question 1 the correct answer is 2 and
for question 2 the correct answer is 1.

Tried to use a variable y to record answer choice, but it was stored locally in a function.

Global variable "i" was used to determine if answer choice was correct or not.

Added a footer where the "correct" or "wrong' message will be displayed.

Got the timer to display "game over message" when it reaches zero value

Got a wrong answer to penilize the player 10 seconds on the timer using Variable -=10

Added a function  to blank screen when the timer reaches zero

Started working on the start screen

Created a replica of the start screen which will be the starting point of the program and is where the program will return to after the quiz is
complete, if the user chooses to start again.

Cleaned up the footer so the message displayed resembles the example given by the university.

When the user chooses an answer, the program responds with a display footer of correct or wrong. I create a function, eraseWrong(),  that removes that display (function when the user hovers over a selection of answers to copy the example the university provided.

UNfortunately, now the message disappears immediately because when the user picks an answer, the program registers a mouse hover and erases 
the message.

Added a new function "micein", so that the user must leave the question and then re-enter before the displayed answer is erased.

I couldn't get the footer border to disappear prior to the first question display. I solved this by adding a script line in the HTML changing the footer border color to white. I later changed the color back to original in the javascript function for displaying correct and wrong answers.

I am getting a weird bug that hides the Enter initials screen when the time runs out. It only happens randomly. I spent 4 days trying to correct it. About 42 hous total.

Remove foot.innerHTML =  ""; at line 29 and 37 as it doesn't appear to do anything.

Removed document.getElementById("foot").style.borderColor = "white"; at line 213 as it doesn't appear to do anything.

Removed else statement at line 226 as it doesn't appear to do anything.


Changed statement document.getElementById("foot").style.display="none" to  document.getElementById("foot").style.display="" at line 210. This removed the bug. It took 40 hours to find this! Ha!

added line 213 to remove negative scores
if (settimer < 0) {
    setTimer = 0}

Added 
 if (i <= 5 && setTimer <= 0) {
        document.getElementById("foot").style.borderColor = "white";
        document.getElementById("foot").style.color = "white";
    }
at line 216 to remove results message if timer runs out

If the quiz ends and the player has a footer display with the result of the last response, the player needs time to read that result. Added the command setTimeout(eraseWrong, 1500); to the endquiz function at line 236. Will erase the last result footer but still allow the user time to see it.

Added a function to accept user input as an initial.

Added an error message if the user inputs anything other than 2 symbols for the initials

Began function for High score screen and storing to local storeage 

Used a class to style the fonts of each elements of the list

Created the final buttons for the game and assigned them multiple classes

Using inputs to append my list of high scores. Had difficulty registering the user imput so that the computer could read it.

using a for loop to add to high scores.

added an array to put scores into table.

Need to create a way to add to an array.

