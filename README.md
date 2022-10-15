# MERN To Do App with JWT Authentication

## Description

This To-Do List project is a fullstack web application. Reactjs was used to create the frontend and Express was used to create the backend of this project. MongoDb was used to store the users data in a database and JWT was used to authenticate the user when he/she logs into the application. After entering the login information of the user, the JWT token can be found easily by opening up the console.
(NOTE: I used the resources below to correct errors and simplify my code for a neater appearance.)

## Table of Contents

<details open="open">
<ol>
<li><a href="#description">Description</a></li>
<li><a href="#table-of-contents">Table of Contents</a></li>
<li><a href="#installation">Installation</a></li>
<li><a href="#handling-sensitive-data">Handling Sensitive Data</a></li>
<li><a href="#usage">Usage</a></li>
<li><a href="#notice">Notice</a></li>
<li><a href="#credits">Credits</a></li>
</ol>
</details>

## Installation

### Project:

- First, create a folder that will store all the files for this project.

- You can now navigate to the Project's directory by opening up your terminal or command prompt and typing "cd/". For example:

```
cd todo-app
```

### Backend:

- For the Backend of this project, create the package.json file by typing in:

```
npm init
```

- Thereafter, build your Express app by individually typing npm install --save followed by:

```
body-parser
cors
dotenv
express
helmet
jsonwebtoken
mongoose
morgan
nodemon
```

- After the installation is done, you can run the the backend application by typing in:

```
npm run dev
```

- Open http://localhost:8080 to run the server in the browser.

#### Note: Security

- For the backend of this project, the Helmet middleware was used to secure this application.

### Frontend:

- For the Frontend/Client side of this project, create the react app by typing in:

```
npx create-react-app
```

- Thereafter, build your app by individually typing npm install --save followed by:

```
axios
bootstrap
react-bootstrap
```

- After the installation is done, you can run the the frontend application by typing in:

```
npm start
```

- Open http://localhost:3000 to run the frontend React application in the browser.

## Handling Sensitive Data

- An .env file is created to store the uri and password needed to connect to mongoDB. A secret code was also created for JSON Web Tokens.

- Inside the .env file, the following can be added:

```
uri=(enter your uri from your mongoDB account)
jwt-secret=(enter your secret JWT code)

```

- For privacy concerns, add this .env file to the .gitignore file to avoid pushing it to gitHub.

## Usage

- The Header appears at the top of the page. The user is able to login using their email address and password or sign up by filling in their first name, last name, email address and password.

- Once logged in, the user can add a task to their to-do list by typing in their task under the "Add Item" heading (in the placeholder) followed by clicking on the "add task" button.

- The users todo entries will now be saved under the "Things to do" heading. The user can delete their items are they please by clicking on the "delete task" button.

- All changes made to the users to-do list will be saved onced he/she logs out.

## Notice:

When any changes to project items are made, the server will restart and update these changes. This is because the Nodeman devDependency is installed and so these notifications will appear in the console or terminal. You can view the changes made to the frontend of the application by opening http://localhost:3000.

## Credits

- [Alex Merced](https://dev.to/alexmercedcoder/auth-with-express-with-jwt-mongodb-and-postgres-4a5)
- [HyperionDev](https://www.hyperiondev.com/)
- [Stack Overflow](https://stackoverflow.com/)
- [Traversy Media](https://www.youtube.com/watch?v=enopDSs3DRw)
- [Unsplash](https://unsplash.com/photos/RLw-UC03Gwc)
