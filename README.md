
# Faisal's Portfolio
### My Portfolio for Programming 101, Spring 2024.
## ***Subway Mysteries***, An Adventure Game:

***Subway Mysteries*** is my Midterm Project and the gem of my portfolio. It allowed me to learn so much more about C# and it helped me identify what the best methods of building code that allows reusability in any context needed.

- The main menu of my game uses a reusable dynamic system that allows the adding or removing of options.
![Main Menu of Adventure Game](/sm-mainmenu.png)

- My ingame menu combines two systems to identify key presses. The first system checks for numbers and the other checks for letters. Using this method allows the player to pick a station/world to go to while also making access to external menus (Pause, Backpack, etc.) always available.
![In-Game Menu of Adventure Game](/sm-ingame1.png)

- The map uses a similar system to the ingame menu that allows players to move with the arrow keys while also listening to any other input. In addition, it uses a grid that stores values and presents it as a letter (See image below...) which allows reusability.
![Adventure Game Map](/sm-map.png)

## My Trivia Game, and what I would have done differently:

The code below is a snippet from my Trivia Game. For me, this code worked fine and I had no issues with it. Looking back on it though, something I learned throughout the course is that it's better to write code that loops when initializing things. For example, in the code below I would initialize each Question/Answer on its own line, although this method works, it's not the most efficient and the reality is that it would have been better to have a List or Array of Questions and Answers then to loop through it to initialize the Trivia Questions. Another method would be to use an external file, and although the choice is up to the Developer, it is important to consider the most efficient method even with something as small as this. ***Small Differences are Noticeable***
```c#
private void CreateTriviaQuestions()
{
    TriviaQuestion Question1 = new TriviaQuestion("What color is the sky?", "blue");
    TriviaQuestion Question2 = new TriviaQuestion("What color is the sun", "yellow");
    TriviaQuestion Question3 = new TriviaQuestion("Which city in Illinois starts with the letters 'Chi'", "chicago");

    string[] Question4Choices = new string[] { "red", "yellow", "apple", "baseball" };
    TriviaQuestion Question4 = new TriviaQuestion("Which of the following is a fruit.", "apple", true, Question4Choices);

    Questions.Add(Question1);
    Questions.Add(Question2);
    Questions.Add(Question3);
    Questions.Add(Question4);
}
```
## Links

 - [My Github](https://github.com/faisal-alb)
