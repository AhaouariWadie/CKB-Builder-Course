# Weekly Progress Report
**Week:** 10 July 2025 – 16 July 2025  
**Author:** Ahaouariwadie (GitHub username)

---

## Summary of Activities

### Thursday, 10 July 2025
- Started learning JavaScript objects using FreeCodeCamp.
- Practiced accessing and modifying object properties using dot and bracket notation.
- Learned how to use objects for flexible data storage.

### Friday, 11 July 2025
- Practiced writing functions that access and return object data.
- Solved FreeCodeCamp challenges on nested objects and arrays.
- Explored how recursion can replace loops in object traversal.

### Saturday, 12 July 2025
- Introduced to JavaScript classes syntax using `class` and `constructor`.
- Practiced creating objects from classes and using `this` keyword.
- Understood difference between object literals and class instances.

### Sunday, 13 July 2025
- Learned how to create methods inside JavaScript classes.
- Practiced using getters, setters, and method chaining.
- Completed class-based exercises and read external examples for clarity.

### Monday, 14 July 2025
- Installed CKB JavaScript SDK libraries using:
  ```bash
  npm install @nervosnetwork/ckb-sdk-core @nervosnetwork/ckb-sdk-rpc blake2b
  ```
- Explored `CKB`, `Address`, and `Script` classes from the SDK.
- Initialized a connection to a testnet RPC node.

### Tuesday, 15 July 2025
- Built a basic transaction using JavaScript SDK.
- Loaded testnet private key using SDK’s `Key` module.
- Used `rpc.getCells` and `rpc.sendTransaction` to gather inputs and broadcast a transaction.

### Wednesday, 16 July 2025
- Analyzed code structure of transaction scripts using JavaScript.
- Reviewed the relationship between cell capacity and contract binary size.
- Researched how to compute contract `code_hash` and reuse deployed smart contracts on-chain.

---

## Challenges & Notes
- Distinguishing between object methods and class instance methods took practice.
- Understanding CKB SDK’s abstractions (cells, scripts, capacity) required combining doc reading and trial runs.
- Debugging JavaScript SDK errors was easier with proper logging and Chrome dev tools.

## Goals for Next Week
- Continue building more complex transactions with JavaScript SDK.
- Begin preparing a custom script for deployment on devnet.
- Learn how to sign and validate transactions using custom lock scripts.
---
