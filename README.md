
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

![zEnter initial first player](https://github.com/Boilermaker74/Quiz-Bootcamp/assets/135560995/293a6fe8-c8ed-4c7b-b51d-c0c18014e7d0)

The player is penalized 10 seconds off the timer for every incorrect response. The final score is the seconds left on the timer after the quiz is completed.

At the bottom of the answers in the footer is the displayed correction to the response, either wrong or correct.

![zwrong](https://github.com/Boilermaker74/Quiz-Bootcamp/assets/135560995/2892468d-b656-453c-8de7-49adfa8d74d0)

![zcorrect](https://github.com/Boilermaker74/Quiz-Bootcamp/assets/135560995/57514608-a626-46e2-a499-85f40ee56d39)

The footer with the "wrong or correct" response to the players’s answer stays visible until the player removes the pointer from an answer button and returns the pointer back to the answer button.

When the timer expires the header displays game over.   Added an if statement so the timer can never drop below zero.

When the player completes the quiz, the quiz displays the message all done, displays the final score and provides a form box for the user to enter their initials.

![zGame over screen time over](https://github.com/Boilermaker74/Quiz-Bootcamp/assets/135560995/e4e9c1d2-2809-43a3-90d9-d8aac20374d3)


If the player tries to enter more or less then 2 symbols for their initials, the quiz responds with a  message telling the player to enter only two initials and displays the initials the player tried to enter.


![z3 initials](https://github.com/Boilermaker74/Quiz-Bootcamp/assets/135560995/f9b00d37-01d5-4e4f-8199-fc01ec592457)

Once player enters their initials a high score list is generated and each time a player enters their initials they are placed at the top of the list. 

![zHigh scores 1 score](https://github.com/Boilermaker74/Quiz-Bootcamp/assets/135560995/9c2a8acb-a101-43d8-b7ed-ba530ecdf63c)
![zHigh score 2 scores](https://github.com/Boilermaker74/Quiz-Bootcamp/assets/135560995/0b691b4d-48dd-4202-ad78-f6f13f5087cf)

The High score list is limited to 10 players. If the high score list has more than 10 players and the player enters their initials, the last player is removed from the list and the new player is placed at the top and the list remains with 10 players until the list is cleared.

![zfulllist 1](https://github.com/Boilermaker74/Quiz-Bootcamp/assets/135560995/3d87b899-d146-47ad-9265-bcdc6e234348)
![zfulllist 2](https://github.com/Boilermaker74/Quiz-Bootcamp/assets/135560995/346a7d89-4fff-4180-9b1b-a09d9c713f26)
![zfulllist 3](https://github.com/Boilermaker74/Quiz-Bootcamp/assets/135560995/8b3829a7-3bd4-4d48-830a-b0b47300956e)

The players initials and scores are saved in local storage under the values dogshow and scoreshow because I couldn't think of a better name.

![zlocal memory](https://github.com/Boilermaker74/Quiz-Bootcamp/assets/135560995/8163238e-cabb-4bb5-af4d-720f6d109401)

All buttons change color when they are hovered over.

Before Hover:

[Before Hover:](https://boilermaker74.github.io/)

![zhoveroff](https://github.com/Boilermaker74/Quiz-Bootcamp/assets/135560995/e1691c26-9b2b-40af-87ff-43b54f355a0c)

While Hovering:

![zhoveron](https://github.com/Boilermaker74/Quiz-Bootcamp/assets/135560995/fae8b4e6-589e-4bcc-974d-b586c4585773)

The “Clear high score” button removes the scores from the list and local memory.

![zcleared high scores](https://github.com/Boilermaker74/Quiz-Bootcamp/assets/135560995/1860844d-487b-4266-8865-d5eb454353cb)

The view high score button at the top left of this screen returns the player to the “high score list”

Thank You!
