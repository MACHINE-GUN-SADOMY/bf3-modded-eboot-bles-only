# BF3 Revival Trainer (PS3)

## 🧠 Overview
**BF3 Revival Trainer** is a PlayStation 3 trainer developed for **Battlefield 3** using **TMAPI** on **DEX consoles**.  
It is intended for **offline testing, debugging, and reverse-engineering purposes**.

The project focuses on **PowerPC opcode patching** rather than traditional variable manipulation.

---

## ✨ Features
- TMAPI connect and attach
- PowerPC instruction patching
- Toggleable game modifications  
  *(UAV, Wallhack, NameTags, No Recoil, etc.)*
- Original opcode restoration (safe OFF state)
- Simple WinForms GUI (C++/CLI)

---

## 📋 Requirements
- PlayStation 3 **DEX**
- **Target Manager** running on PC
- TMAPI (x86)
- Debug settings enabled on the PS3
- Battlefield 3 *(offline recommended)*

---

## 🔍 Offsets & Research
- Base offsets referenced from:  
  👉 https://consolecrunch.com/threads/battlefield-3-offsets-1-9.30783/

- Original **OFF values (restore opcodes)** were identified using the  
  **Target Manager Debugger**, by inspecting PowerPC instructions at runtime.

All addresses and opcodes are centralized in a dedicated header file for easier maintenance and version updates.

---

## ⚙️ How It Works
1. Connects to the PS3 via **TMAPI**
2. Attaches to the Battlefield 3 process
3. Writes PowerPC instructions directly into memory
4. Restores original instructions when disabling features

---

## ⚠️ Notes
- This project does **not** use CCAPI
- TMAPI attach timing is critical
- Designed for learning and experimentation
- Online usage is **not recommended**

---

## 📜 Disclaimer
This project is for **educational and research purposes only**.  
The author is not responsible for any misuse.