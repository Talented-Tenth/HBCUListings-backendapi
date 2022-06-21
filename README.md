# Talented Tenth 
  <p float="left">
   <img src="public/img/HBCUTours.jpg" width="1000" height="450"     /> 
   </p>


# Historically Black Colleges & Universities API

The Talented 10th HBCU API was developed to allow for reading an HTTP API that queries available datasets of Historically Black College and Universities. This API will allow authorization and authentication as well as the ability to create, GET, POST, and DELETE a favorites list of preferred HBCU college and unversities.

This document explains:
<ul>
<li>How to create a "favorite listing" of schools by location, major, size, cost, population, etc.</li>
<li>How to create query results using C.R.U.D endpoints</li>
<li>The data is read only but allow for Create, Post, Delete a favorites list</li> 
<li>How to use the "wild card" search for data</li>  
<li>How to define and execute queries as URLs</li>
<li>Extracting query results in JSON format</li>
<li>Detecting query errors with error messaging and HTTP error codes</li>
<li>Authentication and Authorization using Basic Auth and OAuth</li>  
</ul>

# Acknowledgements:
Our name, Talented Tenth, is coined from the concept of Harvard educator and author, W.E.B Dubois, who emphasized the necessity of cultivating a "talented tenth" of well-educated community leaders to develop the leadership of black Americans, to become leaders to guide the devlopment and uplift of our communites through higher education.

We used the U.S Department of Education College Scorecard API as our main source of data to build our datasets of HBCU Colleges and Universities API. The purpose of this API is allow developers to have access to a dynamic dataset of HBCU listing supporting further development of APIs promoting HBCUs (Historical Black College and Universities).


# API Access 
<ul>
<li>A vaild username and password are required to access the API data.</li>
</ul>

# Introduction to using POSTMAN to access HBCU API

*Click on the link below for intstructions on how to use Postman:

https://documenter.getpostman.com/view/18690426/Uyr5myYG


  
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
<ul>
<li>https://documenter.getpostman.com/view/17252203/UUxxgoaP</li>
</ul>

# Code Dependencies for Backend
<ul>
<li>"dependencies":</i>
<li>"bcrypt": "^5.0.1"</i>
<li>"express": "^4.17.1"</i>
<li>"express-basic-auth": "^1.2.0"</i>
<li>"nodemon": "^2.0.13", </i>
<li>"sqlite3": "^5.0.2"</i>
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
<ul>
<li>https://en.wikipedia.org/wiki/List_of_HTTP_status_codes</i>
</ul>

# Sample Code for Sequelize - Model Querying - Basic Operators

<img width="473" alt="image" src="https://user-images.githubusercontent.com/94479449/163604706-da7303ef-228e-4342-931b-2e1c0570853d.png">





# HBCU API DATA Elements

Click on the link below for details of the API calls:
<ul>
<li>https://verizon.enterprise.slack.com/files/U02EKK1G43V/F03BG8Y420N/hbcu_api_data_elements.xlsx?origin_team=T013H7EC8R5&origin_channel=C03AFBUMPQA</i>
</ul>
  

# DevOp Developers
- Irene Bowers
- Erica Newman
- Crystal Johnson
- Mohammad Kasem



