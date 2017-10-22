## Week Three - Module 4 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week. 

Note: When you're done, submit a PR. 

1. At a high level, what is Node?
  Node is a runtime environment for running javascript code outside the browser. 
  
2. What is Express? What is Express similar to in the Ruby world?
  Express is similar to Sinatra, or Rails Server within Rails, in that it launches a make-shift server for handling HTTP requests and rendering templates.
  
3. How do we setup a route when creating an API with Node and Express? Please provide a code snippet.
  First, at the top of your page, you must require Express, and then use it as an instantiated object representing your app. Then you must set the port and listen for that port on your server page. Express gives you thereafter all the HTTP verbs as functions off this instatiated express app, and so you can write routes as follows: 
    // require express 
    var express = require('express')
    var app = express()

    // set port
    app.set('port', process.env.PORT || 1234)
    // set title of app
    app.locals.title = 'Secret Box'

    // construct route, in this case the home page
    app.get('/', function(request, response) {
      response.send('It\'s a secret to everyone.')
    })
    
    // listen for activity on this port
    app.listen(app.get('port'), function() {
      console.log(`${app.locals.title} is running on ${app.get('port')}.`)
    })

4. What do we use Knex for?
  We use Knex as a SQL query builder for communicating with the database from the Browser and from the backend environment, in our case Node.
  
5. How could you organize your code to follow the MVC design pattern in your Quantified Self project?
  You can organize model-related activity (database communication and data rendering) into a set of files, the routes and express code into a 'Controller' file, and similarly the html views in a folder as well.  

6. How do you execute raw SQL in node?
  Knex offers a .raw() function that allows you to interact with its database directly with raw SQL. Ex: 
    const find = (id) => {
      return database.raw(
        `SELECT id, name, calories FROM foods WHERE id = ${id};`
      )
    };
 
7. What are some advantages to having your front end and back end code live in separate applications? What are some disadvantages?
  Advantages include keeping different functionality (that of backend, data and template rendering, vs frontend post-load DOM manipulation) separate, refactored, and clean, which allows those separate code bases to be exported independently, as well as manipulated without affecting the other. 
  Disadvantages include (a) keeping codebases separate requires the two to run their servers simultaneously, and (b) when wanting to showcase your code, viewers will have to clone separate projects, which is annoying. 

#### Review  

8. Describe DNS.
  DNS's, or Domain Name Servers, are a list of domains and their associated IP addresses, which your browser uses to 'look up' IP addresses for sending HTTP requests to. Any time you type in a website, your browser uses a Domain Name Server to find the assocaiting IP address in order to initiate the Client-Server interaction via a request.
  
9. What does writing clean code mean to you?
  Abstracting complexities away from the higher-level models, organizing files in reference to the commonalities of task (i.e. adhering to the MVC model, above, where routing processing takes place in one file, database/data manipulation in another, perhaps front-end stuff organized separately by the html template they modify, etc.), and finding the most efficient, simplest way to accomplish goals. 
  
10. If you were building an application that models hotels, what classes would you need? What classes would be responsible for what functionality?
  ?
