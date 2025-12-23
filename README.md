<p align="center">
  <img src="https://media.giphy.com/media/3o7TKMt1VVNkHV2PaE/giphy.gif" width="120" />
</p>

<h1 align="center">🚀 GramJS Telegram Member Adder Bot</h1>

<p align="center">
  <b>A GramJS-based Telegram bot to invite users into groups using phone numbers</b><br>
  Optimized for <b>Termux (Android)</b> & <b>Linux</b> using <b>Yarn</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Node.js-v18+-green">
  <img src="https://img.shields.io/badge/GramJS-Latest-blue">
  <img src="https://img.shields.io/badge/Platform-Termux%20%7C%20Linux-orange">
  <img src="https://img.shields.io/badge/Status-Stable-success">
</p>

---

✨ Features

- ✅ Add users to Telegram groups using phone numbers  
- ✅ Automatic verification of numbers before adding  
- ✅ Fixed 10s delay between adds  
- ✅ Hard-coded daily limit of 100 members  
- ✅ Waits 3 hours after limit before continuing  
- ✅ Runs 24×7 without disconnecting session  
- ✅ Simple CLI with only three commands  

---

📥 Preparing Your Numbers List

To use the bot, you’ll need a file of Telegram phone numbers.

**Create users.txt:**  
[![Create users.txt](https://img.shields.io/badge/Create-users.txt-blue?style=for-the-badge)](https://globalphone.wasmer.app)

Save the file in the project root, with one number per line:

`
+919876543210 +14155552671 +44791112345
`

⚠️ Only verified Telegram numbers will be kept after running `/verify`.

---

🔑 Get Telegram API ID & API Hash

You must generate your own API credentials from Telegram.

**Open Telegram Developer Portal:**  
[![Telegram Developers](https://img.shields.io/badge/Open-Telegram%20Developers-2CA5E0?style=for-the-badge&logo=telegram)](https://my.telegram.org)

**Steps:**
1. Open the link above  
2. Log in with your Telegram phone number  
3. Choose **API development tools**  
4. Fill in:
   - App title (any name)
   - Short name (any)
   - Platform: Desktop / Android
5. Submit the form  
6. Copy your **API ID** and **API Hash**

These will be requested automatically on first run and saved to `config.json`.

---

📦 Installation & Setup

1️⃣ Install packages (Termux):
```copy
pkg update -y && pkg install git nodejs -y && npm install -g yarn
```

Clone Repository:


```copy
git clone https://github.com/amanmohdtp/Get-Telegram-Members.git &&
cd Get-Telegram-Members
```

Install dependencies:

```copy
yarn install
```

---

🔧 Interactive Config

On first run, the bot asks for:

📱 Your Telegram number

🔑 API ID

🔑 API Hash

🎯 Target group link


Saved automatically to config.json.


---

▶️ Run the Bot

```copy
yarn start
```

---

💻 Bot Commands (CLI)

🔍 Verify numbers

`
/verify
`

Removes non-Telegram users from users.txt.

➕ Add verified members

`
/add
`

Adds members with 10s delay.
After 100 users, waits 3 hours automatically.

📊 Check status

`
/status
`

Shows current time, verified count, and commands list.


---

⚠️ Important Notes

Only valid Telegram numbers are processed

Users with strict privacy settings may be skipped

Daily limit of 100 enforced automatically

Session stays alive 24×7


---
<p align="center">
  <img src="https://media.giphy.com/media/26AHONQ79FdWZhAI0/giphy.gif" width="300" />
</p>
---

🛠 Development Info

🟢 Node.js

📦 GramJS

🧶 Yarn

💻 Linux | macOS | Windows | Android (Termux)
