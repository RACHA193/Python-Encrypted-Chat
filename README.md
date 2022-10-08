# Python-Encrypted-Chat

A simple cli based python-encrypted-chat(PEC) room. A small chat room program written in Python 3, that allows multiple people to instant messaging over the internet. It consist of two scripts a server and a client.

__________________________________________________________________________________________________________________________________________________________

# USAGE

>>   Run server.py on the machine you wish to act as the server, entering the desired hostname/IP and port you wish to run the server on. You can run          multiple independent servers, however they must be running on different ports. 
>>   Any clients can now connect to the server by running client.py then entering the IP and port the server is running on (as seen in the server              terminal). Clients can choose a username and then send messages by entering them into the Python terminal. Messages from other clients will be            printed to the Python terminal.
>>   The client and server will generate a keypair if there are none present within their respective keys directory.
>>   After connecting and entering a username, the client and server will perform a public key exchange, all messages sent will be encrypted along the          wire.
>>   The client and server directory have a generated keypair, if you wish to generate your own, simply delete the contents of the keys directory, or the      directory itself.

__________________________________________________________________________________________________________________________________________________________

# KNOWN ISSUES

>>  While using the program as a client, if you are typing a message and receive one at the same time, you may experience some errors with the received       message interrupting the message you are typing. Unfortunately, this is unfixable currently due to Python 3 having issues with printing and accepting     user input at the same time, however this bug is only visual and any typed message will send as normal.
>>  occasionally when connecting the server will read the public key in the username, will have a look into this later. This bug require you restart the       server and client.

__________________________________________________________________________________________________________________________________________________________

# REQUIREMENTS

>>  Python3
>>  Socket Module (standard library)
>>  Threading Module (standard library)
>>  PyCryptodome

__________________________________________________________________________________________________________________________________________________________

