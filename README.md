# In-Memory-Database-Server

# In-Memory Database Server in C

> Building a high-performance in-memory database from first principles to explore systems programming, networking, and low-level optimization in C.

![Language](https://img.shields.io/badge/Language-C-blue)
![Platform](https://img.shields.io/badge/Platform-Linux-lightgrey)
![Build](https://img.shields.io/badge/Build-Makefile-success)
![Status](https://img.shields.io/badge/Status-Work%20in%20Progress-orange)

---

## About the Project

Modern databases like Redis are incredibly fast, but understanding *why* they are fast requires looking beneath the abstraction.

This project is my attempt to build an in-memory database server completely from scratch in C. Instead of relying on existing libraries or frameworks, every major component—from the underlying data structures to the networking layer—is implemented manually to gain a deeper understanding of systems programming.

The goal isn't simply to create another key-value store. It's to understand how efficient memory layouts, optimized search algorithms, socket programming, and careful resource management come together to build software capable of handling thousands of operations per second.

---

## Why This Project?

This repository is primarily a learning journey focused on:

* Writing production-style C code
* Understanding memory at a low level
* Designing efficient data structures
* Learning TCP socket programming
* Exploring high-performance server architecture
* Improving debugging and optimization skills

Every feature is implemented incrementally, making the repository a record of both the final implementation and the engineering decisions behind it.

---

## Features

### Data Storage

* Custom binary tree implementation
* Dynamic node allocation
* Insert, delete, update, and search operations
* Efficient in-memory key-value storage
* Tree visualization for debugging

### Networking

* TCP socket server
* Client-server communication
* Command parsing
* Request processing
* Concurrent client handling

### Performance

* Optimized tree traversal
* Transition from linear search to hash-based lookups
* Manual memory optimization
* Cache-conscious data organization

### Systems Programming

* Structs and unions
* Pointers and function pointers
* Linked data structures
* Dynamic memory allocation
* Process forking
* Low-level debugging techniques

---

## Technology Stack

| Category     | Technology        |
| ------------ | ----------------- |
| Language     | C                 |
| Build System | Make              |
| Platform     | Linux             |
| Networking   | POSIX TCP Sockets |
| Debugging    | GDB               |
| Development  | VS Code           |

---

## Project Structure

```text
in-memory-db/
│
├── src/
│   ├── server.c
│   ├── database.c
│   ├── tree.c
│   ├── hashtable.c
│   ├── parser.c
│   ├── network.c
│   ├── memory.c
│   └── utils.c
│
├── include/
│   ├── database.h
│   ├── tree.h
│   ├── hashtable.h
│   ├── network.h
│   └── utils.h
│
├── tests/
├── docs/
├── Makefile
└── README.md
```

---


## Building the Project

Clone the repository:

```bash
git clone https://github.com/yourusername/in-memory-database.git
```

Navigate into the project:

```bash
cd in-memory-database
```

Compile:

```bash
make
```

Run:

```bash
./database
```

---

## Future Improvements

* Self-balancing trees
* LRU cache
* Write-ahead logging
* Disk persistence
* Replication
* Transactions
* Benchmark suite
* Multi-threaded request handling
* Command pipelining

---


## License

This project is licensed under the MIT License.

---


B.Tech Graduate • Systems Programming Enthusiast • Backend Development • Data Structures & Algorithms
