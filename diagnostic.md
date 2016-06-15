# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What is the purpose of a backend?

```bash
stores data, communicate with the front-end, its the part of the application that is not visible for the users but makes the application functional and adds features
```

Which layer in the MVC pattern is used by the controller to fetch data?

```bash
the controller uses the model. The model communicated with the database and gives the required information back
```

Which layer in the MVC pattern communicates with the model?

```bash
the controller taks to the model
```

Why don't we use views in our interpretation of the MVC pattern?

```bash
because we make them ourselves and we havent learned it yet.
```

What does C.R.U.D stand for?

```bash
create
read
update
delete
```

In which part of the MVC pattern can we find C.R.U.D actions?

```bash
the model handels these things, but the model gets intructed from the controller what to do.
```
List at least 5 standard actions that C.R.U.D corresponds to?

```bash
- sign up a new user
- delte a review from a webpage
- post a comment in a blog
- create a  comment
- update a file in dropbox
```

A user action fires a `GET` request for `person/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```bash
1. get request goes to controller
2. controller: "hey get request!"--> goes to model
3. controller tells mode: "do this get request and get me the info I want about person/1"
4. model goes to database and looks for person/1
5. model finds person/1 and hands it back to controllercontroller says "cool thing"
6. controller tells the view that it found the request
7. view reders what ever it needs to dosplay the success to the users

9. voila
```

What is the command to generate a new rails-api app?

```bash
rails new app_name
```

What is the command to start an instance of a rails server?

```bash
rails server -p 3001

-p 3001 makes the server run on port 3001, so you can have several rails server
```

What are the commands to drop, create and migrate a database? (3 bullet points)

```bash
- rake db:drop
- rake db:create
- rake db:migrate
```

What is the command to scaffold a pet with a name and an age?

```bash
Scaffold allows us to specify how the application database may be used

$ rails generate scaffold Post name:pet title:string content:age
```

List two advantages of using serializers? (2 bullet points)

```bash
 - serializer can include logic that protects stufff you don't want everybody to see (passwords, bank account numbers)
 - more control over how the pbject you request will be represented
```
