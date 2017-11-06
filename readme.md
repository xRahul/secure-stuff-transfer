## Secure Stuff Transfer

![Heroku](https://heroku-badge.herokuapp.com/?app=heroku-badge)

Plan is to create a secure data transfer tool at the end.

Current Implementation:
* A basic chatroom web app following tutorial: https://www.callicoder.com/spring-boot-websocket-chat-example/

Next Planned:
* Adding public/private keys in JS to secure chats end-to-end.
  * Each user who joins the chatroom will have a public/private key value pair.
  * On joining the chatroon, public key along with username will be sent to the server for storage.
  * Whenever a new user joins, they will get the complete list of users and their public keys.
  * When sending a chat, that chat will be individually encrypted for each user with their public keys and sent to the server.
  * The server then sends that payload to the channel and each user will decrypt the chat by their private key and it will be displayed to them.
  * The payload will have a tag signifying it's a public chat for the entire chatroom
  
Further Iteration:
* Adding private chat support.
* Using the framework to send other type of data.
