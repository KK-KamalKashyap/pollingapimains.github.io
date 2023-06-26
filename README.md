# PollingAPI
API for Polling Questions - Coding Ninjas Backend Skill Test Project

Task: Need to create an API where anyone can create questions with options and also add votes to it

---

## Features
- Create a question
- Add options to a question
- Add a vote to an option of question
- Delete a question → (optional: A question can’t be deleted if one of it’s options has votes)
- Delete an option → (optional: An option can’t be deleted if it has even one vote given to it)
- View a question with it’s options and all the votes given to it

## Required Routes
- /questions/create (To create a question)
- /questions/:id/options/create (To add options to a specific question)
- /questions/:id/delete (To delete a question)
- /options/:id/delete (To delete an option)
- /options/:id/add_vote (To increment the count of votes)
- /questions/:id (To view a question and it’s options)

## Folder Structure
```
 Routes & URL

/questions/create

To create a new question hit the following URL with a post request:

https://polling-system-api-517c.onrender.com/api/v1/questions/create
/options/:id/create

To create a new option for a question hit the following URL with a post request:

https://polling-system-api-517c.onrender.com/api/v1/questions/:idOfQuestion/options/create
/options/:id/addVote

To increment the count of votes on an option, hit the following URL with a get request:

https://polling-system-api-517c.onrender.com/api/v1/options/:idOfOption/addVote
/questions/:id

To view a question and it’s options, hit the following URL with a get request:

https://polling-system-api-517c.onrender.com/api/v1/questions/:idOfQuestion
/options/:id/delete

To delete an option, hit the following URL with a delete request:

https://polling-system-api-517c.onrender.com/api/v1/options/:idOfOption/delete
/questions/:id/delete

To delete a question, hit the following URL with a delete request:

https://polling-system-api-517c.onrender.com/api/v1/questions/:idOfQuestion/delete
