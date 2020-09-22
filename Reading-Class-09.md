# Using Express Routing
https://expressjs.com/en/guide/routing.html

* *routing* is how endpoints respond to client requests
  * we use the **app** object with HTTP methods to handle requests
* this all seems pretty confusing at the moment. This page has a lot of good reference code.

# Supertest
https://github.com/visionmedia/supertest

* This is a link to the github repo for supertest
* supertest is high-level testing for HTTP
* tests look the same as in superagent
* expectations are run in the order of definition

# Using Express Middleware
https://expressjs.com/en/guide/using-middleware.html

* express applications are basically a series of middleware function calls
* middleware functions have access the the req object, res object and the next function
* they can:
  -execute code
  -make changes to req and res
  -end the req, res cycle
  -call the next function in the stack

# Express Middleware
https://www.tutorialspoint.com/expressjs/expressjs_middleware.htm

* *app.use()* restricts the middleware call to a specific route
* there's a lot of third party middleware for Express that can be found: http://expressjs.com/en/resources/middleware.html

# Express Middleware List
https://expressjs.com/en/resources/middleware.html

* cors is one of these
