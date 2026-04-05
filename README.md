AI WAS USED TO CREATE THIS

# ContactVerify 🔐

![Status](https://img.shields.io/badge/status-hobbyist-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Browser](https://img.shields.io/badge/browser-Chrome%2FFirefox%2FEdge-lightgrey)

**ContactVerify** is a lightweight, client-side verification tool for sharing time-limited, contact-specific codes (PV1 codes) between trusted users. Perfect for hobby projects, friends, or small groups who want a simple way to confirm identities or exchange ephemeral secrets without a server.  

> ⚠️ **For trusted users only — not for production or sensitive data.**

---

## Features

- 🔐 **Encrypted Vault**: Contacts and secrets stored locally in the browser using AES-GCM encryption.  
- 👤 **Contact-Specific Codes**: Generate PV1 codes tied to a specific contact, with expiry times.  
- ⏱ **Expiry Enforcement**: Codes expire after 5 min, 15 min, 1h, or 24h.  
- 🛠 **Offline & Client-Side**: Fully functional in your browser, no server required.  
- 🗂 **Unique IDs**: Each contact has a unique ID to allow duplicate names safely.  
- 📋 **Copy-to-Clipboard**: One-click copy for PV1 codes.  
- 💻 **Responsive UI**: Works on both desktop and mobile.  

---

## How It Works

1. **Add Contacts**: Each contact has a name, secret, and unique ID.  
2. **Generate PV1 Codes**: Codes include the contact ID, name, and expiry, signed with HMAC using the contact’s secret.  
3. **Verify Codes**: PV1 codes can be verified to ensure validity for the correct contact and check expiry.  

---

## Getting Started

1. Download or clone this repository.  
2. Open `ContactVerify.html` in your browser (Chrome, Firefox, or Edge recommended).  
3. Set a master password, add contacts, and generate PV1 codes!  

---

## Limitations

- Designed for **trusted users only**.  
- **Vault password is critical**: losing it means losing all contacts.  
- **Replay attacks**: PV1 codes can be reused until expiry.  
- Stored locally in browser `localStorage` — may be accessed if your device is compromised.  

---

## Contributing

Feel free to fork, open issues, or submit pull requests! This project is a hobbyist verification tool and designed for experimentation.  

---

## License

[MIT License](LICENSE)
