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


When learning Java will talk about this more