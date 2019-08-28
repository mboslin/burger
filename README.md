# Burger - DEVOUR BURGER

### Overview

Burger is a full stack, MVC (Model-View-Controller) application that allows you to create burgers (POST), view a list of burgers available to eat (GET), devour burgers (PUT), and throw them away after devoured (DELETE).

Please check out the launched app on Heroku [Click Here](https://shrouded-crag-31044.herokuapp.com/)!


### Functionality

Using an ORM, the app has 3 main CRUD functions.
  1. READ all entries from the MySQL database and display them to the DOM using Handlebars.
  2. UPDATE a selected burger by clicking "Devour it", which
    * Triggers a `/burger/eat/:id` route in Express to change its "devoured" status in the MySQL database.
    * Re-routes the webpage back to the index, where the burger is now in the devoured column (via Handlebars).
  3. CREATE a new burger using the "Place Order" form, which
    * Triggers a `/burger/create` route in Express to insert a new burger into the MySQL database.
    * Re-routes the webpage back to the index, where the burger is now ready to be eaten column (via Handlebars).


    ![Alt Text](Screenshots/burger.gif)