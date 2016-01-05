## Instructions:
Fork and clone this repo.  Then submit a pull request with all of the bad answers deleted and only the correct answers showing.

#### 1.  Which browser does Node share a runtime with?

* E) All javascript enabled browsers


#### 2.  Which of the following code in a js file will include a core module named 'fs' ?   

* D) require('fs')


#### 3.  The below code is an attempt to run a simple Node.js server. The server fails to start. Without seeing the server error message, what can you fix in the code to make the server run ?

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

* H) change *text/plain* to *text/html*


###4. Consider the following code from boxes.js , which is required by another file.  What **DATA TYPE** type will be returned from module.exports in this file?
```
var boxes = ["cardboard", "plastic", "metal"]

module.exports = function(){
  return boxes;
}

```


* C) an array


###5. What do we mean when we say that Node has a non-blocking IO model ?  (free response) . Give an example from class if you can remember it, or any other example of how this can work.

Non-blocking IO(input output) refers to an asynchronous flow.  It will not get hung up on processes that a synchronous process would.  
An example would be if there is a large ajax call happening as well as a small ajax call happening, it will not make the process wait for the larger one to finish, it will load both and display them as they are completed.  Nmuta's example refered to tell the color and information of every pen in a class handed out to each student as well as just give a black pen to the person on your left.  The shorter process (hand pen to person on left) could carry out prior to the larger process finishing.  
