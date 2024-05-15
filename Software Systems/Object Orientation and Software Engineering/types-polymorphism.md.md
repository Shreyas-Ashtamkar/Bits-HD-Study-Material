Path : [/Software Systems](<..\..\index.md>) [/Object Orientation and Software Engineering](<..\index.md>)
## Types and Polymorphism in Object Orientation and Software Engineering

**Types in Object Orientation:**

Types define the structure and behavior of data and methods in object-oriented programming. They categorize values and promote data integrity by ensuring compatibility and consistency. Different types exist:

**1. Primitive Types:**
- Built-in types like `int`, `float`, `char` representing basic data values.


**2. User-Defined Types:**
- Classes and structures created by users to represent complex data or behavior.


**3. Reference/Pointer Types:**
- Hold memory address of other objects.


**4. Derived/Inherited Types:**
- Created by inheriting properties and methods from base/super classes.


**Polymorphism:**

Polymorphism allows objects of different types to be treated as a common type. It involves two key concepts:

**1. Compile-time Polymorphism:**
- Overloading methods/operators with same name but different parameters.
- Overriding methods in derived classes with more specific implementation.


**2. Runtime Polymorphism:**
- Ability to determine the actual type of an object at runtime.
- Allows calling the correct method based on the actual type of the object.


**Types of Polymorphism:**

**1. Operator Overloading:**
- Overloading operators like `+` or `-` for different operand types.


**2. Method Overloading:**
- Creating multiple methods with the same name but different parameters.


**3. Method Overriding:**
- Defining a method in a derived class with the same name and signature as a method in the base class.


**4. Dynamic Dispatch:**
- Runtime mechanism that selects the appropriate method based on the actual type of the object.


**Applications of Polymorphism:**

- **Extensibility:** Ability to add new features by overriding methods without changing existing code.
- **Modularity:** Reusable code through inheritance and polymorphism.
- **Maintainability:** Easy updates and bug fixes by overriding methods.


**Example:**

```java
class Shape {
    void draw() {
        // Generic drawing code
    }
}

class Circle extends Shape {
    @Override
    void draw() {
        // Code to draw a circle
    }
}

class Square extends Shape {
    @Override
    void draw() {
        // Code to draw a square
    }
}

Shape shape = new Circle(); // Dynamic dispatch - runtime polymorphism
shape.draw(); // Will draw a circle
```

**Conclusion:**

Types and polymorphism are integral aspects of object-oriented programming, enabling flexibility, reusability, and extensibility in software systems. By leveraging these features, developers can create robust, maintainable, and adaptable code.
