Path : [/Software Systems](../../index.md) [/Structured C Programming](../index.md)
## Loops in Control Constructs in Structured C Programming in Software Systems

### Introduction

Loops are iterative constructs allowing code to be executed repeatedly for a defined number of times or until a specific condition is met. They enhance code efficiency by eliminating redundant code and improving readability by encapsulating repetitive tasks. 

**Types of Loops:**

- **for Loop:** Repetitive execution based on a counter variable.


```c
for (initialization; condition; increment) {
   // Code to be executed
}
```


- **while Loop:** Repetitive execution as long as a condition remains true.


```c
while (condition) {
   // Code to be executed
}
```


- **do-while Loop:** Executes code at least once before checking the condition.


```c
do {
   // Code to be executed
} while (condition);
```


### Applications of Loops

- Data processing and manipulation
- Array traversal
- List handling
- File processing
- Algorithmic implementation


### Example 1: Factorial Function using for loop

```c
int factorial(int n) {
   int result = 1;
   for (int i = 1; i <= n; i++) {
      result *= i;
   }
   return result;
}
```


### Example 2: Finding Sum of Even Numbers in an Array using while Loop

```c
int sum = 0;
int i = 0;
while (arr[i] != -1) {
   if (arr[i] % 2 == 0) {
      sum += arr[i];
   }
   i++;
}
```


### Example 3: Implementing Binary Search using do-while Loop

```c
int binary_search(int arr[], int n, int key) {
   int low = 0;
   int high = n - 1;
   do {
      int mid = (low + high) / 2;
      if (arr[mid] == key) {
         return mid;
      } else if (arr[mid] < key) {
         low = mid + 1;
      } else {
         high = mid - 1;
      }
   } while (low <= high);
   return -1;
}
```

### Conclusion

Loops are essential control constructs in Structured C Programming, offering a versatile way to automate repetitive tasks and improve code efficiency. Understanding and effectively utilizing loop types is crucial for effective software development in C.
