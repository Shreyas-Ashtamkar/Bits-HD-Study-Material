Path : [/Software Systems](../../index.md) [/Object Orientation and Software Engineering](../index.md)
## Basics of OOP - Objects, Classes and Delegation in Object Orientation and Software Engineering

**Object-Oriented Programming (OOP)** is a programming paradigm that emphasizes the use of "objects" to design applications and software systems. These objects are bundles of data (attributes) and methods (actions) that can be easily combined to create complex applications.


### Objects

**Definition:** An object is a collection of data and methods that represent a real-world entity such as a customer, product or employee.

**Properties:**
- Data fields/attributes
- Methods/functions


**Example:**

```
class Customer {
    name: string
    email: string
    address: string

    greet(): void {
        console.log('Hello!')
    }
}
```

In this example, `Customer` is a class (blueprint) with attributes `name`, `email` and `address`, and a method called `greet()`.


### Classes

**Definition:** A class is a blueprint or template for creating objects. It defines the properties and methods that are common to all objects of that class.

**Characteristics:**
- Reusable
- Extensible
- Encapsulated


**Example:**

```
class Vehicle {
    wheels: number
    engines: number

    move(): void {
        console.log('Moving forward.')
    }
}

class Car extends Vehicle {
    seats: number

    honk(): void {
        console.log('Honk!')
    }
}
```

Here, `Vehicle` is a base class with properties `wheels` and `engines` and a method `move()`. `Car` is a derived class from `Vehicle` adding property `seats` and method `honk()`.


### Delegation

**Definition:** Delegation is the process of assigning responsibility for certain tasks to objects other than the one performing the action.

**Mechanism:**
- The object performs an action but forwards the execution to another object.
- A method calls a method on another object through its reference or pointer.


**Example:**

```
class UserService {
    fetchUser(id: string): User {
        // Code to fetch user data from database
    }
}

class AuthenticationService {
    authenticate(token: string): boolean {
        // Code to authenticate user
    }
}

class UserController {
    constructor(private userService: UserService, private authenticationService: AuthenticationService) {}

    getUser(id: string): User {
       const user = this.userService.fetchUser(id)
       if (this.authenticationService.authenticate(user.token)) {
           return user
       }
    }
}
```

**Benefits of Delegation:**
- Reduced code duplication
- Improved modularity and maintainability
- Enhanced reusability and extensibility


**Conclusion:**

OOP concepts like objects, classes and delegation are fundamental to software engineering. Understanding these principles is crucial for developing modular, reusable and maintainable applications and software systems. By leveraging these concepts, developers can create cohesive and efficient software solutions.
