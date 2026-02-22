angularjs-chat
==============

A simple chat application written in AngularJS - using SockJS (not using server-side socket library such as Socket.io).

## Details

I created a NodeJS server for this project. SockJS has implementations for other langugages as well, see https://github.com/sockjs.

### Dependencies

- AngularJS, [sockjs-client](https://github.com/sockjs/sockjs-client)

- NodeJS, [express](expressjs.com), [sockjs-client-node](https://github.com/sockjs/sockjs-node)

- Package managers ([Bower](http://bower.io/), [NPM](https://npmjs.org/)) and finally [Grunt](http://gruntjs.com/)


### SockJS

Taken from its readme:
> SockJS is a browser JavaScript library that provides a WebSocket-like object. SockJS gives you a coherent, cross-browser, Javascript API which creates a low latency, full duplex, cross-domain communication channel between the browser and the web server.

> Under the hood SockJS tries to use native WebSockets first. If that fails it can use a variety of browser-specific transport protocols and presents them through WebSocket-like abstractions.

For more details about the SockJS project, see https://github.com/sockjs/sockjs-client.

### Issues

I am sure you can break the live server (http://angularjs-chat-server.aws.af.cm/), but please, just try not to do that :) This is a simple project to show you how to use AngularJS and SockJS to create interactive applications. 

I tested the application using 2 browsers on the same computer. Sometimes when you quit chat on one browser, the connection on the other browser gets broken. Feel free to fix the issue :)


### Installing Modules

* First you need to install node_modules. Cd to node-server folder.  ``` $cd node-server ```

* Execute ``` $sudo npm install ```

* Then, you need to install dependencies for our Angular application. Cd to angular-app folder.  ``` $cd angular-app ```

* Execute ``` $sudo npm install ```

* And execute ``` $sudo bower install ```


### Running the app

* Change directory to node-server folder  ``` $cd node-server ```

* Start the Node server: ``` $node app ```

* Open another console and cd to angular-app folder  ``` $cd angular-app ```

* Now, you can start the grunt server: ``` $grunt serve ```

* It will open the AngularJS app in your default browser. Have fun :)


