Path : [/Computer Science](<..\..\index.md>) [/Compiler Construction](<..\index.md>)
## Phases of Compiler Construction

### Phase 1: Lexical Analysis (Scanning)

- Identifies and classifies the characters of the source code (keywords, identifiers, operators, delimiters, etc.)
- Uses a finite state machine (FSM) to recognize patterns in the input
- Outputs a stream of tokens


**Example:**
```
Input: "if x > 10 then print(x)"

Output: {IF, ID, GREATER_THAN, NUM, ID, LEFT_PAREN, PRINT, ID, RIGHT_PAREN}
```

### Phase 2: Syntax Analysis (Parsing)

- Checks if the sequence of tokens adheres to the grammar of the language
- Uses a parsing algorithm (e.g., LL(1), LR(1)) to derive the sentence structure
- If successful, generates a parse tree


**Example:**
```
IF x > 10 THEN PRINT x
```

### Phase 3: Semantic Analysis

- Checks type compatibility of variables and operators
- Enforces language rules and constraints
- Creates an intermediate representation of the program (e.g., abstract syntax tree)


**Example:**
```
if integer x > 10 then print integer x
```

### Phase 4: Intermediate Code Generation

- Translates the intermediate representation into assembly language or bytecode
- Represents operations in a form that the target machine can understand


**Example:**
```
push x
gt 10
if_true print
```

### Phase 5: Code Optimization

- Reduces redundant or unnecessary code
- Optimizes performance by applying various techniques (e.g., register allocation, loop optimization)


**Example:**
```
if x > 10 goto print_label
label print_label: print x
```

### Phase 6: Tat Getting

- Translates the assembly language or bytecode into the machine code for the target platform
- Includes procedures for linking, loading, and running the program


**Example:**
```
0x100: push x
0x101: gt 10
0x102: jz print_label
0x103: ... (code for print function)
0x104: print_label: ... (code to jump to print function)
```
