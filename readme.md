# Four Pillar of OOP

Objects are containers that: 
1) Contains data
2) Has functionality

All Objects are based on a **Class**

Class is a prototype of an object. It describes what variable and function the object should have.

C & C++ are programs that does garbage collection. (RAM Influence)

There is no control on when this will happen. 

"Buffer Overflow"

Mordern language will automatic empty the RAM. 

Compiled language vs Intepreted language


## Encapsulation & Data Hiding
Put all information and functions that are related into a single **Class**
Data or business rules

Data must be relavent
```
Class Employee{
    constructor(first_name){
        this.first_name = first_name
    }

}
```

Business rules can be as such (Make certain conditions before data can be stored)
```
setFirstName(newName){
    if (newName.length > 3){
        this.first_name = newName
    }
}
```

Data hiding is to prevent people from directly changing certain value

JavaScript is not a full OOP language because data hiding cannot be done. 

Only way is to have consenses not to touch other people's variable

## Inheritance
* Share code from one class to another


## Polymorphism
Not needed in JavaScript

## Composition
As a class, it can contain another class. Example a school have many department. 

When learning Java will talk about this more


# Linked list (refer to Node.js under 02-linked-list)

[Article to reference](https://humanwhocodes.com/blog/2019/01/computer-science-in-javascript-linked-list/)

It is a gateway to more complex things

Every data that is stored in a linked list is a node

Every node knows what is the next node AFTER it

Normally we are using Vectors 

Vectors can solve data fragmentation

Single linked list and Double linked list (can refer to previous node)

Must understand the "next" behaviour

Linked list is a collection of nodes that contain data elements in a linear collection. 

In a list, it starts with a head (before the first node) and ends with a null (after the last node).


Two case that will happen (reference to LinkedList.js)
1. When the list is empty
2. When the list is occupied


## LinkedList Questions
1. Add a function with the name `count` to the LinkedList that returns how many items there.

2. Add a function with the name `contains` and returns `true` if the given argument exists as data in one of the nodes in the linked list.
Else return `false`


# Stack and Queue
List, queue and stack are the basic data structures used in programming. 

Lists are also known as linked lists.

Queues are first-in first-out data structures.  (FIFO)

Example, printer queue system

#### Computer Simulation (Queue)
Using a random number generattor to simulate queues/processess, simulations can help planners to predict the efficiency of a business process or assembly line.

Stacks are last-in first-out data structures. (LIFO)

Example of stacks, undo function in computer, stack of cards, browser history & back button.

Parentheses checking


# Recursion
Iterative loop (while and for)
```` 
for (let i = 0; i<=10; i++){
    console.log(i)
}
``` 

Using recursive way to call a loop
You will get a COPY of the function inside the stack
Recursive solution has three component
Processing - What do you do  to the data
Base case - When you do not need to call the function back
Recursive - Start another function inside the function
```
function countUp(start, end){
    console.log(start)
    if (start == end){
        return;
    }
    countUp(start+1, end); 
}

(countUp(1,4))
```