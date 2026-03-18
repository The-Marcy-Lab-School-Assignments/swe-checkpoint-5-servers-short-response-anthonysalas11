# Short Response Questions

Answer each of these questions completely but concisely. Use the proper technical terminology. You may refer to the [Marcy Lab School Docs](https://marcylabschool.gitbook.io/marcy-lab-school-docs) or Google but do NOT copy and paste definitions or explanations verbatim.

You can earn up to 6 points for each response (3 points for writing quality, 3 points for technical content).

Before submitting your responses, use a spell checker / AI to ensure that you have no grammar or spelling mistakes.

## Question 1: Servers and HTTP

What is a server? Describe the HTTP request-response cycle including the key components of a request (method, endpoint, headers, body) and a response (status code, headers, body). Use an analogy to support your explanation.

**Your Answer:**
A server is a program that listens for request, analyzes the request and sends back a constructed response.The sever uses specific ports to actively listen for incoming request.The ports are used as channels that direct traffic between incoming request to the proper port.It is similar to ordering pizza, the building itself would be the computer, and the doors with apartment numbers are the ports.Without the apartment number, the person delivering the pizza would have trouble knowing which door to deliver the pizza to, since there are so many.The HTTP request-response cycle is the communication between client-server applications over the web.When a client sends a request to a server it has components such as the method which tells the server what type of request it will be.An example can be GET which reads or request data, or POST which creates new data.A request also includes the URL which serves as a specific endpoint to let the server know what resource is being accessed.The headers include information like the content-type, information about the web browser we are using, and a body which is usually empty.The body is what the response uses to input actual data.The response includes status codes to let the client know if the response was a success or failure.three digit codes along the 200's signify successes and 400's signify failures.The response also has headers that include status text along with status code,content-type and the data that it will send back in the body.It is like delivering mail.The card has the senders address (request) and the the address of the person we are trying to reach (response). The mailman knows where (API) each address lives so if anything should go wrong it can send the mail back to the sender and let them know what went wrong (status codes).

## Question 2: Middleware

What is middleware in Express? How does it differ from a regular controller? Explain the role of `next()` and provide an example of when middleware is useful.

**Your Answer:**
Middleware is a function that is used to process incoming HTTP request.It performs server-side actions like parsing the request,modifying the response, and executing additional logic before passing it to the next middleware in the chain.

## Question 3: API Key Security

Why is it dangerous to use API keys in client-side (frontend) code? Explain how a backend server solves this problem (the "proxy" pattern). Include what role environment variables (`.env`) play in this approach.

**Your Answer:**

## Question 4: Debugging a Server

A fellow student is building an Express server. They send a `PATCH` request to `/api/bookmarks/1` using Postman, but they receive a `404` status code. List at least three things you would check to debug this issue and explain why each one could be the cause of the problem.

**Your Answer:**
