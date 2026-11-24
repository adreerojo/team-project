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
### Use Case 3
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
