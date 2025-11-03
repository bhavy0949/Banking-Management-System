# 🏦 Bank Management System

> **A comprehensive banking application using client-server architecture with concurrency and data integrity using file locking, semaphores, `fork` and system calls in C.**

---

### 📜 Project Overview

This **Bank Management System** simulates real-world banking operations, allowing customers, bank employees, and administrators to interact securely. Designed with **client-server socket programming**, the system ensures concurrent operations while preserving data consistency through techniques like **file locking**, **semaphores**, **multithreading**, and **inter-process communication**.

### 🌟 Features

1. **Role-Based Access Control**:
   - **Customer**: Account details, transaction history, loan application and fund transfers.
   - **Bank Employee**: Customer management and loan processing.
   - **Manager/Administrator**: Oversee transactions, accounts, and ensure data integrity.
  
2. **Concurrency & Synchronization**:
   - **File Locking**: Prevents data corruption in concurrent transactions.
   - **Socket Programming**: Efficient communication between client and server.
   - **System Calls**: Enhanced control and performance.
  
3. **Data Integrity**:
   - **Logging System**: Synchronized logs for system auditing and troubleshooting.
   - **Fork and Semaphores**: Ensures concurrent processes with shared resources.

---

### 🚀 Getting Started

#### Prerequisites
- GCC Compiler
- Linux Environment

#### Installation & Setup

1. **Clone the Repository**
   ```bash
   git clone https://github.com/imrds7/Software-systems-Project.git
   cd Software-systems-Project
2. **Compile the code**
   ```bash
   gcc server.c -o server -L/lib/x86_64-linux-gnu/libcrypt.so -lcrypt -pthread
   gcc client.c -o client
3. **Run the server**
   ```bash
   ./server
4. **Run the client**
   ```bash
   ./client
