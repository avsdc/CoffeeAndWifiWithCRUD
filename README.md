**Coffee And Wifi**


**Description**

CoffeeAndWifi is a CRUD application created in Python, and also uses Flask and SQLAlchemy.
The application has a SQLAlchemy database 'cafes.db'.

There are two classes in CoffeeAnDWifi. The first is class CafeForm that takes FlaskForm as parameter. 
It has 4 StringFields. These are name, location, open_time, close_time. There are 8 SelectFields. 
These are coffee, tea, smoothie, breakfast, lunch, bakery, wifi, power. There is also one SubmitField for submit.

The other class is class Cafe for creating a table. The parameters are id, name, location, open_time, close_time, coffee, 
tea, smoothie, breakfast, lunch, bakery, wifi, power.

The app.route "/" with the home function, displays the home page.

For the CRUD, the app.route "/cafes" with the cafes function, displays all the cafes (Read),
the app.route "/add" with the add_cafe function, allows adding a new cafe (Create),
the app.route "/edit" with the edit_cafe function, makes it possible to edit cafe information (Update).
A edit link from the cafes page, when clicked, navigates to /edit page. The same form CafeForm
is used for both add and edit.

Finally, a delete link from the cafes page when clicked, navigates to the "/delete" app.route that uses the delete
function, and makes it possible to delete a cafe from the cafe list (Delete).

**Requirements:**

Using pip install, install the following:

Flask 2.3.2
WTForms==3.0.1
Flask_WTF==1.2.1
Werkzeug==3.0.0
flask_sqlalchemy==3.1.1
SQLAlchemy==2.0.25
