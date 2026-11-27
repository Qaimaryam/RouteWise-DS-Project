# RouteWise 
### Smart Delivery and Route Optimization System

RouteWise is a console-based C++ application designed for a courier company to manage customers, parcels, delivery requests, and city routes efficiently.

The project demonstrates the practical implementation of fundamental and advanced data structures and algorithms in a real-world delivery management scenario. All data structures are implemented manually without using STL containers.

---

## Project Overview

RouteWise provides a menu-driven delivery management system that allows operators to register customers and parcels, manage delivery requests, track parcel records, undo operations, and explore optimized routes through a city road network.

The system loads customer records, parcel records, and the city network from text files. New records are saved automatically, helping maintain data between program executions.

---

## Features

- **Customer Management** – Register and manage customer information.
- **Parcel Registration** – Add parcels with tracking IDs, source, destination, weight, and priority.
- **Parcel Search** – Search parcels efficiently using a hash table.
- **Delivery Dispatching** – Manage normal and urgent delivery requests.
- **Priority-Based Delivery** – Process urgent parcels according to priority.
- **Delivery History** – Maintain records of processed and delivered parcels.
- **Undo Operations** – Undo the last supported operation.
- **Parcel Indexing** – Store and retrieve parcel records using BST and AVL trees.
- **City Network Visualization** – Display the city road network.
- **Network Traversal** – Explore locations using BFS and DFS.
- **Shortest Delivery Route** – Find the shortest route between two locations using Dijkstra's algorithm.
- **Minimum Delivery Network** – Generate a minimum spanning tree using Prim's algorithm.
- **Performance Comparison** – Compare BST and AVL tree performance.
- **System Statistics** – Display customers, parcels, delivery queues, network information, and tree statistics.

---

## Data Structures & Algorithms

RouteWise uses the following data structures and algorithms:

| Module | Data Structure / Algorithm |
|---|---|
| Customer Records | Linked List |
| Parcel Records | Hash Table with Linear Probing |
| Normal Delivery Requests | Queue |
| Urgent Delivery Requests | Max-Heap |
| Delivery History | Doubly Linked List |
| Undo Operations | Stack |
| Parcel Index | Binary Search Tree (BST) |
| Balanced Parcel Index | AVL Tree |
| City Road Network | Graph using Adjacency List and Matrix |
| Network Traversal | Breadth-First Search (BFS) |
| Network Traversal | Depth-First Search (DFS) |
| Shortest Route | Dijkstra's Algorithm |
| Minimum Network | Prim's Minimum Spanning Tree (MST) |

---

## System Modules

The project is organized into modular header files:

| File | Responsibility |
|---|---|
| `CustomerList.h` | Customer management using a linked list |
| `ParcelHashTable.h` | Parcel storage and searching using hashing |
| `Queue.h` | Normal delivery queue |
| `UrgentHeap.h` | Priority-based urgent delivery dispatch |
| `DeliveryHistory.h` | Delivery history management |
| `Stack.h` | Undo functionality |
| `ParcelBST.h` | Parcel indexing using BST |
| `ParcelAVL.h` | Balanced parcel indexing using AVL tree |
| `Graph.h` | City network, traversal, shortest route, and MST |
| `Models.h` | Customer, parcel, and other record structures |
| `Utils.h` | Input validation and utility functions |
| `RouteWiseSystem.h` | Integration of modules and menu system |

---

## Main Menu

RouteWise provides 18 menu options:

1. Register Customer
2. Register Parcel
3. Search Parcel
4. Add Normal Delivery Request
5. Add Urgent Delivery Request
6. Process Next Delivery
7. Mark Parcel as Delivered
8. Undo Last Operation
9. Display Pending Deliveries
10. Display Parcel Records
11. Display City Network
12. BFS Network Traversal
13. DFS Network Traversal
14. Find Shortest Delivery Route
15. Generate Minimum Delivery Network
16. Compare BST and AVL Performance
17. Display System Statistics
18. Exit

---

## Time Complexity

The following table summarizes the expected time complexity of major operations:

| Operation | Time Complexity |
|---|---|
| Stack Push / Pop | O(1) |
| Queue Enqueue / Dequeue | O(1) |
| Heap Insert / Remove Top | O(log n) |
| Hash Insert / Search | O(1) average, O(n) worst |
| BST Insert / Search | O(log n) average, O(n) worst |
| AVL Insert / Search | O(log n) |
| Linked List History Addition | O(1) |
| BFS / DFS | O(V + E) |
| Dijkstra's Algorithm | O(V²) |
| Prim's Algorithm | O(V²) |

Where:
- `n` = number of records
- `V` = number of vertices (locations)
- `E` = number of edges (roads)

---

## Technologies Used

- **Language:** C++
- **Programming Approach:** Modular, Object-Oriented Programming
- **Data Structures:** Manually implemented without STL containers
- **Storage:** Text files
- **Interface:** Console-based menu system
- **Algorithms:** Searching, sorting/indexing, graph traversal, shortest path, and minimum spanning tree

---

## Data Storage

RouteWise uses text files to store customer records, parcel records, and city network information.

The application loads existing data when it starts and saves new records automatically.

---

## Team Members

| Name | Roll Number |
|---|---|
| Zunaira Ahmad | 25F-3069 |
| Qaima Maryam | 25F-3016 |
| Hiba Saeed | 25F-3017 |

---

## Project Objective

The objective of RouteWise is to demonstrate how data structures and algorithms can be applied to solve practical problems in courier and delivery management.

By combining parcel management, priority-based dispatching, undo operations, and graph-based route planning, the project provides an educational implementation of a smart delivery management system.

---

**RouteWise — Smarter Deliveries, Optimized Routes.**
