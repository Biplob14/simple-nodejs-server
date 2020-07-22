# simple-nodejs-server
This code is the symbol of my node js beginning. 🥳\
Using this code can create a simple localhost server to access in this specific file. 🥴
### 💥Understanding code💥

---
>`var http = require('http');` <br>

To use the HTTP server and client one must require('http')

>`http.createServer()` <br>

Creates HTTP server object. Inside parenthesis holds the request listener function.
>`function (req, res)`

Request Listener function. The function is called each time the server gets a request and passed as a parameter to the http.createServer() method. <br>
Handles requests from the user and also respond to user.

>`res.writeHead(200, {'content-type': 'text/html'});`

First argument contains status code 200 means everything's working properly. Second argument type of object containing the response header. <br>
This lets manipulate the meta-data associated with the response to send to a client from server.

>`res.end('Hello World!');`

Finish sending the request to client.

>`}).listen(8080);`

Start a server listening for connection on port 8080.