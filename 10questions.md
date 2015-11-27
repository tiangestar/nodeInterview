1. What is Nodejs

Nodejs is a platform for building fast, scalable network application. Its advantages over other server side languages is that it uses event-driven, non-blocking I/O model that makes it light-weight and efficient.

2. Can you explain how Nodejs works

It uses Google V8 Javascript engine to execute code. It contains built-in asynchronous I/O library for file, socket and HTTP communication. Node.js encapsulates libuv to handle asynchronous events.

Also Read : 5 Interview Questions on Node.js

3. Is Nodejs really Single-Threaded

Node.js operates on single-thread, but using non-blocking I/O calls allows it to support many concurrent connections. That means node doen't process the requests in parallel but all the back-end stuffs which actually takes lot of time run in parallel.

4. Can you explain the Asynchronous approach in Nodejs

Nodejs operats asynchronously using event loop and callback functions.An Event Loop is a functionality which handles and processes all your external events and just converts them to a callback function. It invokes all your event handlers at a proper time. So, that means while executing a single request, it does a lot of things in the back-end so that the current request or the coming request doesn't take much time.

You can read more here - Asynchronous approach in Nodejs

5. Can you explain what is Globals in Nodejs

Global, Process and Buffer are combinedly termed as Globals.

Global : Its a global namespace object
Process : Its also a global object but it provides essential functionality to transform a synchronous function into a asynchronous callback.
Buffer : Raw data is stored in instances of the Buffer class.

You can read more here - Globals in Nodejs

6. What is the Use of underscore in Nodejs?

To access the last expression, we have to use the (_) underscore/underline character.

You can read more here - Use of Underscore (_) in Nodejs

7. Can you create Http Server in Nodejs, explain with code

Yes, we can create Http Server in Nodejs. We can use http-server command to do so.

Code :

var http = require('http');
var requestListener = function (request, response) {
  response.writeHead(200, {'Content-Type': 'text/plain'});
  response.end('Hello You\n');
}

var server = http.createServer(requestListener);
server.listen(8080); // The port where you want to start with.

8. How to load HTML in Nodejs

To load HTML in Nodejs we have to change the Content-type from text/plain to text/html.

You can read more here - Loading HTML in NodeJS

9. Can you explain the difference between Node.js vs Ajax

The difference between Node.js and Ajax is that Ajax is a client side technology whereas Nodejs is server side technology. Ajax is used for updating the contents of the page without refreshing it whereas Nodejs is used for developing server software. Nodejs is executed by the server whereas Ajax is executed by the browser.

10. Can you explain the difference between readFile vs createReadStream in Nodejs

readFile - It will read the file completely into memory before making it available to the User.

createReadStream - It will read the file in chunks of the size which is specified before hand.

You can read more here - readFile vs createReadStream in Nodejs

Please Like and Share the Blog, if you find it interesting and helpful.