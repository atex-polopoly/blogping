=================================
1. Work assignment 
=================================

The point of this assignment is to let you show us how you handle a java based programming task. When we review your code we'll take into account concepts like:

 - Clean design
 - Reuse (3:rd part products)
 - Maintainability
 - Testability
 - Java knowledge
 - Coding style

It's up to you to decide how much time and effort you need to devote to the assignment to show us that you know how to work with the above concepts. 

=================================
2. Assignment description - Blog Ping
=================================

Write a java client and server that implements the "blog ping" protocol.

Client:
 - Command-Line or web interface
 - Calls a blogping server using the REST-api
 - Handles errors

Server:
 - Accepts blogping messages using REST
 - Serves a changes.xml over HTTP containing all pinged blogs.
 - Handles concurrent connections

The blogping and changes.xml format is documented at http://www.weblogs.com/api.html. Note that only the REST interface is necessary to implement in this assignment.


=================================
3. Provided code base
=================================

To get up and running with the provided base code you'll need maven and a recent JDK. Try running "mvn jetty:run" and opening http://localhost:8080/hello in your browser. You should see a greeting message served by the HelloAtexServlet.java class. There is some example code included in BlogpingServlet.java that you can use as a starting point.

There are a couple of unit and integration tests included. To run the integration tests, run "mvn verify". The provided integration test "BlogpingIT" should pass if your implementation is correct. 

Note that we encourage you to write your own unit and integration tests to assert that your code works as intended (and to show us how you test your code).
