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