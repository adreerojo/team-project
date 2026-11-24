# Team Project

Please keep this up-to-date with information about your project throughout the term.

The readme should include information such as:
- a summary of what your application is all about
- a list of the user stories, along with who is responsible for each one
- information about the API(s) that your project uses 
- screenshots or animations demonstrating current functionality

By keeping this README up-to-date,
your team will find it easier to prepare for the final presentation
at the end of the term.

# Cuble
## Team Information
### Team Members
Adrian Arrojo  
Tanish Ariyur  
Song Hyeokjae  
Jiu Lee

---
## Project Description
### Domain: 
Recreation & Competition 

### Description:
Cuble is a Daily Rubik's Cube Challenge game, providing daily scrambles for users, inspired by Wordle. Users can track their daily scramble progress and view their global rankings in a range of official WCA events.
---
## User Stories
### User Story 1
As a cuber, I want to solve the daily scramble (Tanish)

### User Story 2
As a cuber, I want to view a daily leaderboard to see where I globally rank, and see the top cubers and solve times for the day. (Jiu)

### User Story 3
As a cuber, I want to be able to view my past daily scramble solve times, so I can measure my progress (Jae)

### User Story 4
As a cuber, I want to create an account and login so I can solve the daily scramble and track my solves (Adrian)

## Use Cases
### Use Case 1 (Tanish)
Solve the daily scramble and save it:

#### Primary Actor
The user (player) who wants to solve the Daily Scramble
#### Preconditions
- The user is logged in to their Cuble account
- The user has not yet attempted the Daily Scramble for that day
#### Trigger
The user clicks “Solve Daily Scramble”, prompting them to the Daily Scramble view. Then, they can see the scramble of the day, and hold the space bar for 2 seconds to begin the timer.
#### Success Outcome
When the user ends the timer (by clicking their spacebar while the timer is on), the scramble is deemed “solved”, and the Solve is saved to the user’s account, tracking the scramble and the time taken to solve (i.e. the Solve is recorded as soon as the timer is stopped).

#### Main Success Scenario:
    i. The user asks to solve the daily scramble
    ii. The system checks that the user hasn’t already attempted the daily scramble
    iii. The user is prompted to the Daily Scramble view
    iv. The user holds the spacebar for 2 seconds to begin the solve
    v. The system begins the timer, once the spacebar is held for 2 consecutive seconds
    vi. The user clicks the spacebar once, while the timer is running, to stop the timer.
    vii. The system saves the scramble, and time taken, as a Solve, for the user.
    viii. The system displays the time taken for the user to solve today’s Daily Scramble.

### Use Case 2
View and query my past daily scramble times. 

#### Primary Actor 
The user (player) who wants to view and query their past Daily Scramble times.
#### Preconditions
- The user is logged in to their Cuble account
#### Trigger
The user clicks "View Past Times", prompting them to the Past Times view, where they can see their previous times represented in a histogram (Scramble Time vs. Solve Date). If the user has no previous Daily Scramble times, then the histogram will have no data. The user can then click "View Histogram" or "View List" to toggle between the histogram view and the list view, where the list view shows the past times in a tabular format. In either view, the user can filter their past times by Solve Type and date range. 
#### Success Outcome
When the user is able to view the histogram/list of their previous times. 

#### Main Success Scenario:
    i. The user asks to view their past Daily Scrambles
    ii. The user is prompted to the Past Times view
    iii. The system requests this user's past daily scramble times
    iv. The system constructs the histogram and list view, and shows the histogram in the view (hiding the table)
    v. If the user toggles between the histogram and list view, the corresponding view type will be displayed.
    vi. If the user applies filters, the system will update both the histogram and list view.

### Use Case 3 (Jiu)
View the daily leaderboard, displaying top solve times from cubers for that daily scramble

#### Primary Actor
the user (cuber) who wants to check their rank and see the fastest record for the day
#### Preconditions:
The user is logged in to their Cuble account
Leaderboard data is available by the selected date and the cube type
#### Trigger 
the user selects “view daily leaderboard”
#### Success Outcome
The system displays leaderboard for the selected date and cube type, showing the top 10 cubers and the user’s rank if they have a solve record.

#### Main Success Scenario 
    i. The user asks to view the Daily Leaderboard
    ii. The system displays the leaderboard for the current day, refreshed with that day’s recorded solves
    iii. The user selects a cube type and date to filter the leaderboard
    iv. The system displays the top 10 cubers and their solve times matching the selected filters.
    vi. If the user has a solve record for the selected date and cube type, the system displays their rank.
    v. The user selects “view more” to see the next 10 cubers 
    vi. The system displays the next 10 results. The user can repeat this to view more results.


### Use Case 4 (Adrian)
Create and account and login:

#### Primary Actor
The user (player) who wants to login
#### Preconditions
- The user does not have a Cuble account, or;
- The user is not logged in to their Cuble account
#### Trigger
The user clicks “Create Account”, prompting them to create a username and password. Or, they select "Login" to enter their existing username and password
#### Success Outcome
The user is created and saved in the database, or the user is now logged in and can solve the daily scramble.

#### Main Success Scenario:
    i. The user asks to create an account and enters a username and password
    ii. The system checks that the username does not already exist
    iii. The system saves the user in the database
    iv. The user is prompted to login and enters their username and password
    v. The system obtains the users data from the database
    vi. The user is now logged in and can solve the daily scramble
---
## Minimal Viable Product (MVP)
| Team Member | MVP Use Case |
|-------------|--------------|
| Tanish | Solve the daily scramble and save it |
| Jiu | View the daily leaderboard |
| Jae | View previous daily scramble solve times |
| Adrian | Create an account and login |
---
## Entities
### Cuber
### Scramble
### Timer
### Solve
### Leaderboard
---
## API Usage
**API Name:** Scramble Web API
**Documentation:** https://github.com/campos20/scramble-web-api
**How it is used in the program:** TODO

---
## Design Diagrams
### UML Class Diagram
### Sequence Diagrams
---
## How to Run
[Instructions for running the program.]
---
## Notes
[Any additional project information.]
