# rahove-backend test project

Be sure to read **all** of this document carefully, and follow the guidelines within.

## case-study and actors of the project

### Actors

- public User:
    - view public  [tasks(questions)](./screenshots/public-tasks.png)
    - signup( create a new account)
- user ( logged in account)
  - give a [vote](./screenshots/vote.png)
  - create a [approach](./screenshots/create-approach.png)
  - create a [approach](./screenshots/create-approach.png)
  - create a [Task](./screenshots/create-task.png)
  - search for a task and approach
  - login

## tech-stack
  - implement logged-in user session using `redis` 
  - use `express` for the server
  - use your preferred database (`postgres`, `mongo`, ...)
  - include postman file in your subscription

## Context

The app concept is about building "question-answer site". It is for peoples to ask(create a 'TASK') or find concise
solution(query an 'Approach') for their problems.

Build a graphql API based on [this SDL](./schema.graphql)

### Functionality

- The API should follow typical Graphql API design pattern.
    - response with appropriate error response
    - use a fragment if there is a chance
    - optimizing data fetching with tools like `dataloader`
    - Avoid deeply nested field attacks
- The data should be saved in the DB.
- Provide proper API documentation.
- Proper error handling should be used.

## What We Care About

Use any libraries that you would normally use if this were a real production App. Please note: we're interested in your
code & the way you solve the problem, not how well you can use a particular library or feature.

_We're interested in your method and how you approach the problem just as much as we're interested in the end result._

Here's what you should strive for:

- Good use of current Node.js & API design best practices.
- Solid testing approach.
- Extensible code.


### Bonus

- Use docker to start your preferred database
- deploy to aws or your preferred infrastructure
