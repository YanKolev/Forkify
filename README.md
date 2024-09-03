# Forkify
--Recipe and Cooking helping application--

-Planing phase -

1, User stories- description of the app's functionality from the user's prespective
-Common format- As a [type of user], I want [an action] so that [a benefit]

ex.
-As a user, I want to seach for recipes, so that I can find new ideas for meals. 
-As a user, I want to be able to update the number of servings, s that I can cook meal for different number of people.
-As a user, I want to bookmark recipes, so that I can review them later
-As a user, I want to be able to create my own recipes, so that I have them all organized in the same app.
-As a user, I want to be able to see my bookmarks and own recipes when I leave the app and come back later, so i can close the app safely after cooking.

-Feature planning:
-Search for recipes-> Search functionality, input field to send request to API with seached keywords, Display results with pagination. Display recipe with relevant data.
-Update the number of servings->Change servings functionality: update all ingredients according to current number of servings.
-Bookmark recipes->bookmark functionality
-Create own recipe-> user recipe, user recipes will automatically be bookmarked, user can only see their own recipes. 
-Store bookmark data in the browser local storage. On page load, read saved bookrmarks from local storage and display.

We need architecture as is it provide structure to the software. Maintainability and expandability should also be accounted. All combined will result to a the ''perfect architecture''.

There are many different types of architecture patterns: 
-MVC- model view controller,
-MVP- model view presenter,
-Flux.

Components of of every architecture
-Business logic:
    *Code that solves the actual business problem
    *Directly related to what business does and what it needs
    *Example: sending messages, storing transactions, calculating taxes
-State:
    *Essentially stores all the data about the application
    *Should be the ''single source of truth''
    *UI should be kept in sync with the state
    *State libraries exist(Redux)
-Http Library:
    *Responsible for making and receiving AJAX requests
    *Optional but alsmost always necessary in real-world apps
-Application logic(Router):
    *Code is only concerned about the implemenentation of application itself
    *Handles navigation and UI evens
-Presentation logic(UI layer):
    *Code that is concerned about the visible part of the application
    *Essentially displays application state

The Model-View-Contoller (MVC) Architecture

-Model:
    *State
    *Business logic
    *HTTP library(data taken from the web)

-Controller:
    *Application logic - Bridge between model and views (which dont know about one another)
-View:
    *Presentation logic(User)