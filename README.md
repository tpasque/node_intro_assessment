## 1.  Which browser does Node share a runtime with?
* A) V8
* B) All browsers
* C) Chrome
* D) both A and C 
* E) All javascript enabled browsers
* F) Firefox
* G) None of the above

## 2.  Which of the following code in a js file will include a core module named 'fs' ?   
* A) npm install fs 
* B) include('./fs')
* C) require('./fs')
* D) require('fs')
* E) node fs
* F) include(fs)
* G) include('fs')

```
var http = require('http');

function showTime(req, res) {
  res.setHeader("Content-Type", "text/plain");
  res.statusCode = 404;
  res.write("<h1>Hello</h1> citizen, if you are here");
  res.end();
};

var server = http.createServer(res);

http.listen(8000, function() {
	console.log("I'm listening on port 8000...")
});

```

## 3.  The above code is an attempt to run a simple Node.js server. The server fails to start. Without seeing the server error message, what can you fix in the code to make the server run ? 

* A) change *require('http')* to *include('http')*
* B) change *var http* to simply *http* 
* C) change *function showTime(req, res)* to *function handleRequest(req, res)*
* D) change *res.statusCode = 404*  to *res.statusCode = 200* 
* E) change *http.listen* to  *server.listen* only 
* F) change *http.createServer(res)* to  *http.createServer(showTime)* only 
* G) change *http.createServer(res)* to  *http.createServer(showTime)* and change *http.listen* to *server.listen*
* H) change *text/plain* to *text/html*
* I) none of the above
