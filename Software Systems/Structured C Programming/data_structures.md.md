Path : [/Software Systems](<..\..\index.md>) [/Structured C Programming](<..\index.md>)
## Dynamically Allocated Data & Linked Lists in Control Constructs in Structured C Programming for Software Systems

**Introduction**

Dynamically allocated data and linked lists are fundamental data structures employed in Structured C programming for software systems. These tools enable flexible memory management and efficient data manipulation in various scenarios.

**Dynamic Allocation**

Dynamic allocation is the runtime memory allocation of memory blocks from a memory pool. In Structured C, the `malloc()` and `free()` functions are used for this purpose.

```c
void *malloc(size_t size);
void free(void *ptr);
```

**Example:**

```c
int *arr = (int *)malloc(sizeof(int) * 10);
free(arr);
```

**Linked Lists**

A linked list is a linear data structure where individual memory blocks (nodes) are connected by pointers. Each node contains two fields:

- **Data:** Stores the actual data value
- **Next:** Points to the next node in the list


**Types of Linked Lists:**

- **Single Linked List:** Each node points only to the next node.
- **Double Linked List:** Each node points to both the next and previous nodes.


**Applications of Linked Lists:**

- Implementing insertion and deletion at the head/tail
- Implementing stacks and queues


**Control Constructs**

Control constructs are statements that influence the flow of program execution based on certain conditions or loops.

**Common Control Constructs:**

- `if-else` statements
- `switch` statements
- `for` loops
- `while` loops


**Dynamically Allocated Data & Linked Lists in Control Constructs**

**1. Inserting data dynamically:**

- Allocate memory for a new node.
- Set the data field of the node.
- Update the `next` pointer of the last node to point to the new node.

**2. Deleting data dynamically:**

- Identify the node to be deleted.
- Update the `next` pointer of the previous node to bypass the deleted node. 
- Free the memory occupied by the deleted node.


**3. Iterating over linked lists:**

- Start from the head of the list.
- While the `next` pointer points to a valid address,
    - Process the data in the current node.
    - Update the current node to point to the next node.


**Conclusion**

Dynamically allocated data and linked lists are powerful data structures in Structured C programming for software systems. Their flexibility and efficient memory management capabilities enable elegant and efficient implementation of various data management and control flow scenarios.
