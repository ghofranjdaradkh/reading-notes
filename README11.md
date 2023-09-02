


## What role do the @Controller classes play in a Spring MVC application?

@Controller is an annotation used in Spring MVC to define a class as a controller. It is used to handle HTTP requests and map them to specific methods.




 ## Explain to a non-technical friend what a GET request is.




A GET request is like ordering food from a restaurant's menu, asking the librarian for a specific book in a library. In web , it's how you ask a website's server for information or a particular webpage. When you type a website's address into your browser and hit Enter, you're making a GET request. The server then responds by sending back the webpage or information you asked for, just like receiving your food order or the book you requested.




 ## What annotation should be placed on your Spring Boot application class?




For a Spring Boot application, you should place the @SpringBootApplication annotation on your main application class.

@SpringBootApplication is a meta-annotation in Spring Boot. It combines several annotations, including @Configuration, @EnableAutoConfiguration and @ComponentScan, into a single, convenient annotation.





## What method allows for a variable defined in Java (in your Spring Controller) to be displayed in HTML with the help of Thymeleaf?

In Thymeleaf, this model attributes (or context variables ) can be accessed and displayed with the following syntax: ${attributeName}, 

You can access model attributes in views with Thymeleaf as follows:

    <tr th:each="message : ${messages}">
        <td th:text="${message.id}">1</td>
        <td><a href="#" th:text="${message.title}">Title ...</a></td>
        <td th:text="${message.text}">Text ...</td>
    </tr>







## Explain the role of a @Controller class in a Spring MVC application.

@Controller class plays a central role in managing HTTP requests and controlling the application's flow. Its primary responsibilities include: Request Handling: A @Controller is responsible for handling incoming HTTP requests. It listens to specific URL patterns and HTTP methods using annotations like @RequestMapping, @GetMapping, @PostMapping, etc.  Data Preparation: prepare data (model attributes) that need to be displayed or included in the response. creating a model map this model map acts as a container for data that will be used by the view.





 ## What is a model attribute refered to in Thymeleaf?   

model attributes: the pieces of data that can be accessed during the execution of views ,In Thymeleaf, a model attribute  is referred to as a "context variable."

















