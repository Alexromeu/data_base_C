# data_base_C

A minimal database prototype written in C.  
This project explores how databases store and retrieve data using **serialization** and **B‑Tree indexing**, focusing on correctness, memory layout, and low‑level file operations.

The goal is to understand how real databases (like SQLite) structure pages, rows, and indexes internally.

---

## Features

- Two independent prototypes:
  - **Row‑serialized storage** (`main_serialized_in_row.c`)
  - **B‑Tree‑indexed storage** (`main_serialized_b_tree.c`)
- Supports:
  - `INSERT` operations
  - `SELECT` operations
  - Printing stored rows
- File‑backed persistence using low‑level system calls
- Manual serialization/deserialization of rows
- Basic B‑Tree node structure (internal & leaf nodes)
- Fully written in C with no external dependencies


Each file is a standalone program demonstrating a different storage architecture.

---

## Build

Compile either version with GCC:

```sh
gcc main_serialized_in_row.c -o db_row
gcc main_serialized_b_tree.c -o db_btree


