Web Basics & HTTP Observation

Today's bjective:
The objective of this task was to understand how a web browser communicates with a web server and observe HTTP requests and responses using Developer Tools.

Website which I observed :
I opened the Google homepage in the browser and used the Developer Tools (Network tab) to observe the communication between the browser and the server.

-> Observed Request:

I observed multiple GET requests being made when the page was refreshed.

One main request was made to load the Google homepage (document type).  
The browser sent a GET request to the Google server to retrieve the HTML content of the page.

After that, additional requests were made to load:
- JavaScript files
- CSS stylesheets
- Images (PNG/SVG)
- Background services (XHR requests)

This shows that even a simple webpage requires multiple resources to fully load.


->Observed status code

I observed the status code 200 for most requests.

Status Code 200 means:
The request was successful and the server returned the requested resource correctly.

I also noticed some 302 responses, which indicate redirection.

->What is HTTP?

HTTP (HyperText Transfer Protocol) is a communication protocol used between a web browser and a web server.

It works in a request-response model:

- The browser sends a request.
- The server processes the request.
- The server sends back a response.


->Difference Between HTTP and HTTPS

 HTTP :
 
1.Not encrypted
2.Less secure
3.Uses port 80

HTTPS :

1. Encrypted
2. More secure
3. Uses port 443

HTTPS uses SSL/TLS encryption to protect data from being intercepted or modified by attackers.

->What is a Status Code?

A status code is a 3-digit number sent by the server in response to a request.

It tells the browser whether the request was successful or if there was an error.

Examples:
- 200 – Success
- 301/302 – Redirect
- 404 – Not Found
- 500 – Server Error

->One Thing That Surprised Me

I was surprised to see how many requests are made just to load a single webpage.

Even a simple homepage like Google loads many scripts, images, and background requests.  
This helped me understand how much activity happens behind the scenes when we browse the internet.


My today's learning outcome

From this task, I learned:

- How browsers communicate with servers using HTTP/HTTPS
- How to observe network traffic using Developer Tools
- The importance of status codes
- How multiple resources are loaded for a single webpage
- Basic understanding of web communication useful for cybersecurity and SOC analysis
