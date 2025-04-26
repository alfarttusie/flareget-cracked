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

### 1. Install FlareGet (Official Version)

- Download and install FlareGet from the [official website](https://flareget.com/).

### 2. Replace Binary with Patched Version

Clone this repository and replace the official binary with the patched one:

```bash
git clone https://github.com/alfarttusie/flareget-cracked.git
cd flareget-cracked
sudo mv flareget /usr/bin/flareget
sudo chmod +x /usr/bin/flareget
```

### 3. Launch and Activate FlareGet

- Open FlareGet.
- Go to `Help` → `Register`.
- Enter **any** name, email, and license key — anything will work.

✅ **Done! FlareGet is now activated.**

---

## 🛠 Tools Used

- **radare2** — binary analysis and patching.
- **Linux terminal utilities** (`mv`, `chmod`).
- **Hex-level editing** (handled internally by radare2).

---

## 📝 Notes

- Always **back up** your original FlareGet binary before replacing it.
- This patch has been tested specifically on **version 5.0.0**. Future updates may break it.
- To apply the patch manually, inspect the binary using radare2 and follow the logic described here.

---

## 📅 Author

- **Modified by:** [@alfarttusie](https://github.com/alfarttusie)  
- **Tool used:** radare2  
- **Year:** 2025
