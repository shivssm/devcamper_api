<!-- middleware -->

Middleware is a function that has access to the request response cycle and runs during that cycle and you can actually set request variables and you can do all types of stuff.

If we set variable in our middleware on the request object, we have access to that thoughout

Example:

1. Middleware that logs on console in every api call
   console.log(
   `${req.method} ${req.protocol}://${req.get('host')}${req.originalUrl}`
   );

Third party logger - Morgan
With this we can do a lot more, like log the request, the method and stuff like that.
install - npm i morgan
