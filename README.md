# reverse-engineering-code


In the Develop folder, there is starter code for a project. Begin inspecting the code to get an understanding of each file's responsibility.

Below gives more understanding of files...

----CONFIG----
MIDDLEWARE  
*isAuthenticated.js* {restricts routes that user is not allowed to visit if they are not logged in or a member. Otherwise, it will fulfill the request.}   
*config.json* { the connection configuration to the server}  
*passport.js* {contains the JS logic to tell the passport that a user wants to login with an email and password}   

----MODELS----  
*index.js* { connects the db and imports the user login credentials}  
*user.js* { requires "bcrypt" for hiding the password. This makes the db secure. Also, defines the JS of what is stored in the database.};   

----ROUTES---- 
*api-routes.js* { contains the routes for signing in or logging out. Grabs specific user data to be displayed.};  
*html-routes.js* { Routes to check whether or not a user is signed in and sends them to the correct page.};  
*package.json* {contains the package info and modules needed for the project.};  
*server.js* { requires packages, enables the PORT, creates express and middleware, creates the routes and syncs the db. Logs messages to the terminal when successfully connected.};  
