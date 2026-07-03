# PIN Strength Validator (C++ Logic Implementation)

## 📌 Project Overview
This repository contains a core C++ program designed to validate the strength of a 4-digit PIN based on specific algorithmic patterns. It demonstrates sequential logic, conditional branching (`if-else`), and modular arithmetic in C++.

## 🔍 How the Algorithm Works
The program takes a 4-digit sequence as characters, converts them to integers, and evaluates them against two "Weak" criteria:
1. **Identical Digits:** Checks if all four digits are exactly the same (e.g., `7777`).
2. **Sequential Digits (Circular):** Checks if the digits follow a consecutive ascending pattern, accounting for the wrap-around from 9 to 0 using the modulus operator `(current_digit + 1) % 10` (e.g., `1234` or `8901`).

If the input matches neither of these weak patterns, it is classified as **Strong**.

## 🚀 How to Compile and Run
Ensure you have a C++ compiler installed (like `g++`). Run the following commands in your terminal:
```bash
g++ -O3 main.cpp -o validator
./validator
