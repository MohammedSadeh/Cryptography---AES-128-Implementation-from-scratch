# AES-128 CBC Implementation and Analysis

This repository contains my implementation for **ENCS4320 – Applied Cryptography Course (Task #2)** at Birzeit University.  
The project focuses on building AES-128 encryption and decryption **from scratch** (without relying on external libraries for the core steps) and analyzing its behavior under different scenarios.


## Features
- **AES-128 Core Implementation**
  - SubBytes / InvSubBytes
  - ShiftRows / InvShiftRows
  - MixColumns / InvMixColumns
  - AddRoundKey
  - Key Expansion (Round Key Generation)

- **CBC Mode Integration**
  - AES-CBC encryption and decryption
  - Supports arbitrary plaintext length
  - User-provided 128-bit IV

- **Interactive Runner Script**
  - Select Encrypt/Decrypt
  - Input plaintext/ciphertext, key, and IV in hexadecimal
  - Outputs result in hexadecimal

- **Avalanche Effect Analysis**
  - Random bit flips in plaintext and key
  - Repeated experiments with result summary
  - Visualization of diffusion strength

- **Extended Analysis**
  - Bit error in ciphertext and its impact on decryption
  - Loss of ciphertext block in CBC mode
  - Data exposure analysis using encrypted images

---

## 📂 File Structure
      ├── Project Document               # Requirement for the task
      ├── Project Report                 # Final Report for this task contains the results
      ├── src                             # code 
          ├── task2_aes.py                         #the core functions for AES and CBC
          ├── task2_run_aes.py                     # Interactive runner script
          ├── task2_aes_avalanche_analysis.py      # Avalanche effect experiments
          └── task2_data_exposure_image.py         # Images Analyzing with CBC mode of operation
      ├── images
          ├── ciphertext_visual_cbc.png                         #the core functions for AES and CBC
          ├── image.bmp  
      └── README.md                      # Documentation
