# PROJECT 3: SIMPLE TO-DO  APPLICATION ON MERN WEB STACK
## Task:  To deploy a simple To-Do application that creates To-Do lists like this.
***
![sampletodolistproject](./Image/SampleTodolistproject.png)
***
MERN Web stack consists of the following components:
MongoDB: A document-based, No-SQL database used to store application data in a form of documents.
ExpressJS: A server-side Web Application framework for Node.js.
ReactJS: A frontend framework developed by Facebook. It is based on JavaScript, used to build User Interface (UI) components.
Node.js: A JavaScript runtime environment. It is used to run JavaScript on a machine rather than in a browser.
***
Update and Upgrade Ubuntu: 
```
Code: sudo apt update 
code: sudo apt upgrade
```
***
Installing Node.js- A JavaScript runtime environment. It is used to run JavaScript on a machine rather than in a browser.
![screenshot 7](./Image/Screenshot%207.jpg)
```
Code:sudo apt-get install -y nodejs
```
this code installs both node.js and npm (NPM is a package manager for node)
***

 A new directory for the Todo list project was created, project was initialised to create the 
![screenshot 8](./Image/Screenshot%208.jpg)
```
code: mkdir Todo
```
***
Next, you will use the command npm init to initialise your project, so that a new file named package.json will be created. This file will normally contain information about your application and the dependencies that it needs to run
![Screenshot](./Image/Screenshot%209.jpg)
```
code: npm init
```
***
INSTALL EXPRESSJS

Remember that Express is a framework for Node.js, therefore a lot of things developers would have programmed is already taken care of out of the box. Therefore, it simplifies development, and abstracts a lot of low-level details. For example, Express helps to define routes of your application based on HTTP methods and URLs.

![screenshot 10](./Image/Screenshot%2010.jpg)
```
code: npm install express
code: touch index.js
```
***
Now it is time to start our server to see if it works. If everything goes well, you should see Server running on port 5000 in your terminal. Inbound rule routed to port 5000.

![screenshot 12:](./Image/Screenshot%2012.png) 

```
code: node index.js
```
![screenshot 13:](./Image/Screenshot%2013.png)
***
MONGODB DATABASE
We need a database where we will store our data. For this we will make use of mLab. mLab provides MongoDB database as a service solution (DBaaS), so to make life easy, you will need to sign up for a shared clusters free account, which is ideal for our use case. Sign up here. Follow the sign up process, select AWS as the cloud provider, and choose a region near you.

![screenshot 14](./Image/Screenshot%2015.png)

 Mongoose a Node.js package that makes working with mongodb easier succesfully installed in Todo directory.
```
code:npm install mongoose
```
***

![screnshot 15](./Image/Screenshot%2015.jpg)

Model directory created, cd into model, Todo file created in the model directory

```
code: mkdir models && cd models && touch todo.js 
```
All three commands above defined in a single line of code using the "&&" operator
***

Postman API development client used to test our code without Frontend using RESTful API

![Screenshot 16](./Image/Screenshot%2016.png) 

***

Frontend Creation: Using react to create the frontend user interface of the To-do app for a Web client (browser) to interact with the application via API. To start out with the frontend of the To-do app, we will use the create-react-app command to scaffold our app.

Database connected succesfully

![Screenshot 17:](./Image/Screenshot%2017.png) 

```
code: npx create-react-app client
```
***
In this project, we will use Postman to test our API. You should test all the API endpoints and make sure they are working. For the endpoints that require body, you should send JSON back with the necessary fields since it’s what we setup in our code. Now open your Postman, create a POST request to the API. This request sends a new task to our To-Do list so the application could store it in the database.

POST request

![Screnshot 18:](./Image/Screenshot%2018.png)

GET request
![Screenshot 19:](./Image/Screenshot%2019.png) 

***
FRONTEND CREATION
Since we are done with the functionality we want from our backend and API, it is time to create a user interface for a Web client (browser) to interact with the application via API. To start out with the frontend of the To-do app, we will use the create-react-app command to scaffold our app.
Running a React App
Before testing the react app, there are some dependencies that need to be installed.
In the same root directory as your backend code, which is the Todo directory, run the code below: 
```
npx create-react-app client
```
Installing Concurrently: This is used to run more than one command simultaneously from the same terminal window.

```
Code: npm install concurrently --save-dev
```
Installing nodemon: This is used to run and monitor the server. If there is any change in the server code, nodemon will restart it automatically and load the new changes.
```
code:npm install nodemon --save-dev
```
***

Screenshot 20: React Logo
Screecnshot 21: Proxy line in package.json
Screenshot 22: Tod App up and running
