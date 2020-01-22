# Node.js Interview Questions and Answers

Node.js lets developers use JavaScript for server-side scripting—running scripts server-side to produce dynamic web page content before the page is sent to the user's web browser. Don't go to your next Nodejs interview without checking that list of most advanced Node js interview questions that may get you your next full stack developer job offer!

> You could also find all the answers here 👉 https://www.fullstack.cafe/Node.js.

## Q1: What is Node.js? ⭐

**Answer:**

Node.js is a web application framework built on Google Chrome's JavaScript Engine (V8 Engine).

Node.js comes with runtime environment on which a Javascript based script can be interpreted and executed (It is analogus to JVM to JAVA byte code). This runtime allows to execute a JavaScript code on any machine outside a browser. Because of this runtime of Node.js, JavaScript is now can be executed on server as well.

*Node.js = Runtime Environment + JavaScript Library*

🔗 **Source:** [tutorialspoint.com](http://www.tutorialspoint.com/nodejs/nodejs_interview_questions.htm)


## Q2: What is npm? ⭐

**Answer:**

`npm` stands for Node Package Manager. npm provides following two main functionalities:

*   Online repositories for node.js packages/modules which are searchable on [search.nodejs.org](http://search.nodejs.org)
*   Command line utility to install packages, do version management and dependency management of Node.js packages.

🔗 **Source:** [tutorialspoint.com](http://www.tutorialspoint.com/nodejs/nodejs_interview_questions.htm)


## Q3: What are the two types of API functions in Node.js?  ⭐

**Answer:**

The two types of API functions in Node.js are: a) Asynchronous, non-blocking functions b) Synchronous, blocking functions

🔗 **Source:** [lazyquestion.com](http://www.lazyquestion.com/interview-questions-and-answer/nodejs)


## Q4: What do you mean by Asynchronous API? ⭐⭐

**Answer:**

All APIs of Node.js library are aynchronous that is non-blocking. It essentially means a Node.js based server never waits for a API to return data. Server moves to next API after calling it and a notification mechanism of Events of Node.js helps server to get response from the previous API call.

🔗 **Source:** [tutorialspoint.com](http://www.tutorialspoint.com/nodejs/nodejs_interview_questions.htm)


## Q5: What are the benefits of using Node.js? ⭐⭐

**Answer:**

Following are main benefits of using Node.js

*   **Aynchronous and Event Driven** - All APIs of Node.js library are aynchronous that is non-blocking. It essentially means a Node.js based server never waits for a API to return data. Server moves to next API after calling it and a notification mechanism of Events of Node.js helps server to get response from the previous API call.
*   **Very Fast** - Being built on Google Chrome's V8 JavaScript Engine, Node.js library is very fast in code execution.
*   **Single Threaded but highly Scalable** - Node.js uses a single threaded model with event looping. Event mechanism helps server to respond in a non-bloking ways and makes server highly scalable as opposed to traditional servers which create limited threads to handle requests. Node.js uses a single threaded program and same program can services much larger number of requests than traditional server like Apache HTTP Server.
*   **No Buffering** \- Node.js applications never buffer any data. These applications simply output the data in chunks.

🔗 **Source:** [tutorialspoint.com](http://www.tutorialspoint.com/nodejs/nodejs_interview_questions.htm)


## Q6: Is Node a single threaded application? ⭐⭐

**Answer:**

Yes! Node uses a single threaded model with event looping.

🔗 **Source:** [tutorialspoint.com](http://www.tutorialspoint.com/nodejs/nodejs_interview_questions.htm)


## Q7: What is global installation of dependencies? ⭐⭐

**Answer:**

Globally installed packages/dependencies are stored in **<user-directory>**/npm directory. Such dependencies can be used in CLI (Command Line Interface) function of any node.js but can not be imported using require() in Node application directly. To install a Node project globally use -g flag.

🔗 **Source:** [tutorialspoint.com](http://www.tutorialspoint.com/nodejs/nodejs_interview_questions.htm)


## Q8: What is an error-first callback? ⭐⭐

**Answer:**

*Error-first callbacks* are used to pass errors and data. The first argument is always an error object that the programmer has to check if something went wrong. Additional arguments are used to pass data.

```js
fs.readFile(filePath, function(err, data) {
  if (err) {
    //handle the error
  }
  // use the data object
});
```

🔗 **Source:** [tutorialspoint.com](http://www.tutorialspoint.com/nodejs/nodejs_interview_questions.htm)


## Q9: What's the difference between operational and programmer errors? ⭐⭐

**Answer:**

Operation errors are not bugs, but problems with the system, like _request timeout_ or _hardware failure_. On the other hand programmer errors are actual bugs.

🔗 **Source:** [blog.risingstack.com](https://blog.risingstack.com/node-js-interview-questions/)


## Q10: What is the difference between Nodejs, AJAX, and jQuery? ⭐⭐

**Answer:**

The one common trait between Node.js, AJAX, and jQuery is that all of them are the advanced implementation of JavaScript. However, they serve completely different purposes.

* Node.js –It is a server-side platform for developing client-server applications. For example, if we’ve to build an online employee management system, then we won’t do it using client-side JS. But the Node.js can certainly do it as it runs on a server similar to Apache, Django not in a browser.

* AJAX (aka Asynchronous Javascript and XML) –It is a client-side scripting technique, primarily designed for rendering the contents of a page without refreshing it. There are a no. of large companies utilizing AJAX such as Facebook and Stack Overflow to display dynamic content.

* jQuery –It is a famous JavaScript module which complements AJAX, DOM traversal, looping and so on. This library provides many useful functions to help in JavaScript development. However, it’s not mandatory to use it but as it also manages cross-browser compatibility, so can help you produce highly maintainable web applications.

🔗 **Source:** [techbeamers.com](http://www.techbeamers.com/top-30-node-js-interview-questions-answers/)


## Q11: How to make Post request in Node.js? ⭐⭐

**Answer:**

Following code snippet can be used to make a Post Request in Node.js.

```js
var request = require('request');
request.post('http://www.example.com/action', {
  form: {
    key: 'value'
  }
}, function(error, response, body) {
  if (!error && response.statusCode == 200) {
    console.log(body)
  }
});
```

🔗 **Source:** [techbeamers.com](http://www.techbeamers.com/top-30-node-js-interview-questions-answers/)


## Q12: What are the key features of Node.js? ⭐⭐

**Answer:**

Let’s look at some of the key features of Node.js.

*   **Asynchronous event driven IO helps concurrent request handling –** All APIs of Node.js are asynchronous. This feature means that if a Node receives a request for some Input/Output operation, it will execute that operation in the background and continue with the processing of other requests. Thus it will not wait for the response from the previous requests.
*   **Fast in Code execution –** Node.js uses the V8 JavaScript Runtime engine, the one which is used by Google Chrome. Node has a wrapper over the JavaScript engine which makes the runtime engine much faster and hence processing of requests within Node.js also become faster.
*   **Single Threaded but Highly Scalable –** Node.js uses a single thread model for event looping. The response from these events may or may not reach the server immediately. However, this does not block other operations. Thus making Node.js highly scalable. Traditional servers create limited threads to handle requests while Node.js creates a single thread that provides service to much larger numbers of such requests.
*   **Node.js library uses JavaScript –** This is another important aspect of Node.js from the developer’s point of view. The majority of developers are already well-versed in JavaScript. Hence, development in Node.js becomes easier for a developer who knows JavaScript.
*   **There is an Active and vibrant community for the Node.js framework –** The active community always keeps the framework updated with the latest trends in the web development.
*   **No Buffering –** Node.js applications never buffer any data. They simply output the data in chunks.

🔗 **Source:** [techbeamers.com](http://www.techbeamers.com/top-30-node-js-interview-questions-answers/)


## Q13: What is control flow function?   ⭐⭐

**Answer:**

It is a generic piece of code which runs in between several asynchronous function calls is known as control flow function.

🔗 **Source:** [lazyquestion.com](http://www.lazyquestion.com/interview-questions-and-answer/nodejs)


## Q14: What are Event Listeners?   ⭐⭐

**Answer:**

**Event Listeners** are similar to call back functions but are associated with some event. For example when a server listens to http request on a given port a event will be generated and to specify http server has received and will invoke corresponding event listener. Basically, Event listener's are also call backs for a corresponding event.

Node.js has built in event's and built in event listeners. Node.js also provides functionality to create Custom events and Custom Event listeners.

🔗 **Source:** [lazyquestion.com](http://www.lazyquestion.com/interview-questions-and-answer/nodejs?page=3)


## Q15: If Node.js is single threaded then how it handles concurrency? ⭐⭐

**Answer:**

Node provides a single thread to programmers so that code can be written easily and without bottleneck. Node internally uses multiple POSIX threads for various I/O operations such as File, DNS, Network calls etc.

When Node gets I/O request it creates or uses a thread to perform that I/O operation and once the operation is done, it pushes the result to the event queue. On each such event, event loop runs and checks the queue and if the execution stack of Node is empty then it adds the queue result to execution stack.

This is how Node manages concurrency.

🔗 **Source:** [codeforgeek.com](https://codeforgeek.com/2017/08/node-js-interview-questions-answers-updated/)


## Q16: What is Callback Hell? ⭐⭐

**Answer:**

The asynchronous function requires callbacks as a return parameter. When multiple asynchronous functions are chained together then callback hell situation comes up. 

🔗 **Source:** [codeforgeek.com](https://codeforgeek.com/2017/08/node-js-interview-questions-answers-updated/)


## Q17:  List out the differences between AngularJS and NodeJS? ⭐⭐

**Answer:**

AngularJS is a web application development framework. It’s a JavaScript and it is different from other web app frameworks written in JavaScript like jQuery. NodeJS is a runtime environment used for building server-side applications while AngularJS is a JavaScript framework mainly useful in building/developing client-side part of applications which run inside a web browser.

🔗 **Source:** [a4academics.com](http://a4academics.com/interview-questions/79-web/802-nodejs-interview?showall=&start=2)


## Q18: Could we run an external process with Node.js? ⭐⭐

**Answer:**

Yes. *Child process module* enables us to access operating system functionaries or other apps. Scalability is baked into Node and child processes are the key factors to scale our application. You can use child process to run system commands, read large files without blocking event loop,  decompose the application into various “nodes” (That’s why it’s called Node).

Child process module has following three major ways to create child processes –

* spawn  - child_process.spawn launches a new process with a given command.
* exec  - child_process.exec method runs a command in a shell/console and buffers the output.
* fork - The child_process.fork method is a special case of the spawn() to create child processes.

🔗 **Source:** [codeforgeek.com](https://codeforgeek.com/2017/08/node-js-interview-questions-answers-updated/)


## Q19:  How you can monitor a file for modifications in Node.js ? ⭐⭐

**Answer:**

We can take advantage of File System `watch()` function which watches the changes of the file.

🔗 **Source:** [codingdefined.com](https://www.codingdefined.com/2017/04/top-20-interview-questions-on-nodejs.html)


## Q20: What are the core modules of Node,js? ⭐⭐

**Answer:**

* EventEmitter
* Stream
* FS
* Net
* Global Objects

🔗 **Source:** [github.com/jimuyouyou](https://github.com/jimuyouyou/node-interview-questions)


## Q21: What is V8? ⭐⭐

**Answer:**

The V8 library provides Node.js with a JavaScript engine (a program that converts Javascript code into lower level or machine code that microprocessors can understand), which Node.js controls via the V8 C++ API. V8 is maintained by Google, for use in Chrome.

The Chrome V8 engine :

* The V8 engine is written in C++ and used in Chrome and Nodejs.
* It implements ECMAScript as specified in ECMA-262.
* The V8 engine can run standalone we can embed it with our own C++ program.



🔗 **Source:** [nodejs.org](https://nodejs.org/en/docs/meta/topics/dependencies/)


## Q22: What is libuv? ⭐⭐

**Answer:**

**libuv** is a C library that is used to abstract non-blocking I/O operations to a consistent interface across all supported platforms. It provides mechanisms to handle file system, DNS, network, child processes, pipes, signal handling, polling and streaming. It also includes a thread pool for offloading work for some things that can't be done asynchronously at the operating system level.

🔗 **Source:** [nodejs.org](https://nodejs.org/en/docs/meta/topics/dependencies/)


## Q23: What is the difference between returning a callback and just calling a callback? ⭐⭐

**Answer:**

```js
return callback();
//some more lines of code; -  won't be executed

callback();
//some more lines of code; - will be executed
```

Of course returning will help the context calling async function get the value returned by callback.
```js
function do2(callback) {
    log.trace('Execute function: do2');
    return callback('do2 callback param');
}

var do2Result = do2((param) => {
    log.trace(`print ${param}`);
    return `return from callback(${param})`; // we could use that return
});

log.trace(`print ${do2Result}`);
```
Output:
```sh
C:\Work\Node>node --use-strict main.js
[0] Execute function: do2
[0] print do2 callback param
[0] print return from callback(do2 callback param)
```

🔗 **Source:** [stackoverflow.com](https://stackoverflow.com/questions/43075181/nodejs-what-is-the-difference-between-return-callback-and-just-callback)


## Q24: What is REPL in context of Node? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q25: What is Callback? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q26: What is a blocking code? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q27: How Node prevents blocking code? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q28: What is Event Loop? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q29: What is Event Emmitter? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q30: What is purpose of Buffer class in Node? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q31: What is difference between synchronous and asynchronous method of fs module? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q32: What are streams? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q33: What is Chaining in Node? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q34: What is the purpose of setTimeout function? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q35: How can you avoid callback hells? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q36: What's the event loop? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q37: How to avoid callback hell in Node.js? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q38: Explain how does Node.js work? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q39: When should we use Node.js? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q40: How does Node.js handle child threads? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q41: What is the preferred method of resolving unhandled exceptions in Node.js? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q42: What is stream and what are types of streams available in Node.js? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q43: What are the global objects of Node.js? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q44: How to use Buffer in Node.js? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q45: When should I use EventEmitter? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q46: How do you debug Node.js applications? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q47: Rewrite promise-based Node.js applications to Async/Await ⭐⭐⭐

**Questions Details:**

Rewrite this code to Async/Await:
```js
function asyncTask() {
    return functionA()
        .then((valueA) => functionB(valueA))
        .then((valueB) => functionC(valueB))
        .then((valueC) => functionD(valueC))
        .catch((err) => logger.error(err))
}
```



 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q48: What is the relationship between Node.js and V8? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q49: What is N-API in Node.js? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q50: Explain the concept of Domain in Node.js ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q51: Are you familiar with differences between Node.js nodules and ES6 nodules? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q52: What are the use cases for the Node.js "vm" core module? ⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q53: What is Piping in Node? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q54: Name some of the events fired by streams. ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q55: What is the purpose of __filename variable? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q56: How can you listen on port 80 with Node? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q57: What tools can be used to assure consistent code style? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q58: What's a stub? Name a use case. ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q59: Does Node.js support multi-core platforms? And is it capable of utilizing all the cores? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q60: Is Node.js entirely based on a single-thread? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q61: Is Node.js entirely based on a single-thread? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q62: When to not use Node.js? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q63: Why to use Buffers instead of binary strings to handle binary data ? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q64: How to gracefully Shutdown Node.js Server? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q65: What are the timing features of Node.js? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q66: Explain usage of NODE_ENV ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q67: What is LTS releases of Node.js why should you care? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q68: Provide some example of config file separation for dev and prod environments ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q69: How would you handle errors for async code in Node.js? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q70: What's the difference between dependencies, devDependencies and peerDependencies in npm package.json file? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q71: How do you convert an existing callback API to promises? ⭐⭐⭐⭐

**Questions Details:**

How to convert this callback code to Promise? Provide some examples.
```js
function divisionAPI (number, divider, successCallback, errorCallback) {
    if (divider == 0) {
        return errorCallback( new Error("Division by zero") )
    }
    successCallback( number / divider )
}
```


 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q72: What are async functions in Node? Provide some examples. ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q73: Can Node.js work without V8? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q74: How the V8 engine works? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q75: How does the cluster module work? What’s the difference between it and a load balancer? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q76: Is it possible to use "Class" in Node.js? ⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q77: Consider following code snippet ⭐⭐⭐⭐⭐

**Questions Details:**

Consider following code snippet:

```js
{
  console.time("loop");
  for (var i = 0; i < 1000000; i += 1) {
    // Do nothing
  }
  console.timeEnd("loop");
}
```

The time required to run this code in Google Chrome is considerably more than the time required to run it in Node.js Explain why this is so, even though both use the v8 JavaScript Engine.


 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q78: Can Node.js use other engines than V8? ⭐⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q79: How would you scale Node application? ⭐⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q80: What is the difference between process.nextTick() and setImmediate() ? ⭐⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q81: How to solve "Process out of Memory Exception" in Node.js ? ⭐⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q82: Explain what is Reactor Pattern in Node.js? ⭐⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q83: Explain some Error Handling approaches in Node.js you know about. Which one will you use? ⭐⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q84: Why should you separate Express 'app' and 'server'? ⭐⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q85: Rewrite the code sample without try/catch block ⭐⭐⭐⭐⭐

**Questions Details:**

Consider the code:
```js
async function check(req, res) {
  try {
    const a = await someOtherFunction();
    const b = await somethingElseFunction();
    res.send("result")
  } catch (error) {
    res.send(error.stack);
  }
}
```
Rewrite the code sample without try/catch block.


 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q86: How many threads does Node actually create? ⭐⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q87: What is the purpose of using hidden classes in V8? ⭐⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q88: How V8 compiles JavaScript code? ⭐⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q89: How does libuv work under the hood? ⭐⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q90: What is V8 Templates? ⭐⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q91: Why do we need C++ Addons in Node.js? ⭐⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q92: Why Node.js devs tend to lean towards the Module Requiring vs Dependency Injection? ⭐⭐⭐⭐⭐

 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q93: Explain the result of this code execution ⭐⭐⭐⭐⭐

**Questions Details:**

Explain the result of that code execution:

```js
var EventEmitter = require("events");

var crazy = new EventEmitter();

crazy.on('event1', function () {
    console.log('event1 fired!');
    crazy.emit('event2');
});

crazy.on('event2', function () {
    console.log('event2 fired!');
    crazy.emit('event3');

});

crazy.on('event3', function () {
    console.log('event3 fired!');
    crazy.emit('event1');
});

crazy.emit('event1');
```


 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q94: Explain the result of this code execution ⭐⭐⭐⭐⭐

**Questions Details:**

Explain the result of this code execution
```js
var EventEmitter = require('events');

var crazy = new EventEmitter();

crazy.on('event1', function () {
    console.log('event1 fired!');
    setImmediate(function () {
        crazy.emit('event2');
    });
});

crazy.on('event2', function () {
    console.log('event2 fired!');
    setImmediate(function () {
        crazy.emit('event3');
    });

});

crazy.on('event3', function () {
    console.log('event3 fired!');
    setImmediate(function () {
        crazy.emit('event1');
    });
});

crazy.emit('event1');
```


 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**


## Q95: What will happen when that code will be executed? ⭐⭐⭐⭐⭐

**Questions Details:**


What will happen when that code will be executed?
```js
var EventEmitter = require('events');

var crazy = new EventEmitter();

crazy.on('event1', function () {
    console.log('event1 fired!');
    process.nextTick(function () {
        crazy.emit('event2');
    });
});

crazy.on('event2', function () {
    console.log('event2 fired!');
    process.nextTick(function () {
        crazy.emit('event3');
    });

});

crazy.on('event3', function () {
    console.log('event3 fired!');
    process.nextTick(function () {
        crazy.emit('event1');
    });
});

crazy.emit('event1');
```


 See 👉 **[Answer](https://www.fullstack.cafe/Node.js)**
