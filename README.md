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

File Structure
shamir-secret-sharing/ ├── shamir_secret.js # Main program file ├── testcase1.json # First test case (auto-generated) ├── testcase2.json # Second test case (auto-generated) ├── README.md # This file └── package.json # Optional: Node.js package configuration

We need k = m + 1 points to uniquely determine the polynomial
The secret is the constant term 'c' = f(0)
Lagrange interpolation reconstructs the polynomial from given points
Error Handling
The program includes error handling for:

Invalid JSON format
Base conversion errors
File reading errors
Mathematical computation errors
Constraints
All coefficients are positive integers
Coefficients are within 256-bit number range
n ≥ k (sufficient roots provided)
Supports bases from 2 to 16
Contributing
Fork the repository
Create a feature branch (git checkout -b feature/improvement)
Commit changes (git commit -am 'Add improvement')
Push to branch (git push origin feature/improvement)
Create Pull Request
License
This project is created for educational purposes as part of a placement assignment.

Assignment Submission
Language: JavaScript (Python not allowed)
