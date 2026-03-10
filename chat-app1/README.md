# Simple Java Chat App
**Author:** Ayantu LG

## What is this project?
This is a basic communication tool built with Java. It allows two computers (a Server and a Client) to send text messages to each other over a network.

## How it works (My Analysis)
After reviewing the code, here is how the connection works:
1. **Server Side:** The server opens a "gate" (Port 4141) and waits for a connection.
2. **Client Side:** The client connects to that specific port to start talking.
3. **1-to-1 Limit:** The code uses a simple loop that handles **one client at a time**. While the server can accept a new person after the first one leaves, it does not support a "group chat" where everyone talks at once.