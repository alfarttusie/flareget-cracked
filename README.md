# 🔓 Assembly-Level Patching — FlareGet

> ## **⚠️ Legal Disclaimer**  
> #### This project is for **educational purposes only**. It demonstrates how software protection mechanisms work and how they can be analyzed using reverse engineering techniques.  
> #### It does **not** promote or condone software piracy or the use of unlicensed software. Use responsibly and only on software you legally own.

---

## 📦 Overview
#### This repository contains a patched version of the download manager **FlareGet**, where its license verification mechanism has been bypassed via **assembly-level modifications**.  
#### The binary was analyzed and modified using **radare2**, targeting the license check routine and altering it to bypass activation.

---

## 🧠 What Was Done

#### - Reverse engineered the binary with `radare2`
#### - Located the license check function and conditional jump
#### - Modified jump logic (e.g., `JNZ` → `JMP`) or replaced checks with `NOP`
#### - Saved the patched binary

---

## 🚀 How to Use
#### 1. INSTALL THE OFFICIAL VERSION
#### 2. Clone this repository:
   ```bash
   git clone https://github.com/alfarttusie/flareget-cracked.git

   cd flareget-cracked

   sudo mv flareget /usr/bin/flareget

   sudo chmod +x /usr/bin/flareget

### launch flareget

Go to Help > Register.

Enter any name, email, and license key — anything will work.

✅ Done! FlareGet is now activated.

# 🛠 Tools Used

###    radare2 — for binary analysis and patching

###    Linux terminal utilities (mv, chmod)

###    Hex-level editing (internally done by radare2)

# 📝 Notes

###    Always back up your original flareget binary before replacing it.

###    This patch works on the specific version 5.0.0 tested. Future updates may break it.

###    If you want to apply the patch manually, you can inspect the binary in radare2 and follow the same logic used here.

# 📅 Author

###    Modified by: @alfarttusie
###    Tool used: radare2
###    Year: 2025
