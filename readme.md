This is a follow up test of LLMs ability to write code without extra assistance. 

For prior version, see: https://github.com/Mx772/skeetShootingGPT

For this test, I am using Windsail; a IDE fork of VSCode with a built-in API to connect to several LLMs. 

For this test, I am using Claude 3.5 Sonnet (11/27/2024).

# The idea:
A simple html scorecard for skeet shooting.

## Attempt 1:

Prompt:
```
Can you write a html website to assist in skeet shooting scoring? 

Some Requirements:
- Lets the user input the amount of station, with how many targets at each station. 
- Lets users input their name. 
- Lets users keep track of the score of each user for each station
- On the far right, totals the scores from each station. 
- For each station, the score is either 'x' or 'o', with X being 1 or a hit, o being 0 or a miss. 
- Displays the information in a table like arrangement
- Is interactable
- Uses cookies to store the information incase the user refreshes the site. 
```

Response in chat:

```
I'll help you create an interactive HTML website for skeet shooting scoring with all the specified requirements. I'll create a modern, user-friendly interface that stores data using cookies.

First, let me create an HTML file with CSS styling and JavaScript functionality.

Created `index.html` +252 -0 0

I've created a complete, interactive skeet shooting scoring website. Here's what I've implemented:

User Interface:
Clean, modern design with clear sections for setup and scoring
Responsive layout that works on both desktop and mobile devices
Easy-to-read table format for scores
Features:
Input fields for number of stations (default 8) and targets per station (default 2)
Player name input with add player functionality
Interactive scoring table where clicking cells toggles between 'x' (hit) and 'o' (miss)
Automatic total calculation for each player
Data persistence using cookies
Reset scores and clear all data options
Functionality:
All scores are stored in cookies and persist through page refreshes
Easy score toggling by clicking on score cells
Real-time total score calculation
Input validation for player names and numbers
Confirmation dialogs for reset and clear operations
Usage Instructions:
Set up the number of stations and targets per station (defaults to 8 stations, 2 targets)
Enter player names and click "Add Player" to add them to the scoring table
Click on any score cell to toggle between 'x' (hit) and 'o' (miss)
Total scores are automatically calculated and displayed in the rightmost column
Use the reset button to clear all scores while keeping players
Use the clear all data button to remove everything and start fresh
The website is ready to use! Just open the index.html file in a web browser. Would you like me to run it for you or would you like any modifications to the current implementation?

```

See code here:
[index.html](index.html)

Note:
> As we can see, compared to last year's attempt using the same prompt, we were able to get an exact answer with 1-shot prompting. Granted, this was a very simple test, but the growth from last year to this year is substantial; and the growth from this year to the next year is likely to be even greater.

## End Result:

![image](https://github.com/user-attachments/assets/588ea09b-04ee-4893-b8bd-1477fd6c8df1)

