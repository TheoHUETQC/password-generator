# ☕ BrewKey - Your Everyday Cup of Secure Passwords

## Simple. Secure. Instant.

Tired of remembering countless passwords?  
Sick of writing them down or creating confusing variations?

**BrewKey** brings you a smarter, simpler solution:  
Just remember **one master password** and **your identifiers**, BrewKey will handle the rest.

With BrewKey, you'll **never need to store** or **write down** your passwords again.  
Your new password vault is your own memory, powerful, secure, and ultra-practical.

![logo](logo/logo.ico)

---

## Why BrewKey? 

- **Forget remembering dozens of passwords** - Just the name of the site as the identifier and a unique master password are enough.
- **No database, no cloud storage** - Nothing is ever saved.  
- **Mathematically guaranteed** - Thanks to strong deterministic algorithms (SHA-256).
- **Ultra-simple to integrate into your daily routine** - Works seamlessly, whether you need 1 password or 100.
- **No risk if you lose your device** - Passwords can always be regenerated.
- **Private and offline** - Your data never leaves your device.

In short:  
✅ **No storage**  
✅ **No sync needed**  
✅ **No leaks**  
✅ **Total peace of mind**

---

## How to use BrewKey :

Enter:    
    - **Identifier** (e.g., `Github`)    
    - **Master Password** (e.g., `My$trongP@ssw0rd!`)    

Click **"Generate"** and copy your new password for Github !    

**All details in this .md file :** [User Manual](user_manual.md)


---

## Features

- **Deterministic password generation** using SHA-256 encryption
- **Zero storage** - passwords are generated on the fly
- **Windows GUI app** (.exe ready : `/windows/generateur_mdp23-2.exe`)
- **Android GUI app** (in progress)
- **Console version** `main.py` for advanced users or integration 
- **Clipboard copy** feature in the GUI
- **Masked/unmasked password display** for privacy
> In future versions, users will be able to choose the password length directly in the .exe file for greater simplicity. They will also be able to choose between dark and light modes.
---

## Project Structure

```
📂 password-generator/ 
├── main.py                          → Console version (Python) 
│ 
├── 📂 windows/ 
│    ├── WindowsPassWordGenerator.py → GUI app (Tkinter) 
│    └── generateur_mdp23-2.exe      → Windows executable 
│ 
├── 📂 android/ 
│    └── generateur_mdp_android.py   → Android GUI (in development) 
│ 
├── 📂 logo/ 
│    ├── logo.png                    → App icon 
│    └── logo.ico                    → Executable icon 
│
├── 📄 user_manual.md               → how to use brewkey
│
└── 📄 README.md (You're here!)
```

---

## How BrewKey Works (Under the Hood)
- Secure hash computation of your identifier and master password using SHA-256.

- Mathematical mixing and deterministic slicing to create a unique hint list.

- Character mapping onto a custom alphabet, ensuring high randomness and strength.

- Fixed output length (e.g., 23 characters) for consistency.

Result?
The same input will always generate the same password — without storing anything.

```py
int(hashlib.sha256(value.encode('utf-8')).hexdigest(), 16)  # Secure hash
# Followed by transformations to select characters
```
---

## Requirements

- **Python 3.9+**

- Only standard libraries:

    - hashlib

    - tkinter (for Windows GUI)

    - kivy (for Android GUI)

nstall needed packages (if needed):
```bash
pip install hashlib tkinter kivy
```

---

## Versioning

Naming format:

- ``generateur_mdp23-2.exe``

    - Generates 23-character passwords
    - Version 2 of the app

> In future versions, users will be able to choose the length of their password for greater simplicity. This format will be discontinued.

---

## Contributions & Ideas

Ideas, feedback, bugs, feel free to:

- Suggest features
- Report issues
- Submit pull requests

Let's make password management easier for everyone!

---

## ☕ Brew smarter. Stay safer.
