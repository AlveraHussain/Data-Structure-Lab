# 🧠 Data Structures Lab in C/C++

Welcome to the **Data Structures Lab** — a hands-on repository designed to help you master the building blocks of efficient programming. This lab includes clean, well-commented implementations of essential data structures using **C/C++**, with a strong focus on understanding memory through **pointers**.

## 📘 Topics 

This lab covers the following core data structures and concepts:

- 🔗 Pointers
- 🧵 Linked Lists
- 🌳 Trees (Binary Trees, BSTs)
- 🚦 Queues (Linear and Circular)

Each module includes:

- ✅ Source code with comments
- 🧪 Sample input/output
- 📊 Diagrams and memory illustrations
- 🧠 Conceptual explanations

---

## 📂 Repository Structure

📁 data-structures-lab/
├── pointers/
│   ├── pointer_basics.c
│   ├── pointer_arithmetic.c
│   └── dynamic_memory.c
├── linkedlist/
│   ├── singly_linked_list.c
│   ├── doubly_linked_list.c
│   └── circular_linked_list.c
├── trees/
│   ├── binary_tree.c
│   ├── bst_insert_search.c
│   └── tree_traversals.c
├── queues/
│   ├── linear_queue.c
│   ├── circular_queue.c
│   └── queue_using_linkedlist.c
└── README.md

# 🔗 Deep Dive into Pointers in C/C++

Welcome to the **Pointers Playground** — a comprehensive guide to mastering pointers in C/C++. This repository is built for learners, developers, and interviewees who want to understand how memory works under the hood and how pointers unlock powerful programming techniques.

## 📘 What You'll Learn

This repository covers the following essential pointer concepts:

- 📌 Pointer Declaration
- 🔁 Pointer vs Array
- 🧭 Pointer to Pointer
- 🧠 Function Pointers
- 🧱 Dynamic Memory Allocation (`malloc`, `calloc`, `free`)
- ➕ Pointer Arithmetic

Each topic includes code examples and explanations to help you visualize memory and pointer behavior.

---

## 🧵 Pointer Declaration

Learn how to declare and initialize pointers, understand their types, and explore how they reference memory addresses.

```c
int a = 10;
int *p = &a;
🧮 Pointer vs Array
Understand the subtle differences and similarities between pointers and arrays, including how they behave in memory and function calls.

int arr[5] = {1, 2, 3, 4, 5};
int *p = arr;

🧬 Pointer to Pointer
Explore multi-level indirection and how pointers can point to other pointers.

int a = 5;
int *p = &a;
int **pp = &p;
🧩 Function Pointers
Use pointers to functions for callbacks, dynamic dispatch, and flexible APIs.

void greet() {
    printf("Hello!");
}

void (*func_ptr)() = greet;
func_ptr();
🧱 Dynamic Memory Allocation
Master memory management with malloc, calloc, and free. Learn how to allocate memory at runtime and avoid memory leaks.

int *arr = (int *)malloc(5 * sizeof(int));
free(arr);

➕ Pointer Arithmetic
Manipulate memory using pointer arithmetic. Understand how to traverse arrays, structures, and buffers.

int arr[] = {10, 20, 30};
int *p = arr;
printf("%d", *(p + 1)); // Outputs 20

📂 Repository Structure
📁 pointers-in-c/
├── declaration/
├── pointer_vs_array/
├── pointer_to_pointer/
├── function_pointers/
├── dynamic_memory/
├── pointer_arithmetic/
└── README.md
# 🧵 Linked Lists in C/C++

Welcome to the **Linked List Lab** — a complete guide to understanding and implementing linked lists in C/C++. This repository is designed for students, developers, and interviewees who want to master dynamic data structures and pointer manipulation.

## 📘 What is a Linked List?

A **Linked List** is a linear data structure where elements (nodes) are stored in memory and linked using pointers. Unlike arrays, linked lists allow dynamic memory allocation and efficient insertion/deletion.

---

📂 Repository Structure
 🧵 Linked Lists/
├── singly_linked_list/
│   ├── insert.c
│   ├── delete.c
│   ├── traverse.c
│   └── reverse.c
├── doubly_linked_list/
│   ├── insert.c
│   ├── delete.c
│   ├── traverse.c
│   └── reverse.c
├── circular_linked_list/
│   ├── insert.c
│   ├── delete.c
│   └── traverse.c
├── README.md
🧩 Topics of linked list
1. 🔗 Singly Linked List
Each node contains data and a pointer to the next node.

Operations:

Insertion (at beginning, end, specific position)

Deletion (by value or position)

Traversal

Reversal

struct Node {
    int data;
struct Node* next;
};
🔁 Doubly Linked List
Each node contains data, a pointer to the next node, and a pointer to the previous node.

Allows bidirectional traversal.

Operations:

Insertion and deletion at both ends

Reversal

Efficient backward traversal
struct Node {
    int data;
    struct Node* prev;
    struct Node* next;
};

3. 🔄 Circular Linked List
The last node points back to the first node, forming a circle.

Can be singly or doubly circular.

Operations:

Insertion and deletion

Circular traversal
struct Node {
    int data;
    struct Node* next; // Points to head if it's the last node
};

4. 🧠 Memory Management with Pointers
Linked lists rely heavily on pointers and dynamic memory allocation.

Use malloc() and free() to manage memory.

Avoid memory leaks by freeing unused nodes.

5. 🧪 Sample Code Snippet
// Insert at beginning in singly linked list
void insertAtBeginning(int value) {
    struct Node* newNode = (struct Node*)malloc(sizeof(struct Node));
    newNode->data = value;
    newNode->next = head;
    head = newNode;
