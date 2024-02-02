---
author: Daniel Sanchez
title: Pointers in C
---

## Types of pointers

- `Null Pointer`: It's a pointer that points to nothing. They are useful
    at initialization.
- `Void Pointer`: It's a pointer that is not allied with any data types.
    Points to some data location within the storage. It's also known
    as a general purpose pointer. In C, `malloc` and `calloc`
    functions return `void*`.
- `Wild Pointer`: Pointers that are not initialized. It could be
    initialized to a non-NULL garbage value which may not be a valid
    address.
- `Dangling Pointer`: A pointer that points to a memory location that
    has been deleted.
- `Struct Pointer`: This pointers can be utilized to refer to a struct
    by its address. This helps pass structs to a function.
- `Near Pointer`: It means a pointer that is utilized to bit address of
    up to 16 bits within a given section of that computer memory which
    is 16 bit enabled. It can only access data of the small size of
    about 64kb withing a given period, which is its main disadvantage.
- `Far Pointer`: Is typically 32 bit which can access memory outside
    that current segment. To utilize the far pointer, the compiler
    allows a segment register to save segment address, then another
    register to save offset inside current segment.
- `Huge Pointer`: A far pointer that is fixed and hence that part of
    that sector within which they are located cannot be changed in any
    way; huge pointers can be.

```mermaid
flowchart LR  
    A(variable) -->|&| B(pointer)
    B -->|*| A
```

```c
// Declare a reference
int& num;

// Equivalent accessing
*(ptr + n) = val;
ptr[n] = val;

// Equivalent accessing
*(*(ch_arr + i) + j);
ch_arr[i][j];

// Equivalent for structs
(*node).next;
node->next;
```

## References
- [:material-web: How to interpret complex `C/C++` (pointer) declarations](https://www.codeproject.com/Articles/7042/How-to-interpret-complex-C-C-declarations)

