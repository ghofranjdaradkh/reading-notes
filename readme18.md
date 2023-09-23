# Reading Class 18 :


# Many to Many relationShip :

### Name a few examples of real world ManyToMany relationships.

Employees and Projects: any given employee can be assigned to multiple projects and a project may have multiple employees working for it, leading to a many-to-many association between the two.

Doctors and Patients: Doctors can have many patients, and patients can consult multiple doctors over time. A ManyToMany relationship exists between doctors and patients.

Actors and Movies:There is often a ManyToMany relationship between actors and movies. Actors can appear in multiple movies, and at the same time, a single movie can feature multiple actors.

### Explain the significance of a join table for ManyToMany relationships.


@ManyToMany annotation is used in both classes to create the many-to-many relationship between the entities.
 The @JoinTable is used to define the join/link table.
The @JoinColumn annotation is used to specify the join/linking column with the main table

join table : where the owning side of the ManyToMany relationship is Employee, the join table Employee_Project is used to connect Employee records with Project records. This join table typically contains foreign key columns that reference the primary keys of the Employee and Project tables. These foreign keys establish the relationships between specific employees and specific projects.

join table :

The join table provides flexibility in managing the relationship

Without a join table, you would need to duplicate data in both tables to represent the relationship.

The join table keeps all the connections between the two tables tidy and organized without any confusion.







### What are the values held within a join table?

the main thing the forign key and the Id 

EXAMPLE: 

CREATE TABLE `employee_project` (

`employee_id` int(11) NOT NULL,

`project_id` int(11) NOT NULL,

PRIMARY KEY (`employee_id`,`project_id`),

KEY `project_id` (`project_id`),

CONSTRAINT `employee_project_ibfk_1` FOREIGN KEY (`employee_id`) REFERENCES `employee` (`employee_id`),

CONSTRAINT `employee_project_ibfk_2` FOREIGN KEY (`project_id`) REFERENCES `project` (`project_id`) )
ENGINE=InnoDB DEFAULT CHARSET=utf8;



### According to the author of the article, will you ever be truly secure from ALL possible security threats?




While it may not be possible to achieve absolute security, 
the goal is to manage and mitigate security risks to an acceptable level. This involves implementing best practices, regularly updating and patching systems, educating users, and continuously monitoring for and responding to security incidents.