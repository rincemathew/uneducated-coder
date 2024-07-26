

What is express?


Minimal and flexible web framework for Node.js
Used for building server-side web applications and APIs
the most popular framework for Node
Simplifies the process of handling HTTP requests and responses.
Express is a very fast and unopinionated framework
express is a framework build top of nodejs http module.



opinonated                                      vs            unopinionated
suggested ways to do things                                   Different ways to do the same things
usually offer a lot of bells and whistles                     Including the bare necessities
strict folder structure                                       Structure folders how you want
eg:larvel,django,ruby on rails                                eg:express, flask, 


Express.js
Its a popular node.js web application framework which provides robust set of features for building web and mobile applications
Features : faster server side application development
Middleware
Routing
Template engine
Debugging 

Middleware
Middleware functions are functions that have access to the request object, the response object, and the next middleware function in the application request-response cycle.
1. Application-level middleware
app.use(name)
2. Third party middleware
3.Router-level middleware
router.route()
4.build-in middleware
5.Error-handling middleware


Route Path: The route path is sent as the first parameter. It is in the form of a URL that will be matched with the URL of the HTTP request received by the server. In this case, we are using a route path: /, which is the root of our website. This route will match GET requests sent from URL: localhost:3000. Instead of using fixed URLs, we can also use string patterns, or regular expressions to define route paths.
Handler Function: The second parameter is a function with two arguments: request, and response, also called the Handler Function. The first argument of the handler function: request represents the HTTP request that was sent to the server. We can use this object to extract information about the HTTP request like request headers, and request parameters sent as a query string, path parameters, request body, etc. The second argument: response represents the HTTP response that we will be sending back to the client.




Application-level middleware which runs for all routes in an app object
Router level middleware which runs for all routes in a router object
Built-in middleware provided by Express like express.static, express.json, express.urlencoded
Error handling middleware for handling errors
Third-party middleware maintained by the community

