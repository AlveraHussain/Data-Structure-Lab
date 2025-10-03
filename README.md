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
