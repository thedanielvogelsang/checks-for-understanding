## Week Two - Module 4 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week. 

Note: When you're done, submit a PR. 

1. What's one difference between ES5 and ES6?
  ES6 accepts const and let, and also block scoped variables and arrow functions.
  
2. What's the difference between asynchronous and synchronous JavaScript? 
  Asynchronous code isn't fired/ran linearly and in order of placement (one after another), and can be intentionally structured to fire only when, say, certain in-time events take place after the broswer loads (jquery for instance), and also api calls that wait to fire the next dependent function in an operation, only once, say, a successful return is received (ajax), or once a previous function is complete such as in Promises--- in all instances, functions outside a specific sequence can continue to be executed out of 'sync' with these timed-out functions; In synchronous javascript functions are fired only one after another, and thus a subsequent function cannot fire until and only until the previous code is ran and executed.
  
3. What are the four pillars of Object Oriented programming?
  Polymophrism- that in object oriented programming, objects can be instantiated into multiple different forms, while retaining shared behavior, yet still individualizing itself if desired. 
  Inheritance- that classes can inherit functions/methods, and thus behavior, of other 'higher' classes and fellow object creators. 
  Encapsulation- the phenomenon of an object being a case of internal methods/properties/attributes, and can be 'moved around' and still retain its same functionality and properties despite changing locations and environments. 
  Abstraction- keeping the more complex code buried 'deeper' and further away from the user, refactored into organized and structured sub- or sister- files. 
  
4. What are some tools available in JavaScript to help you write object oriented code?
  Hashes serve as encapsulators for JS Objects, and can encapsulate both properties and functions (attributes and methods)
  
5. What are some key concepts to be aware of when refactoring your JavaScript?
  In javascript functions must be exported, which requires something like Webpack to share and require functions.

6. What's a callback function and what are some reasons when we use/need callback functions?
  Callback functions are functions that are executed by other functions, as arguments. We use them in order to create a chain of actions and so we can refactor out code. 
  
7. What's the scope of variables in Javascript?
  Var/Const variables (in Es5/Es6 respectively) are automatically hoisted to the beginning of their highest scope, while let (Es6) is a block scoped variable, which means its contained to its scope. This can mess with your code, so gotta be careful.

8. What's the difference between `==` and `===` in JavaScript?
  == is strictly equal, which functions more or less like == in Ruby, as an operator to determine likeness in code. For instance 2 == 2 would evaluate to true, while '1' == 'abc' would return false. === is an identity operator and evaluate to true only if the two objects/variables are identical, meaning they share object ids as well. 
  
9. Why do front end frameworks exist?
  To create an interactive experience for the users, to carry data, and to process and display dynamic information after brower loads. 

#### Review  

10. Why do people say "HTTP is stateless"?
  I really don't know.
11. Describe a RESTful API.
  RESTful APIs have HTTP requests that follow the same format for GET, POST, PUT/PATCH and DELETE, which correspond to specific routes / controller's methods: (INDEX/SHOW); (NEW/CREATE); (EDIT/UPDATE) and DELETE. 
12. What are some main characteristics of a team following an agile workflow?
  iterative and rapidly evolving responses to challenges, fast-to-production blueprints, and appreciation for editing, tests/measurements, and post-hoc enhancement.
13. What are some advantages **and** disadvantages to using OAuth to authenticate a user?
  advantages: outsourcing the responsibility of security to someone else; not having to store data.
  disadvantages: being dependent on the security and/or success of the hosting OAUTH sites' success.
