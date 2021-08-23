# Weekend Challenge 11 - React-Redux Feedback Form

## Instructions

Reviewing code is an important role developers play. We're going to practice reviewing code from others.

- Get the repo url from your partner
- Get your partner's project running on your computer
- Review the code from your partner and give relevant feedback
- Complete the Markdown section and submit that in the notes section on the assignment app. (Make sure you include who's code you reviewed.)

Practicing compassionate code reviews is important (you can learn more from this video on the topic: https://www.youtube.com/watch?v=Ea8EiIPZvh0 )

## Review Checklist

## Base Required Features 

- Multi-Part Form:  
  - [X] Able to add feedback
    - [X] Data collected on individual pages & components
    - [X] Click on next takes you to the next page in sequence
    - [X] Data saves in DB after *all* the parts are completed (not piecemeal)
    - [X] Thank you page takes you back to the first view
    - [X] Old Data is cleared on form completion

- Client code:
  - [X]  Individual components for each form part
  - [X]  Redux setup complete
    - [X] Store linked to react with `<Provider>`
    - [X] Store setup with reducer(s) and logger middleware 
  - [ ] Reducers & Actions Working
    - [X] Actions are in SCREAMING_SNAKE_CASE and semantically named
    - [ Payload but no "type" ] Actions have a `type` key, and `payload` if sending data
    - [X] Reducers are returning a new state, or the old state (not mutating)
    - [X] Reducers are using spread correctly (to keep old data, while adding new)
  - [X] Review Component shows at all times with current redux state
  - [X] React-Redux Working
    - [X] Dispatching actions onClick
    - [X] Grabbing data from the redux store with `useSelector`
  - [X] Axios POST request to add feedback


- Server code:   
  - [X] Router made for GET, POST


## General Items
Feedback should be provided for these items, but they do not impact scoring.

- Git 
  - [Yes] Multiple git commits showing incremental progress
  - [Yes] Commits are descriptive of the changes made or feature added 
  - [Yes] Has .gitignore with node_modules
  - [No] Readme file updated (assuming this is previously discussed)
- Code Style 
  - [No] Appropriate amount of code comments
  - [Yes] Code is consistently formatted
- Client
  - [Mostly] Appropriate use of HTML tags
  - [Nothing other then what was already there] Basic CSS styling with margins/padding


## Stretch Goals
First must be complete for score of  _Exceeds Expectations_

- Previous Steps
  - [No] allows a user to go to a previous step, either directly or by cycling backward thru the steps
  - [No] user can upate their score for a step
    - [No] new score is validated to not be empty
    - [No] redux is updated with new score
  - [No] user can continue on to review page and submit as in Base Mode


- Admin View
  - [No] All entries are visible with correct data from inputs
    - [ No] Most recent is at the top
  - [No] Can Delete an entry
    - [No] User is prompted before deleting
  - [No] Axios GET request to get all feedback for `/admin` view in componentDidMount

  Busywork Goals, consider removing or making more useful

- [No] Styling with Material UI
- [No] Ability to flag a feedback item on `/admin` for further review
- [No] Deployed to Heroku


## Markdown

```
Hey Jeremy,

General Feedback.

---
| Functional Requirements | Complete |
| --- | :---: |
| Multi page form with client side routing and navigation (next button) | yes |
| Data stored in Redux when navigating from page to page | yes |
| User is notified when trying to leave a blank score | yes |
| Review Component displays scores and comments from current redux state | yes |
| Submit button sends data to the server via Axios | yes |
| Confirmaion Page displays after data is POSTed to the server | yes |
| Button on Confirmation Page clears Redux and starts a new survey | yes |
| Views are broken down into components | yes |

---
### Notes:

Notes on the above Functional Requirements.

You have everything on the basic requirements done correctly I couldn't find anything that was wrong with it.

---
| General Items | Complete? |
| --- | :---: |
| More than 15 git commits | no |
| Commits are descriptive of the changes made or feature added | yes |
| Readme file updated | no |
| Appropriate amount of code comments | no |
| Code is consistently formatted | yes |
| Server code organized with router & module files | yes |

---
### Notes:

Notes on General Items

```
The readme file was not properly edited I make that mistake a lot as well. I would do a pass after your assignment is over and write some code comments on your work so the next person who views them can understand what's going on. 

There isn't enough commits I believe they'd like you to commit after almost every tiny thing. I have trouble doing this in my work as well so I personally can't fault you but what seems to work best for me (when I remember to do so) is commit every time I see the webpage functional even if it's not finished with a core feature. 
