# 📦 Multiple Data Compression & Encryption using Iterative Technique

## 🚀 Overview
This project implements a multi-level data compression and encryption system using an iterative technique. It focuses on reducing file size while maintaining data security and fast processing.

The system dynamically selects compression methods and applies iterative encoding and encryption to achieve efficient storage and secure data transmission.

---

## ✨ Key Features
- Multiple compression techniques (compress2 → compress7)
- Dynamic selection using function pointers
- Custom encoding with bit-length optimization
- Iterative encryption using substitution & permutation
- Efficient decoding and reconstruction
- File handling for complete pipeline
- Performance tracking using statistics module
- Bash automation for testing (logScript)

---

## 🛠️ Tech Stack
- C Programming  
- Data Structures (Arrays, Hashing)  
- Bit Manipulation  
- Linux (Ubuntu)  
- Bash Scripting  

---

## ⚙️ Project Architecture

### 📂 Core Modules

#### Compression
- compression.c
- compress2.c → compress7.c

#### Decompression
- deCompression.c
- decompress2.c → decompress7.c

#### Encoding Logic
- codelength.c
- unique.c

#### Statistics & Analysis
- compStatistics.c
- decompStatistics.c

#### Utility Functions
- findlocation.c
- openfile.c

#### Control & Flow
- main.c
- mainMenu.c
- init.c (function pointer setup)
- exitProject.c

#### Headers
- header.h
- declaration.h
- DS.h

#### Build & Automation
- Makefile
- logScript

---

## 🔄 How It Works

1. Initialization  
   Function pointers are set up in init.c  

2. Input Processing  
   File is read using openfile.c and unique characters are extracted  

3. Compression  
   codelength.c determines optimal bit size and calls compress2 → compress7  

4. Encryption  
   Applies substitution and permutation  

5. Decompression  
   Uses decompress2 → decompress7  

6. Output Reconstruction  
   Restores original file accurately  

---

## ▶️ How to Run

### Using Makefile
make  
./main  

### Manual Compilation
gcc *.c -o program  
./program  

### Run Script
bash logScript  

---

## 📊 Performance
- Compression Efficiency: 40–60% (text files)  
- Fast processing using bit-level operations  
- Secure iterative encryption  

---

## 📈 Comparison
- ZIP  
- LZW  
- AES (for benchmarking)  

---

## 📸 Sample Output
Input File: myfile.txt  
Original Size: 120 KB  

Compressed Size: 58 KB  
Compression Ratio: 51%  

Encryption Applied ✔  
Decompression Successful ✔  

---

## 🔍 Concepts Used
- Data Compression Techniques  
- Cryptography (Substitution & Permutation)  
- Function Pointers in C  
- Bitwise Encoding  
- Hash Maps  
- File Handling  

---

## 🎯 Future Improvements
- GUI-based interface  
- Support for binary files (images, videos)  
- Advanced compression (Huffman Coding)  
- Integration with AES encryption  
- Performance visualization dashboard  

---

## 👨‍💻 Author
Amaan Waris  
GitHub: https://github.com/amaanwaris
