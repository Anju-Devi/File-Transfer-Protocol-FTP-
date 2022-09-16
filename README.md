# File-Transfer-Protocol-FTP-
FTP is a client-server protocol that relies on two communications channels between the client and server: a command channel for controlling the conversation and a data channel for transmitting file content.  Here is how a typical FTP transfer works:  A user typically needs to log on to the FTP server, although some servers make some or all of their content available without a login, a model known as anonymous FTP. The client initiates a conversation with the server when the user requests to download a file. Using FTP, a client can upload, download, delete, rename, move and copy files on a server.


Algorithm: 
1. The server starts and waits for filename.
2. The client sends a filename.
3. The server receives filename.
   If file is present,
   server starts reading file 
   and continues to send a buffer filled with
   file contents encrypted until file-end is reached.
4. End is marked by EOF.
5. File is received as buffers until EOF is 
received. Then it is decrypted.
6. If Not present, a file not found is sent.
