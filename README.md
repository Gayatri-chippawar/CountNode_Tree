# 🌳 Count Nodes in a Binary Tree (Java)

## 📌 Overview

This project demonstrates how to **count the total number of nodes in a Binary Tree** using **recursion in Java**.

Counting nodes is a fundamental operation in **Binary Tree data structures** and is frequently used in **tree-based algorithms and coding interview problems**.

---

# 🌿 Binary Tree Example

Example tree used in the program:

```
        1
       / \
      2   3
     / \  / \
    4  5 6   7
```

Total number of nodes in this tree:

```
7
```

---

# 📏 Problem Statement

Given the **root of a binary tree**, calculate the **total number of nodes** present in the tree.

---

# ⚙️ Algorithm

The algorithm uses **recursion** to count nodes.

### Steps

1️⃣ If the root is `null`, return `0`
2️⃣ Recursively count nodes in the **left subtree**
3️⃣ Recursively count nodes in the **right subtree**
4️⃣ Add the counts and include the **current node**

Formula:

```
Total Nodes = Left Subtree Nodes + Right Subtree Nodes + 1
```

---

# 💻 Java Implementation

```java
public static int countNodes(Node root){
    if(root == null){
        return 0;
    }

    int lhCount = countNodes(root.left);
    int rhCount = countNodes(root.right);

    return lhCount + rhCount + 1;
}
```

---

# ▶️ Program Output

```
7
```

This means the binary tree contains **7 nodes**.

---

# ⏱ Time and Space Complexity

| Complexity       | Value |
| ---------------- | ----- |
| Time Complexity  | O(n)  |
| Space Complexity | O(h)  |

Where:

* **n** = number of nodes
* **h** = height of the tree (recursion stack)

---

# 🧠 Concepts Used

* 🌳 Binary Trees
* 🔁 Recursion
* 📊 Tree Traversal
* 🧮 Divide and Conquer

---

# 🎯 Learning Outcomes

After completing this program you will understand:

✔ How to recursively traverse a binary tree
✔ How to count nodes efficiently
✔ How recursion works in tree structures
✔ Basic tree algorithm design

These concepts are important for **Data Structures and Algorithms (DSA)** and **technical interviews**.

---

