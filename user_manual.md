# ☕ BrewKey - User Manual

Welcome to **BrewKey**, your personal, secure password brewer.

No more forgotten passwords, no more insecure notes. BrewKey gives you **secure**, **repeatable**, and **instant** passwords with just **one master password** to remember.

---

## What is BrewKey?

BrewKey is a **deterministic password generator**:  
It creates the same secure password every time you input the same **identifier** and **master password** — without saving anything anywhere.  
Your data stays **private**, **local**, and **uncompromised**.

---

## Why use BrewKey?

✅ **No need to remember multiple passwords** — just your master password.  
✅ **No data storage** — nothing is saved, nothing is at risk if you lose your device.  
✅ **Cross-platform** — Works on Windows (GUI), Android (soon), and console (Python).  
✅ **Offline** — No internet needed, no tracking, no leaks.  
✅ **High security** — Based on SHA-256 hashing and strong deterministic techniques.  
✅ **Instant results** — Generate your password in seconds.

---

## How does it work?

Simply provide two pieces of information:
- An **Identifier**: the service or site name (e.g., "gmail", "banking", "work_email").
- Your **Master Password**: the single password you must memorize.

BrewKey will instantly generate a unique, strong password specific to that identifier.  
Every time you enter the same two inputs, you get the exact same password.

---

## Getting Started

### 🖥️ Windows Application

1. Launch `generateur_mdp23-2.exe` (found in `/windows/`).
2. Enter:
    - **Identifier** (e.g., `facebook`)
    - **Master Password** (e.g., `My$trongP@ssw0rd!`)
3. Click **"Generate"**. or Press **Enter** to generate and copy your new password.
4. Your password is displayed (masked by default) and copied to the clipboard for easy use!

Toggle visibility if you want to see the password.  
Clipboard support lets you paste it directly.

---

### 💻 Console (Python)

If you prefer using the terminal:

1. Make sure you have **Python 3.9+** installed.
2. Open a terminal and run:
   ```bash
   python main.py
    ```
3. Enter your Identifier and Master Password when prompted.

Your secure password will appear directly in the console.

---

## 📱 Android Version (Coming Soon!)

- The mobile app is under development and will follow the same logic:

    - Minimalist design.

    - Instant password generation.

    - Fully offline and secure.

> For now, use the console version `main.py` on an application that interprets Python.
---

## Best Practices

- Choose a strong, **memorable** master password.

- Use **consistent** identifiers (e.g., **always** write "Gmail" the **same way**).

- Back up your master password securely, it's your only key.

- Use different identifiers for different services (e.g., "gmail" vs. "github").

- Write down your identifiers somewhere or follow a single pattern (e.g., a capital letter followed by the name of the site "Github")

---

## FAQ

Q: What happens if I lose my master password?    
A: You won't be able to regenerate your **master passwords**. It's essential to securely memorize or back up your master password.

Q: Can someone guess my password if they find my identifier?    
A: No. Without your master password, the output remains cryptographically secure.

Q: Are my passwords stored somewhere?    
A: No. BrewKey does not store any passwords, identifiers, or master password information — everything is calculated on the fly.

Q: Is BrewKey open-source?    
A: Yes! You can review the source code anytime on GitHub to verify its security and behavior.

---

## Support

If you encounter bugs, have ideas for improvements, or just want to contribute:

- Visit our GitHub repository : [github.com/TheoHUETQC/password-generator/](https://github.com/TheoHUETQC/password-generator/)

- Submit issues or pull requests!

- My personal contact : `theo6huet@gmail.com`

---

## Personal comment

> I use this software myself on a daily basis. It's simple and bug-free. I no longer write down any of my passwords, just my identifiers in an Excel spreadsheet. My master password is stored in my head, and that works perfectly for me.

## ☕  Brew smarter. Stay safer. with BrewKey.
