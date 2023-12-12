**Chat Room Program Manual**

**1. Overview:**
   - The chat room program consists of two parts: the server and the client.
   - The server manages connections and broadcasts messages to all connected clients.
   - Each client connects to the server and can send messages to the chat room.

**2. Files:**
   - Server: `Server.java`
   - Client: `Client.java`

**3. How to Run:**
   - Compile both `Server.java` and `Client.java` using a Java compiler.
   - Open two separate command prompt or terminal windows.

**4. Start the Server:**
   - In one window, navigate to the directory containing `Server.class`.
   - Run the command: `java Server`

**5. Connect Clients:**
   - In the other window, navigate to the directory containing `Client.class`.
   - Run the command: `java Client`
   - Repeat step 5 for additional clients.

**6. Client Commands:**
   - After connecting, clients can perform the following commands:
     - `/nick [newNickname]`: Change the nickname.
     - `/quit`: Disconnect from the chat.

**7. Interacting in the Chat:**
   - Type your messages in the client's console and press Enter to send.
   - Messages will be broadcasted to all connected clients.

**8. Nickname Change:**
   - Use the `/nick` command followed by the desired nickname to change your nickname.
   - Example: `/nick NewUser`

**9. Disconnecting:**
   - Use the `/quit` command to disconnect from the chat.
   - The server will broadcast a message when a user leaves the chat.

**10. Notes:**
   - The server listens on port `9999`.
   - Each client connects to the server's IP address (`127.0.0.1` for local testing).
   - The server uses a thread pool to handle multiple client connections concurrently.

**11. Exiting:**
   - To stop the server, press `Ctrl + C` in the window where the server is running.
   - Close the client windows to exit.

**12. Troubleshooting:**
   - If any unexpected errors occur, restart the server and reconnect the clients.
   - Check that the server port (`9999`) is not blocked by a firewall.

**Note:** This chat room is a basic example for learning purposes. It doesn't include security features and may not handle all edge cases. Consider it as a starting point for understanding socket programming in Java.
