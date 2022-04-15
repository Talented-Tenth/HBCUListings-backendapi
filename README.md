# Talented Tenth 

<center>
  <p><img src=/"public/img/LogoWhite2.JPG" width="200" height="200"/></p>
</center>

<center>
  <p><img src="\public\img\LogoWhite2.JPG"how to width="200" height="200"/></p>
</center>

<center><img src="LogoWhite2.JPG" alt="centered image" height="200" width="200"></center>

![image](https://user-images.githubusercontent.com/94479449/163514553-b7f98158-186c-4f18-91ca-bdcecce495f9.png) 

<img src="https://user-images.githubusercontent.com/94479449/163514553-b7f98158-186c-4f18-91ca-bdcecce495f9.png" class=centerImage" alt="CH Logo" height="200" width="200"> 


# Historically Black Colleges & Universities API

The Talented 10th HBCU API was developed to allow for reading an HTTP API that queries available datasets of Historically Black College and Universities. This API will allow sign in / sign up authentication and create a favorites list, add to favorites list, and delete from favorites list.

This document explains:
<ul>
<li>How to create a "favorite listing" of schools which can include the schools(location, size, population, majors, cost etc.)</li>
<li>How to create query results using C.R.U.D endpoints</li>
<li>The data is read only for Create and Update</li> 
<li>The favorite lisiting will allow for Post and Delete</li> 
<li>How to use the "wild card" search for data</li>  
<li>How to define and execute queries as URLs</li>
<li>Extract query results in JSON format</li>
<li>Detecting query errors with error messaging and HTTP error codes</li>
<li>Authentication and Authorization using Basic Auth and OAuth</li>  
</ul>

# API Access 
<ul>
<li>A vaild username and password are required to access the API data.</li>
</ul>

# Introduction to using POSTMAN to access HBCU API

<ul>
<li>-To Create a listing of users with GET;</li>
<li>GET http://localhost:3000/users</li>
<li></li>  
<li>-To Delete a user to the database with Delete;</li>
<li>Delete http://localhost:3000/users</li>
<li>Body, raw, json</li> 
<li></li> 
<li>-To Add a user to the database with POST;</li>
<li>POST http://localhost:3000/users</li>
<li>Body, raw, json</li>
 <li> "name":"Dan"</li>
<li></li>
<li>-To Update a user to the database with PUT;</li>
<li>PUT http://localhost:3000/users</li>
<li>Body, raw, json</li>
 <li> "id":5</li>
  <li>"name":"Debra"</li>
</ul>

We started with an initial plan where we put our various ideas together on a google doc. Created an organization with two repositories (Backend & Frontend). Frontend with BasicAuth (for user input) and Backend (Seed file database). Creation of the project's organization and Cloning of repository. Initialized and installed tools as well as relevant dependencies. Revised scripts in package.json. Created development branches and testing environments. Created sprints to enable a smooth project planning in Jira. Established the Entity Relational Diagram with Draw.io. Distributed tasks between team members.

# Project Goals:
The goal of this project is for developers to have access to data regarding HBCUs for the creation of APIs for HBCUs (Historical Black College and Universities).

# HBCU History:
Institutions of higher education in the United States founded prior to 1964 for African American students. The term was created by the Higher Education Act of 1965, which expanded federal funding for colleges and universities... Their was a great debate in 1881 between Booker T. Washington who founded Tuskegee University and was an exemplary supporter of vocational training, which emphasized agricultural and industrial education vs W.E.B DuBois a Harvard trainded sociologist who was a prominent exponent of the intellectual approach to education. Du Bois argued for the necessity of cultivating a "talented tenth" of well-educated community leaders... for more historial information click on the link below:
https://www.britannica.com/topic/historically-black-colleges-and-universities


![image](https://user-images.githubusercontent.com/94479449/163096021-a134fee9-d716-4059-ba39-100cd0365c6e.png)
# Cheyney University
<ul>
<li>Cheyney University was founded in 1837 as the Institute
for Colored Youth, making it the oldest HBCU in the nation</li>
</ul>
  
# Technologies Used for HBCU Backend
<ul>
<li>JavaScript</li>
<li>Sequealize</li>
<li>SQLite 3</li>
<li>Express</li>
<li>*Postman</li>
<li>Basic Auth</li>
<li>OAuth</li>
<li>JWTs</li>
</ul>

*Click on the link below for detailed examples of how to use Postman:
https://documenter.getpostman.com/view/17252203/UUxxgoaP

# Code Dependencies for Backend
<ul>
<li>"dependencies":</i>
<li>"bcrypt": "^5.0.1"</i>
<li>"express": "^4.17.1"</i>
<li>"express-basic-auth": "^1.2.0"</i>
<li>"nodemon": "^2.0.13", </i>
<li>"sqlite3": "^5.0.2"</i>
</ul>


# Project Planning

<ul>
<li>JIRA</i>
<img width="800" alt="image" src="https://user-images.githubusercontent.com/94479449/162358989-2d3f25dc-157f-47c5-8afb-bd5ed3460156.png">


<li>ERD</i>

<li>This Entity Realtionship Diagram is a One-TO-MANY because it shows the relationship of one user being able to select several HBCU universities or colleges to create their list of favorite schools.</i>

![HBCU Talented Tenth drawio](https://user-images.githubusercontent.com/94479449/163228700-f27f1730-b5ed-48a6-bbe0-56e074bc7baf.png)

</ul>

# HTTP Status Codes

<ul>
<li>100 - Informational</i>
<li>200 - Success</i>
<li>300 - Redirection</i>
<li>400 - Client Error</i>
<li>500 - Server Error</i>
</ul>

Click on the link below for detailed explanation of status codes:
https://en.wikipedia.org/wiki/List_of_HTTP_status_codes

# Sample Code for Regex
A RegEx (Regular Expression), is a sequence of characters that forms a search pattern. RegEx can be used to check if a string contains the specified search pattern.

<ul>
<li>const searchTerm = req.query.search;</i>
  <li>const closeMatch = { "$regex": searchTerm, "$options": "i" };</i>
 <li>//find close matches for search term in username, title, tags, or body</i>
 <li>Post.find( { $or:[</i> 
    <li>{'username':closeMatch},</i>
    <li>{'title':closeMatch},</i> 
    <li>{'tags':{$in: [searchTerm]}},</i> 
    <li>{ "body":closeMatch}</i>
 <li>]})</i>
</ul>

# Github - Branch Update Process
<ul>
<li>How to perform the Git Hub Branch Process:</i>
<li>1. git checkout -b "new branch name"</i>
<li>2. git status</i>
<li>3. git add .</i>
<li>4. git commit -m " Provide notes what you are committing"</i>
<li>5. git push origin (new branch name)</i>
<li>Then go to your git hub and merge the request. Once you are done then go back to your vs code.</i>
<li>6. git checkout main</i>
<li>7. git pull origin main</i>
</ul>


  
# Production
The planning process for Talented-Tenth/HBCUListings-backendapi started each day with:
- Daily Standup meeting with the Scrum Master before the start of the work day and completing Daily Exit Tickets at the   end of the day.
- We Individually and as a group worked on our assigned tasks.
- Watched class recordings together to better understand certain concepts for a better realization of our project.
- Built a solid backend then worked on the frontend structures.
- Handled debuggings and other issues that came up.

# Team Members
- Irene Bowers
- Erica Newman
- Crystal Johnson
- Mohammad Kasem


