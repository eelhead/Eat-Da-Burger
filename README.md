### Eat-Da-Burger

A MySQL, Node, Express, Handlebars restaurant app that lets users input the names of burgers they'd like to eat.

# Overview

Eat-Da-Burger! is a restaurant app that lets users input the names of burgers they'd like to eat. Whenever a user submits a burger's name, your app will display the burger on the left side of the page -- waiting to be devoured. Each burger in the waiting area also has a Devour it! button. When the user clicks it, the burger will move to the right side of the page. App stores every burger in a mysql database, whether devoured or not.

# Functionality

Using an home-grown ORM, the app has 3 basic CRUD functions...

READ all entries from the MySQL database and display them to the DOM using Handlebars.
UPDATE a selected burger by clicking "Devour It", which...
hits an /burger/eat/:id route in Express to change its "devoured" status in the MySQL database
re-routes the webpage back to the index, where the burger is now in the devoured column (via Handlebars)
CREATE a new burger using the "Place Order" form, which...
hits a /burger/create route in Express to insert a new burger into the MySQL database
re-routes the webpage back to the index, where the burger is now ready to be eaten column (via Handlebars)


![screen shot 2018-02-25 at 6 53 41 pm](https://user-images.githubusercontent.com/31674994/36649899-97ae9d56-1a5d-11e8-81f3-cf938ad4f72a.png)


Technologies Used
Node.js
MySQL Workbench
Node Packages (express, mysql, express-handlebars, body-parser)
Bootstrap

Installation
To run the application locally, first clone this repository with the following command.

git clone https://github.com/eelhead/Eat-Da-Burger.git
Next, install the application dependencies.

npm install
Finally, run the node server locally.

node server
Now, open the local application on port 3030 at the URL: http://localhost:3030/.

Enjoy!


![screen shot 2018-02-25 at 6 55 02 pm](https://user-images.githubusercontent.com/31674994/36649900-99805ab6-1a5d-11e8-967d-012fa61bc879.png)
