## Things I want to know more about
# class4


The LinkedList class is a collection which can contain many objects of the same type, it is  a data structure that contains nodes that links/points to the next node in the list. can shrink and grow in memory. It doesn’t need a set amount of memory to be allocated in order to exist, and its size and shape can change, and the amount of memory it needs can change as well.

## Analogy

A common analogy for Linked Lists is a train. The engine is the head and each car is a node. The train cars are linked together, but can be reordered by changing how the cars are linked.

## Explanation:


Node (Train Car): A node is like a train car that holds information (data) and knows the next car's location. Each node can store different types of data, just like passengers with distinct details.

Data (Passengers): Think of data as the passengers inside each train car (node). Each passenger has their own unique information, such as names or numbers.

Next Pointer (Coupling): Nodes are connected in a sequence using next pointers, just like train cars are linked by couplings. Each node knows where the next node is located.

Head Node (Train Engine): The head node is the first car of the train. It's the starting point for exploring the linked list and guides the traversal process.

Insertion (Adding Cars): Adding a new node is like inserting a new car between two existing cars. You adjust the couplings (next pointers) to include the new node in the sequence.

Deletion (Removing Cars): Deleting a node is like removing a car from the train. The neighboring cars' couplings are adjusted to maintain the connection, skipping the deleted node.


 

 ## Types of  linked list :

Singly Linked List: Each node points to the next node.

- Doubly Linked List: Each node has pointers to both the next and previous nodes.

- Circular Linked List: Last node points back to the first node.




## How the LinkedList works

The LinkedList stores its items in "containers." The list has a link to the first container and each container has a link to the next container in the list. To add an element to the list, the element is placed into a new container and that container is linked to one of the other containers in the list.




## WHY the LinkedList :

Linked lists provide a dynamic and flexible way to manage collections of data.
They excel in scenarios where frequent insertions and deletions are common, without the need for contiguous memory allocation.




## WHAT structure:

A linked list is a linear data structure composed of nodes, each containing data and a reference (or pointer) to the next node in the sequence.
Unlike arrays, linked lists do not require contiguous memory allocation, allowing elements to be scattered in memory.




## example :

import java.util.LinkedList;

public class Main { public static void main(String[] args) {

LinkedList<String> cars = new LinkedList<String>();

cars.add("Volvo");

cars.add("BMW");

cars.add("Ford");

cars.add("Mazda");

System.out.println(cars); } }




    ## Create a vocabulary/definition list

Node: A fundamental unit of a linked list, containing data and a reference to the next node (and previous node in a doubly linked list).

Singly Linked List: A type of linked list where each node points to the next node in the sequence.

Doubly Linked List: A type of linked list where each node has references to both the next and previous nodes.

Head: The first node in a linked list, serving as the starting point for traversal.

Tail: The last node in a linked list, indicating the end of the sequence.

Pointer: A reference that points to another node's memory location.

Insertion: The process of adding a new node to a linked list at a specific position.

Deletion: The process of removing a node from a linked list.

Traversal: Moving through each node of a linked list to perform an operation.




## Linked List Visualization:

1. Node 1 -> Node 2 -> Node 3 -> Node 4 -> Node 5

[ Data | Next ] [ Data | Next ] [ Data | Next ] [ Data | Next ] [ Data | Next ].

