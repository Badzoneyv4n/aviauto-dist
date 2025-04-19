# AviAuto Distribution

**AviAuto** is a remote-controlled automation script for the Aviator casino game, designed to run in the browser using Tampermonkey.

This repository hosts the **production-ready** bundled version of AviAuto, including the necessary user scripts and update files used by Tampermonkey.

---

## 🚀 Features

- ✅ Automates Aviator tasks like:
  - Claiming rain/free bets
  - Placing wagers
  - Reloading the game
  - Sending custom notifications
- ✅ Supports multiple platforms (Fortebet, Winner, Africabet)
- ✅ Controlled remotely via Firebase
- ✅ Modular and easy to extend
- ✅ Built for scalability and maintainability

---

## 🧠 How It Works

AviAuto fetches live configuration data from Firebase Firestore and executes specific modules (claimer, wager, reloader, notifier) depending on what is enabled remotely.

This allows full control of your automation script even when you're away from your device.

---

## 🛠 Installation (via Tampermonkey)

1. Install [Tampermonkey](https://tampermonkey.net/)
2. Create a new script
3. Paste the following:

```js
// ==UserScript==
// @name         AviAuto (Remote Controlled)
// @namespace    https://avi-auto.badzone.rw
// @version      1.0.0
// @description  Firebase-controlled Aviator automation by Badzone 🧠
// @author       Badzone
// @match        https://aviator-next.spribegaming.com/*
// @grant        GM_notification
// @grant        GM_setValue
// @grant        GM_getValue
// @require      https://cdn.jsdelivr.net/gh/Badzoneyv4n/aviauto-dist@main/dist/aviauto.bundle.js
// ==/UserScript==

(() => {
    // The main logic is handled inside the bundled script.
})();
```

## 📁 Repository Structure

dist/
└── aviauto.bundle.js       # Minified and bundled logic
└── aviauto.secure.js       # (Optional) Obfuscated version for production

## ⚠️ Disclaimer
This script is for educational and research purposes only. Use at your own risk. Always comply with the terms and conditions of any platform you interact with.

#### 🧑‍💻 Author
Made with 🚀 by Badzone yv4n
For questions, contact: [Github](https://github.com/Badzoneyv4n/)
