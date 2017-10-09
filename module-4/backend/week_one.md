## Week One - Module 4 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week. 

Note: When you're done, submit a PR. 

1. What's the most useful thing you learned from completing the intermission week work?
* Easily that I am capable of learning a new technology/language on my own. 
2. What are some tools to help debug JavaScript code?
* debugger, using console.log(x) like puts, and pryjs
3. What are some tools you need in order to unit test your JavaScript?
* mocha, chai,
4. What is the syntax for invoking a function?
* myFunctionName()
5. What's `this` in JavaScript?
* similar to 'self', 'this' is used to reference the next highest scoped object in order that you might be able to change the attributes of a thing from within.
6. What is Webpack and why is it useful?
* Webpack is nodejs version of a server, and allows us to test our javascript client side experience.
7. When/why do you want to use event delegation?
* always! use event delegation to change the page dynamically after the browser loaded by listening for user actions and performing page manipulations thereafter. 
8. What's `npm` and what do we use it for?
* npm stands for node package manager, and is like nodejs' version of a gemfile. 

#### Review  
9. What's the MVC design pattern? Describe each part of MVC.
* MVC, or Model View Controller, is a way of designing an app's server-client process, where http requests are sent first to a controller, which then uses a model to format data for a view, which is then sent back to the original client. Its a way of dividing and separating out the responsibilities between routing, data-manipulation/returns, and html/xml/erb response.
10. What are a few ways to optimize a Rails application?
* Im not sure how to answer this question. My best guesses include: refactoring out redundant code and spaces; caching large dataloads; 
11. What's a background worker? When would we want to use a background worker?
* background workers are elements of your app that run all the time underneath your applications user interface and/or in response to specific user actions, but behind the scenes. It allows time-lengthy processes to be performed while the user can continue working on the app.
