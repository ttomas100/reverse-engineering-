## REVERSE ENGINEERING
PASSWORD AUTHENTICATION
This application allows the user to create an account, and easily authenticate the profile. The password and the email is storage in a database.

# USER STORY
I want to Log in to a site and be sure that my credentials are stored in the safest way possible..

# TECH USED 
-BCRYPTJS -EXPRESS -EXPRESS-SESSION -MYSQL2 -PASSPORT -PASSPORT-LOCAL -SEQUELIZE

# GETTING STARTED
Clone the repository
Create a passport_demo database in mysql.
Run npm i to install all the packages. 
Run in the terminal node server.js
The app will be running in http://localhost:8080

# FILES
# CONFIG
# MIDDLEWARE
- isAuthenticated.js: restricts the routes. Don’t allow visitors to go to any page if the user is not authenticated.

- Config.json: connection to the database
- Passport.js: here is the authentication process, is the javascript that tells the app that we want to login. 

# MODELS
- Index.js:  connects to database and imports users log in data;
- user.js Using bcrypt is a secured way to store passwords in my database regardless of whatever language my app's backend is built in, here we define what is stored on our database.
 
# ROUTES
- Api-routes.js: here we have all the routes to singing in, logging in and show the user specific data from the backend .
- html-routes.js here are the routes that check whether user is signed in, whether user already has account and send them to the correct html file.
- package.json: contains all package info, node modules used, version info.
- server.js: requires packages, sets up PORT, creates express and middleware, creates routes and syncs database / logs message in terminal on successful connection to server.
