# Char-Room
a simple unencrypted instant messenger: BasicIM.  BasicIM consists of two parts: a single instance of a server (server.py) and a variable number of BasicIM clients (client.py).  Each client connects to the server, the latter of which is responsible for receiving instant messages from a client and echoing those messages to all other connected clients.  (The client that sent the message doesn't receive a copy of it.)  In other words, BasicIM provides group chat, similar to IRCLinks to an external site., and uses TCP socketsLinks to an external site. to communicate.

messages and nicknames will be encrypted using an encrypt-then-MAC scheme, with AES-256 (AES with 256-bit keys) in CBC mode 
and an HMAC backed by SHA-256.
