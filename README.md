# C++ Data Structures

My personal implementations of core data structures from scratch in C++, built during the **Programming Advices** curriculum.

## 📚 Course
* [Data Structures Level 1](https://programmingadvices.com/p/12-data-structures-level1)

## 🛠 Technologies
* **C++**
* Pointers, Memory Management, and Classes

## 🚀 Implementations Included
* **Singly Linked List:** Custom `Node` classes with functions for `InsertAtBeginning`, `InsertAfter`, `DeleteNode`, etc.
* **Doubly Linked List:** Advanced node linking with `Prev` and `Next` pointers for bi-directional traversal.
* **Stacks & Queues:** Implementations demonstrating LIFO and FIFO behavior.
* **Map:** Basic key-value mapping concepts.

### 🧠 Memory Architecture (Doubly Linked List)
```mermaid
flowchart LR
    %% Styling
    classDef ptr fill:#f8bbd0,stroke:#c2185b,stroke-width:2px,color:#000
    classDef data fill:#e1bee7,stroke:#7b1fa2,stroke-width:2px,color:#000
    classDef nullptr fill:#cfd8dc,stroke:#455a64,stroke-width:1px,stroke-dasharray: 5 5,color:#000

    %% Nodes
    NULL1["NULL"]:::nullptr
    NULL2["NULL"]:::nullptr

    subgraph Node 1
    direction LR
        P1["Prev"]:::ptr
        D1["Data (A)"]:::data
        N1["Next"]:::ptr
    end

    subgraph Node 2
    direction LR
        P2["Prev"]:::ptr
        D2["Data (B)"]:::data
        N2["Next"]:::ptr
    end

    %% Connections
    NULL1 <-- "Prev Pointer" --> P1
    N1 -- "Next Pointer" --> Node2
    P2 -- "Prev Pointer" --> Node1
    N2 -- "Next Pointer" --> NULL2
```
