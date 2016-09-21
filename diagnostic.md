# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```bash
A backend acts as a database, and gives you the ability to store and retreive data.
```

Which layer in the MVC pattern is used by the controller to fetch data?

```bash
The `models` layer.
```

Which layer in the MVC pattern communicates with the model?

```bash
The `controller` layer.
```

Why don't we use views in our interpretation of the MVC pattern?

```bash
Because it is the job of the front end.
```

What does C.R.U.D stand for?
```bash
CRUD stands for:
Create
Read
Update
Destroy
```

In which part of the MVC pattern can we find C.R.U.D actions?

```bash
In the controller, which communicates with the model.
```

List at least 5 standard actions that C.R.U.D corresponds to.

```bash
1. Create
2. Show
3. Index
4. Update
5. Delete
```

A user action fires a `GET` request for `/persons/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```bash
  - the request (a GET in this case) is received by the ROUTER
  - the ROUTER selects the appropriate controller (in this case, the one for PEOPLE)
  - the controller tells the model to carry out the request
  - the model makes a request to the appropriate database
  - the DB searches for a PERSON (singular) with the ID of `1` in the PEOPLE table
  - the information (data) is given back to the model
  - the model gives the data back to the controller
  - the controller gives the data to the front end so it can be rendered in the
  browser and viewed by the user who fired the request
```

What is the command to generate a new rails-api app?

```bash

```

What is the command to start an instance of a rails server?

```bash
Typing `bundle exec rails s` in the terminal spins up the rails server.
```

What are the commands to drop, create and migrate a database? (3 bullet points)

```bash
  -dropdb tablename
  -createdb tablename
  -bundle exec rake db: migrate
```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash
I am not sure, but I think it is:
rails scaffold pet name:string age:integer
```
