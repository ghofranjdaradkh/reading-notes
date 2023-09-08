
# Reading LAB 13

## Related data in Spring (only read section “3. One-to-Many Relationship”)
### Name a few real life examples of “One To Many” relatioships.
Teachers and Students :

A teacher can have multiple students in a classroom, but each student has only one teacher for that particular class.

Parent and Children:

One parent can have multiple children, but each child has only two biological parents (one mother and one father).

====================================================================================================
### Given two entities, one named Player and one named Team, if you wanted to create a one to many relationship with those entities which would be the one and which would be the many?


In a one-to-many relationship between "Player" and "Team," the "Team" entity would  be the "one" side, and the "Player" entity would be the "many" side.

========================================================================================================
### Explain one to many relationships to a non-technical friend.

"one-to-many" relationship between a teacher and students, one teacher is connected to many students (the "many" side), but each student is connected to only that one teacher (the "one" side). Just like in a classroom, where the teacher teaches many students, but each student has only one teacher

========================================================================================================
========================================================================================================
##  Spring Integration Testing

### Describe the difference between a unit test and an integration test.

Unit Test:   purpose of unit tests is to verify that each small piece of code (a unit) performs its specific task correctly. They check whether functions or methods produce the expected output when given certain inputs.Unit tests are designed to run independently from the rest of the application. They should not depend on external systems, databases, or other components of the software >>>>>>>>>>> Integration Test:  purpose of integration tests is to validate that the integrated system functions as expected. They check whether various parts of the software work together harmoniously and that data flows correctly between them.  focus on testing the interactions and connections between different units or components of a software application. They aim to ensure that these units work correctly together when integrated into the larger system. 

========================================================================================================
### What is the object that provides support for Spring MVC Testing?

MockMvc is a part of the Spring Test framework and is designed specifically for testing Spring MVC applications. It allows you to simulate HTTP requests and interact with your controllers as if you were making real HTTP requests to your application. This makes it a valuable tool for writing integration tests for Spring MVC controllers and testing how they handle various requests and scenarios in a controlled and isolated environment.

========================================================================================================

### What does the “perform()” method do in a Spring integration test?

perform() method part of "MocMvc" framework in Spring Mvc testing, will call a HTTP requestS methods(GET, POST ,...), which returns the ResultActions. Using this result, we can have assertion expectations about the response, like its content, HTTP status, or header.

========================================================================================================