# README


HTTP and Websockets
In HTTP, the connection between the server and the client has a short lifespan: The client requests a resource from the server, a connection with a server is established and the requested resource (be it JSON, HTML, XML or some kind of a file) is streamed to the client as a response. Then, the connection is closed. But how would the client know if the server has new or updated data? Usually, HTTP would use long polling, in which the client would “ask” the server if there is something new in a given interval of time.

Unlike HTTP, WebSockets is protocol that enables the client and the server to keep an open connection, enabling them to directly stream data between each other. The client subscribes to an open websocket connection in the server and when there is new information, the server broadcasts the data and the subscribed clients receive it. This way, both the server and the client know about the state of the data and can easily synchronize changes as they occur.


* Git clone the repo `https://github.com/Mutuba/ActionCableChatApp.git`

* cd into `ActionCableChatApp` and bundle install

* run rails s

* Go to `http://localhost:3000/` on your browser. You should a user interface waiting for you to type a message. On typing and hitting enter key you should see the message at the top as part of your chats.

* In the terminal you will be able to see streams from the channel and job queues.
