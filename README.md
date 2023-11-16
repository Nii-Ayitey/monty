The Monty language
Monty 0.98 is a scripting language that is first compiled into Monty byte codes (Just like Python). It relies on a unique stack, with specific instructions to manipulate it. The goal of this project is to create an interpreter for Monty ByteCodes files.

Monty byte code files

Files containing Monty byte codes usually have the .m extension. Most of the industry uses this standard but it is not required by the specification of the language. There is not more than one instruction per line. There can be any number of spaces before or after the opcode and its argument:
### LIFO and FIFO:

- **LIFO:** Stands for "Last In, First Out." In a LIFO data structure, the last element added is the first one to be removed. It operates like a stack of plates—new plates (or elements) are added to the top, and the last one added is the first one removed.

- **FIFO:** Stands for "First In, First Out." In a FIFO data structure, the first element added is the first one to be removed. It operates like a queue in real life—people enter a queue, and the first person who joined is the first to proceed.

### Stack:

- A **stack** is a data structure that follows the LIFO principle. Elements are added or removed from the top of the stack. It supports two main operations: `push` (to add an element) and `pop` (to remove the top element).

- **When to Use:**
  - Managing function calls and recursion (call stack).
  - Undo mechanisms in applications.
  - Expression evaluation (postfix/prefix notation).
  - Browser history.

### Queue:

- A **queue** is a data structure that follows the FIFO principle. Elements are added at the rear and removed from the front. It supports two main operations: `enqueue` (to add an element) and `dequeue` (to remove the front element).

- **When to Use:**
  - Print job scheduling.
  - Task scheduling in operating systems.
  - Breadth-first search algorithms.
  - Request handling in web servers.

### Common Implementations:

- **Stack:**
  - Implemented using arrays or linked lists.
  - Python's list can be used as a stack.

- **Queue:**
  - Implemented using arrays or linked lists.
  - Python's `collections.deque` provides an efficient implementation.

### Common Use Cases:

- **Stack:**
  - Reversing items.
  - Syntax checking (e.g., parentheses matching).
  - Function call management.
  - Undo/Redo functionality.

- **Queue:**
  - Task scheduling.
  - Print job management.
  - Breadth-first search.
  - Order processing systems.

### Proper Use of Global Variables:

While it's generally recommended to minimize the use of global variables, if you need to use them:

- Clearly document their purpose.
- Avoid using them unnecessarily; prefer passing variables as arguments.
- Use uppercase names to distinguish them from local variables.
- Consider encapsulating them in a module or class to minimize global namespace pollution.
- Be cautious about potential side effects on the program's state.
