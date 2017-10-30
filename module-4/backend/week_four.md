## Week Four - Module 4 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week. 

Note: When you're done, submit a PR. 

1. What's your favorite project management tool?
  I prefer waffle to pivotal
2. Why do we create staging environments?
  To keep unfinished products away from production, so that bugs/errors/and precompilation issues can be solved without effecting the live product. 
3. What are the characteristics of a good README (in your opinion)?
  Explaination of hwo to start up the app, examples of code and explainations of structure of the app, the problems it aims to solve, and maybe even some history on the project and the impetus for its creation. 
4. What's one main improvement you're going to make to your code regarding accessibility issues?
5. What are some basic security concerns to be aware of when building applications?
   Injection (common in legacy code), Cross Site Scripting (possible any time you're not parsing data, also more possible in legacy code), and Sensitive Data exposure (which may be an issue both when data is being sent, stored publically in state, or un-encrypted in the database) were the major take-aways from the conversation. 
6. Why is continuous integration helpful/important?
  It keeps the project code constantly groomed for integration issues, so that major issues don't take place at the end of a project. 
7. What are some continuous integration tools?
  Travis CI -- which is currently causing me a lot of problems; Jenkins; GitLab; bamboo

#### Review  

8. What are some characteristics of "good" git workflow?
  Lots of comments, frequent commits, adequate and thorough discriptions within commits; merging pull requests into subsidiary branches and using development branch as a final place for integration testing, away from the production or master branch. 
  
9. What are the four fundamental concepts of object oriented programming?
Abstraction (keep the simpler methods toward the surface, keep more complex algorithms buried); Encapsulation (objects contain data and algorithms; encapsulation is the concept that 'enclosed' code, or objects, can be transportable and dependable); Polymorphism (that shared classes nonetheless can be instantiated with different methods/expressions of behavior); Inheritance (that behaviors can be transportable and that classes can receive behaviors from other classes).

10. What's a module in Ruby and what's the difference between a class and a module?
  modules are either used for namespacing similar but different classes, or for extending chosen behaviors into other classes.  
