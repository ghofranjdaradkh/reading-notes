 ## Question 1 :How are query methods defined when using Spring Data JPA?

In Spring Data JPA, query methods are defined by creating method signatures in a repository interface. These method signatures follow a specific naming convention that allows Spring Data JPA to automatically generate the corresponding SQL queries at runtime.

Method names should start with a prefix like findBy  ,the next part of the method name should specify the property  you want to query by using camelCase. For example, if you have a lastName property in your entity, you can use findByLastName.

## Question 2 :Which dependencies will you need in order to complete the Spring guide?

Spring Data JPA SQL Persist data in SQL stores with Java Persistence API using Spring Data and Hibernate.
H2 Database SQLProvides a fast in-memory database that supports JDBC API and R2DBC access, with a small (2mb) footprint. Supports embedded and server modes as well as a browser based console application.


## Question 3 :What annotations are used to specify an auto generated identification number for an Entity?

@Id so that JPA recognizes it as the object’s ID. The id property is also annotated with @GeneratedValue to indicate that the ID should be generated automatically.





## Question 4: Which of the Spring Data Repositories covered in the readings has the most methods available to it? 

 JpaRepository  >>>

findAll() – get a List of all available entities in the database
findAll(…) – get a List of all available entities and sort them using the provided condition
save(…) – save an Iterable of entities. Here, we can pass multiple objects to save them in a batch
flush() – flush all pending tasks to the database
saveAndFlush(…) – save the entity and flush changes immediately
deleteInBatch(…) – delete an Iterable of entities. Here, we can pass multiple objects to delete them in a batch

## Question 5 :Name a downstide of a Spring Data Repository :
Our code becomes tightly coupled to the library and its specific abstractions, including Page and Pageable. This coupling isn't exclusive to this particular library; however, we must exercise caution not to inadvertently reveal these internal implementation details.

When we extend a repository interface like CrudRepository, we expose a comprehensive suite of persistence methods all at once. In many cases, this is perfectly acceptable. Nevertheless, there might arise situations where we desire a more granular level of control over which methods we make accessible. For instance, we may wish to craft a specialized ReadOnlyRepository that deliberately omits certain methods, such as save(…) and delete(…), which are part of the standard offering in CrudRepository.


## Question 6 :How would you define an operation to find a student based on their name in a repo named StudentRepository which extends JpaRepository?

To define an operation to find a student based on their name in a repository named StudentRepository, which extends JpaRepository, you would create a method with a specific naming convention. Assuming you have an entity class named Student with a property name, you can define the method as follows:



import org.springframework.data.jpa.repository.JpaRepository;
public interface StudentRepository extends JpaRepository<Student, Long> {
Student findByName(String name); }

 