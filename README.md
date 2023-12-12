# Group Chat Project in Java using Socket

This is a simple group chat application that allows multiple users to communicate with each other in real time over a network. It uses Java sockets and threads to establish connections and exchange messages between a server and multiple clients.

## How it works

- The server class creates a `ServerSocket` object that listens for incoming connections from clients on a specified port.
- The client class creates a `Socket` object that connects to the server on the same port.
- The thread class implements the `Runnable` interface and overrides the `run` method. This class handles the reading and writing of messages between the server and the clients.
- The server creates an `ExecutorService` object to manage a pool of threads. For each client connection, it creates a new thread object and executes it using the `ExecutorService`.
- The client creates two thread objects, one for reading messages from the server and one for writing messages to the server. It starts both threads using the `start` method.
- The thread class uses a loop to read and write messages until a termination condition is met, such as typing "exit" or "bye". It closes the socket and the streams when the communication is over.

## How to run

- First create two separate projects in Netbeans. Add client in one and server in other.
- Run the Server.java file in Server project to initiate the server.
- Run the register_UI.java file to open a user registration popup.
- Enter your name and click "Register" to join the chat.
- Repeat the above steps for each client you want to add to the chat.
- Start typing messages in the terminal and press "Enter" to send them to the group.
- Type "exit" or "bye" to leave the chat.

## References

- [A Group chat application in Java](^5^)
- [Create a chat app with java sockets](^6^)

Source: Conversation with Bing, 12/12/2023
(1) A Group chat application in Java - GeeksforGeeks. https://www.geeksforgeeks.org/a-group-chat-application-in-java/.
(2) Create a chat app with java sockets | by Jihen Barhoumi - Medium. https://medium.com/nerd-for-tech/create-a-chat-app-with-java-sockets-8449fdaa933.
(3) How to Write a Good README File for Your GitHub Project - freeCodeCamp.org. https://www.freecodecamp.org/news/how-to-write-a-good-readme-file/.
(4) Creating a project - GitHub Docs. https://docs.github.com/en/issues/planning-and-tracking-with-projects/creating-projects/creating-a-project.
(5) Hello World - GitHub Docs. https://docs.github.com/en/get-started/quickstart/hello-world.
(6) What Is Project Description: Key Criteria and Steps - KnowledgeHut. https://www.knowledgehut.com/blog/project-management/what-is-project-description.
(7) mohsinht/Group-Chat-System-in-Java - GitHub. https://github.com/mohsinht/Group-Chat-System-in-Java.
(8) GitHub - deysarkarswarup/ChitChat: A simple group chat Application .... https://github.com/deysarkarswarup/ChitChat.
