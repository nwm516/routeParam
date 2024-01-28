# Handling Route Parameters in Express
This was for an assignment in my Web Applications & Development class, requiring me to "develop an Express NodeJS server that handles dynamic route parameters, allowing for personalized responses based on URL input". Pretty cool!
# Running the Server
I have found two ways in going about this:

<ins>Altering package.json:</ins> Including a "type" : "module" designation, and then additionally "start": "node routeParam.js" (singular parameter, btw) within the "scripts" identifier of the package.json file allowed me to run "routeParam.js" without needing to alter the filename.

"node routeParam.js" would successfully run the code with these alterations.

<ins>Running server as is:</ins> Running "routeParam.js" as "routeParam.mjs" allowed the program to proceed and the server to run successfully. Otherwise, importing express caused errors to occur, citing issues with importing modules from outside.

"node routeParam.mjs" would successfully run the code with these alterations.
# Testing the Server
Testing can be as simple as entering an intended user name after "/user" and seeing if the appropriate text output correlates to what was entered (which is largely how I tested). More in-depth solutions, such as implementing testing libraries, can also be used to determine the appropriate output when test cases are ran.  
# How route parameters are used in Express
Through the use of route parameters, dynamic routes can be created. By using the ":" (colon) in the URL, followed by a parameter (say, a user's name), the parameter can be stored within the program, allowing for later use. For instance, this program takes in "/user/Donny", for instance, and will return "Hello, Donny" once the destination has been reached.
Also, an empty parameter after "/user" will lead to a 404 page.
