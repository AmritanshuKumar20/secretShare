# Secret Sharing Solver using Lagrange Interpolation
# 🔐 Shamir's Secret Sharing Solver

This project implements a simplified version of **Shamir's Secret Sharing** scheme using **Lagrange Interpolation** to reconstruct the original secret from encoded shares.

## 📁 Files

- `main.js`: Main code to parse JSON and compute the secret
- `testcase1.json` and `testcase2.json`: Sample JSON inputs with keys in different bases

## 🛠️ Features

- Reads JSON input (number of shares and minimum threshold)
- Decodes values from different bases (e.g. binary, hex, base 3)
- Uses Lagrange Interpolation to recover the constant term (the secret)

## 🧪 How to Run

```bash
node main.js

