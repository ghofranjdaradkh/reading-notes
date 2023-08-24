


## What are the five steps in the HTTP Request Lifecycle?

Local Processing: The client (usually a browser) extracts the relevant components from the URL, such as the protocol, host, optional port, resource path, and query strings. It may also check its cache and various caches (e.g., DNS cache) for the IP address of the host.

Resolve an IP: If the IP address is not found in the cache, the client sends a DNS request to resolve the IP address of the host. This involves a series of DNS server lookups, recursive requests, and responses to obtain the target IP address.

Establish a TCP Connection: The client establishes a TCP connection with the server using a three-way handshake. This involves a SYN packet from the client, SYN-ACK packet from the server, and an ACK packet from the client, resulting in an established connection.

Send an HTTP Request: With the TCP connection established, the client sends an HTTP request to the server. The request consists of a request line, headers, and an optional body, containing information about the desired resource and other details.

Tearing Down and Cleaning Up: Once the server responds with the HTTP response, both client and server exchange FIN (finish) and ACK (acknowledge) packets to gracefully close the TCP connection. This four-way handshake marks the end of the connection.

---------------------------------------------------------------------------------------


## What are the two things the client needs before it can make an HTTP Request?

IP Address: The client needs the IP address of the server it wants to communicate with. This IP address is obtained through DNS resolution, which involves converting the human-readable domain name (e.g., www.example.com) into an IP address.

TCP Connection: After obtaining the IP address, the client establishes a TCP connection with the server. This involves a three-way handshake, where the client and server exchange SYN (synchronize) and ACK (acknowledge) packets to establish a reliable connection.


---------------------------------------------------------------------------------------
 ## Explain the four way handshake and what it does.:

The client sends a FIN packet to the server, indicating it has finished sending data.
The server acknowledges the client's FIN with an ACK packet, confirming the receipt of the FIN.
The server sends its own FIN packet to the client, indicating it has finished sending data.
The client acknowledges the server's FIN with another ACK packet.


---------------------------------------------------------------------------------------

## True or False: When making an HTTP request, you MUST follow any redirect returned by the request. Back up your answer.


False. While HTTP requests generally follow redirects automatically (unless disabled), it's not mandatory to follow redirects. 
The decision to follow a redirect is often based on the configuration of the HTTP client or the specific needs of the application.
---------------------------------------------------------------------------------------

 ## Which built-in Java class can be used to perform an HTTP request?

The HttpUrlConnection class allows us to perform basic HTTP requests without the use of any additional libraries.
All the classes that we need are part of the java.net package.

---------------------------------------------------------------------------------------
## What HTTP status codes represent a successful response? A redirect? A client error?

successful response status : codes are part of the HTTP specification and typically start with "2" (e.g., 200, 201, 204).

redirect : when a request returns a status code 301 or 302, indicating a redirect, we can retrieve the Location header and create a new request to the new URL.

A client error : If the HTTP status code is greater than 299, it indicates a client error or a server error.

---------------------------------------------------------------------------------------