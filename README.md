#socketfun-ios
Test-Project for WebSocket connections.
As an testserver you can use the  [socketfun](https://github.com/a0n/socketfun) repo.

This project uses [socket.IO-objc](https://github.com/pkyeck/socket.IO-objc).

To checkout the project:

    git clone
    git submodule init
    git submodule update

or

    git clone --recursive

##Dependencies
[socket.IO-objc](https://github.com/pkyeck/socket.IO-objc) is an interface to communicate between Objective-C and [Socket.IO](http://socket.io/) with the help of websockets and uses

* [cocoa-websocket](https://github.com/erichocean/cocoa-websocket)
* [RegexKitLite](http://regexkit.sourceforge.net/RegexKitLite/)
* [json-framework](https://github.com/stig/json-framework/)
* [ASIHTTPRequest](http://allseeing-i.com/ASIHTTPRequest/)

##Configuration for an own project
###socket.IO-objc
Copy SocketIO.h and Socket.IO.m into your project.

###cocoa-websocket
Copy WebSocket.h and WebSocket.m into your project.

###AsyncSocket
Copy the AsyncSocket files into your project. AsnycSocket is included in cocoa-websocket.

###RegexKitLite
Copy RegexKitLite.h and RegexKitLite.m into your project.
In your project settings in "Build Settings" under "Other Linker Flags" include the value "-licucore".

###json-framework
Copy all files from the classes folder into your project.

###ASIHTTPRequest
Copy all needed files into your project (see the homepage at setup instructions).
In your project configs link with CFNetwork, SystemConfiguration, MobileCoreServices, CoreGraphics and libz.dylib.


##Usaqge
Please see [socket.IO-objc](https://github.com/pkyeck/socket.IO-objc)
