---
title:  "U Impactify"
subtitle: "E-learning for marginalized groups"
author: "Simon Ha"
avatar: "img/authors/typing.png"
image: "img/g.jpg"
date:   20-11-24 15:25:00
---

### CSCC01 [U Impactify](http://github.com/simonha9/U-Impactify)  
CSCC01 is a 3rd year Software Engineering course with a prerequisite of CSCB07 (see "Dollar Store" post).  In C01, we continually learned about modern software engineering practices and implemented them in groups.  

### Background  
As a project to work on throughout the semester, we had a choice between SportCred - an app where you can keep track of all your favourite sports teams with respective sports "player cards" trading and betting capabilities, and U Impactify - an e-learning platform for socially marginalized groups.  As you can probably guess, my group of 6 other insanely bright computer science students tackled the admittedly challenging task of building an education platform.

### Software Development Practices  
Like the B07 project, we implemented Agile methodologies in building this web-app.  At the beginning of the semester, we came up with a product backlog which consisted of the 4 main Epic features we wanted to develop.  To track project progress and overall organization we used Jira, updating tickets with screenshots of how to call endpoints and other necessary information as features were finished.  

The semester consisted of 4 biweekly sprint planning sessions where as a group, we decided upon which features out of the product backlog we would take by assigning story points and also taking the availabilities of everyone in the group into consideration.  Keep in mind that we are still students and have 4 other courses and probably 17 assignments to do at the same time.  Despite all the other assignments and academic committments we were forced to hold, we still managed to complete over 20 stories (minimum was 5) whilst holding up the quality standard we initially agreed upon.  I am very proud of my group for sticking with it, learning all these new frameworks and practices and building a great product.  

### Technologies Used  
Everyone in the group played the role of a Full Stack Developer, working on both the front and back-end.  Many of us had experience in one of either front-end or back-end, so we took this oppurtunity to learn a new skill and popular frameworks in both fields.  

For the front-end, we used React and Node, using React component and class idealogies to seperate each standalone feature into modular cogs in the metaphorical e-learning machine.  For those unfamiliar with React, it is a framework that is coded with JavaScript where each component has a render function which, as the name suggests, renders the component according to the function implementation.  

For the back-end, we used Spring and Hibernate to build the endpoints for which the front-end would call.  My team was not as familiar with these frameworks, so after creating the data model, I persisted all domain classes into PostgreSQL, and added documentation on how to get the server up and running.  In persisting the domain classes, I had to add annotations on the getters of each attribute which described the relationship this table had with another.  I re-learned and solidified my understanding of Spring and Hibernate while building CRUD (and other fancy) APIs.  The project can be found on my github /U-Impactify.  
