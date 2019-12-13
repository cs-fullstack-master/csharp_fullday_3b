# csharp_fullday_3

## Complete Phases
1: Due at 10:30a, Get the server up and running using Postgres

2: Due at 12:45pm, See all recipes, add a recipe, and detailed recipe pages working (excluding the ingredient and instruction lists)

3: Due at 2:30pm, Edit and delete pages working.

4: Due at 4:00pm, Figure out lists and CSS

## Create a recipe app

Create a recipe site using a Postgres database. Each recipe should show up on the home page and allow the user to add a recipe or see the details of a recipe. Each recipe should have the following attributes in the database:        
        
- recipe name
- recipe author
- recipe publish date
- recipe picture
- recipe ingredients
- recipe instructions

### Index Page
- Welcome users to the site. Let them click a link to go to the home page.

### Home Page
- Have a link to the home page and a link to add a new recipe
- List all of the recipes using CSS Grid to organize them horizontally. See the attached images as resources.
- Allow a user to click somewhere on the recipe to link to the detailed page of each recipe.

### Add Page
- Have a link to the home page and a link to add a new recipe
- Include a form that will add a new recipe to your Postgres database.
- All of the ingredients should be on different lines.
- All of the instructions should be on different lines.
- Do not let the user add the publish date. It should be automatically populated. See the note below for date/time
- Once they hit submit, go back to the home page.

### Details Page
- Have a link to the home page and a link to add a new recipe
- List all of the details of the recipe.
- Each ingredient on a different line in the database should be on it's own bullet point.
- Each instruction on a different link in the database should be on listed numericaly.
- Include a button to edit and delete the information.
- The edit button should go to the edit page.
- The delete button should delete the recipe and go back to the home page.

### Edit Page
- Have a link to the home page and a link to add a new recipe
- Fill the form with the existing data. When you submit, the data should be updated. Keep the published date the same.
- Once the hit submit, go back to the details page.

### Note!!!
- You can use your previous projects as much as you want to.
- In the server, you can use ```DateTime``` as the data type.
- Download https://momentjs.com/ and put it in your javascript folder. If you need to use it in a javascript file, add the script ABOVE your js file in your html.
- You can get today's information with moment using this code: ```moment(Date.now()).toDate()```
- Make sure your publish date is not being reset when submitting your information.

## Challenge
- Figure out how to trim empty or blank white space in the between lines so they are not included a a step in ingredients or instructions
Example:
```
1 cup flour

2 tsp sugar
```
