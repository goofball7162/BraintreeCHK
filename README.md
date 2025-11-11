<h1 align="center">BraintreeCHK</h1>

<p align="center">
  <b>Card checker gates braintree VBV lookup (3D Check's)</b>
</p>

<p align="center">
  <a href="https://www.python.org/">
    <img src="https://img.shields.io/badge/Python-3.12%2B-blue?logo=python&logoColor=white" alt="Python 3.12+">
  </a>
  <a href="https://github.com/KianSantang777/BraintreeCHK">
    <img src="https://img.shields.io/github/stars/KianSantang777/BraintreeCHK?style=social" alt="GitHub Stars">
  </a>
  <a href="https://github.com/KianSantang777/BraintreeCHK">
    <img src="https://img.shields.io/github/forks/KianSantang777/BraintreeCHK?style=social" alt="GitHub Forks">
  </a>
  <a href="https://github.com/KianSantang777/BraintreeCHK/blob/main/LICENSE">
    <img src="https://img.shields.io/badge/License-Proprietary-red" alt="License">
  </a>
  <a href="https://t.me/xqndrs">
    <img src="https://img.shields.io/badge/Contact-Telegram-blue?logo=telegram" alt="Telegram">
  </a>
</p>

---

## Jump To
- [Overview](#braintreechk)
- [How BraintreeCHK Works](#how-braintreechk-works)
- [Features](#features)
- [System Requirements](#system-requirements)
- [Installation Guide](#installation-guide)
  - [1. Clone the Repository](#1-clone-the-repository)
  - [2. Install Dependencies](#2-install-dependencies)
    - [Windows](#windows)
    - [Termux-android](#termux-android)
  - [3. Run the Script](#3-run-the-script)
- [Repository](#repository)
- [Author](#author)
- [License](#license)

---

## How BraintreeCHK Works

**BraintreeCHK** is a lightweight Python tool for mass BIN card verification using the Braintree API.  
It automatically performs **VBV (Verified by Visa)** and **3D Secure lookups** to determine card validity and authentication support.  
Using Braintree’s gateway, the tool checks whether each card supports VBV or 3D Secure, and identifies those that are active, require authentication, or are invalid.

During verification, Braintree communicates with Visa to retrieve key parameters such as:  
- `liabilityShiftPossible` — indicates if fraud liability can shift to the issuer  
- `liabilityShifted` — confirms if liability has shifted  
- `status` — e.g., `authenticate_successful`, `attempt_successful`, or `failed`  

Results are automatically classified as **LIVE** (valid) or **DEAD** (invalid).  
Fully compatible with **Windows** and **Termux (Android)** for fast, automated mass checking.

<p align="center">
  <img src="https://raw.githubusercontent.com/KianSantang777/BraintreeCHK/refs/heads/main/pic/pict%201.png" alt="BraintreeCHK Preview 1" width="70%" style="border-radius:10px; margin:10px 0;">
  <br>
  <img src="https://raw.githubusercontent.com/KianSantang777/BraintreeCHK/refs/heads/main/pic/pict%202.png" alt="BraintreeCHK Preview 2" width="70%" style="border-radius:10px; margin:10px 0;">
</p>

---

## Features
- Built with **Python 3.12.0**  
- Supports all devices  
- Automatically saves **LIVE cards** in real time  
- Supports both **proxy** and **proxyless** modes  
- Automatically rotates **user agents** for improved security  
- Utilizes **5 concurrent threads** for faster validation  
- **Green text (output)** = LIVE card  
- **Red text (output)** = DEAD card  
---

## System Requirements
- **Python 3.12.0** or higher  
- **pip** `requests, colorama, psutill distro, bs4, fake, pyfiglet, urllib3`
- Active internet connection
---

## Installation Guide
```bash
# Termux (Android)
- termux-setup-storage
- pkg update && pkg upgrade
- pkg install python git nano -y

# Clone the repository
- git clone https://github.com/KianSantang777/BraintreeCHK.git
- cd BraintreeCHK
- pip install --upgrade pip
- chmod +x run.sh
- ./run.sh
```
---
## Repository
[![GitHub Repo](https://img.shields.io/badge/GitHub-BraintreeCHK-blue?logo=github)](https://github.com/KianSantang777/BraintreeCHK)
[![Stars](https://img.shields.io/github/stars/KianSantang777/BraintreeCHK?style=social)](https://github.com/KianSantang777/BraintreeCHK/stargazers)
[![Forks](https://img.shields.io/github/forks/KianSantang777/BraintreeCHK?style=social)](https://github.com/KianSantang777/BraintreeCHK/network/members)

**Repository:** [github.com/KianSantang777/BraintreeCHK](https://github.com/KianSantang777/BraintreeCHK)

---
## Author
**Kian Santang**  
GitHub: [@KianSantang777](https://github.com/KianSantang777)  
Telegram: [xqndrs](https://t.me/xqndrs)

---

## License
[![License](https://img.shields.io/badge/License-Proprietary-red)](LICENSE.md)
[![Subscription](https://img.shields.io/badge/Subscription-Required-orange)](https://t.me/xqndrs)

This software is **proprietary** and requires an **active monthly subscription** to use.  
Unauthorized copying, redistribution, or modification of the code is strictly prohibited.  
For license purchase or renewal, please contact **[@xqndrs](https://t.me/xqndrs)** on Telegram.

© 2025 **Kian Santang** — All Rights Reserved.
