# 🚀 BitScanner 2026
yt link: https://youtu.be/HIHTRHv9vvk

contact: hacker001ethical@proton.me


## 📄 Project Description

**BitScanner 2026** is a high-performance Bitcoin private key scanning tool designed to detect matches between generated keys and a large predefined list of Bitcoin addresses. It efficiently explores vast keyspaces to find any corresponding Bitcoin addresses present in the input dataset.

The program leverages advanced techniques such as multithreading and memory-mapped file access to handle large datasets smoothly and speed up the scanning process.

---

## ⚙️ Key Features

- 🔑 **Private Key Range Scanning**  
  Systematically scans large Bitcoin private key ranges for potential matches.

- 📂 **Memory-Mapped File Support**  
  Loads and queries large sorted Bitcoin address files with minimal memory overhead.

- 🔍 **Optimized Address Lookup**  
  Uses fast search algorithms for quick verification of addresses.

- 🧩 **Compressed & Uncompressed Address Generation**  
  Generates both types of Bitcoin addresses from each private key.

- 💾 **Results Logging**  
  Saves found addresses with corresponding private keys in HEX and WIF formats.

- 🧵 **Multithreaded Processing**  
  Utilizes all available CPU cores for maximum scanning throughput.

- ⏸️ **Checkpointing & Resume**  
  Allows pausing and resuming the scan without losing progress.

- 📊 **Real-Time Progress Monitoring**  
  Displays live updates on scan progress and key generation speed.

---

## 🎯 Intended Audience

This tool is intended for:

- Security researchers  
- Blockchain analysts  
- Bitcoin enthusiasts  
- Educational and penetration testing purposes

---

## 🛠️ Requirements

- **Operating System:** Linux (recommended for full POSIX and mmap support)  
- **Compiler:** C++17 or newer compatible  
- **Libraries:**  
  - OpenSSL (for cryptographic hashing)  
  - secp256k1 (for elliptic curve operations)  
- Standard C++ and POSIX libraries

---

## 🔍 How It Works (Overview)

1. 📂 Loads a large sorted Bitcoin address list via memory-mapped file for efficient access.  
2. 📏 Divides a large private key range into steps for manageable scanning chunks.  
3. 🔑 Generates Bitcoin private keys within these ranges and derives both compressed and uncompressed public addresses.  
4. 🔎 Checks each generated address against the loaded address list to find matches.  
5. 💾 Saves any discovered matches along with their private keys securely.  
6. 🧵 Runs scanning tasks concurrently on multiple CPU threads for performance.  
7. ⏸️ Supports checkpointing to save progress and allow resuming scans seamlessly.

---

## 📢 Disclaimer

This software is for research and educational purposes only. Use responsibly and ethically.
