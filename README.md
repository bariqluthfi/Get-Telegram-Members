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
- ✅ Hard‑coded daily limit of 100 members  
- ✅ Waits 3 hours after limit before continuing  
- ✅ Runs 24×7 without disconnecting session  
- ✅ Simple CLI with only three commands  

---

📥 Preparing Your Numbers List

To use the bot, you’ll need a file of Telegram phone numbers.  
You can create your `users.txt` file using the following link:
# Create users.txt
👉🏻 https://globalphone.wasmer.app
  
Save the file in the project root, with one number per line:

```
+919876543210
+14155552671
+447911123456
```

⚠️ Important: Only verified Telegram numbers will be kept after running `/verify`.

---

📦 Installation & Setup

1️⃣ Install packages

```bash
pkg update -y && pkg install git nodejs -y && npm install -g yarn
```

2️⃣ Clone the Repository

```bash
git clone https://github.com/amanmohdtp/Get-Telegram-Members.git &&
cd Get-Telegram-Members
```

3️⃣ Install Dependencies

```bash
yarn install
```

---

🔧 Interactive Config

On first run, you’ll be asked for:

- 📱 Your own Telegram number  
- 🔑 API ID  
- 🔑 API Hash  
- 🎯 Target group link  

These values are saved into `config.json` automatically.  
No need to edit files manually.

---

▶️ Run the Bot

Start the bot manually:

```bash
yarn start
```

---

💻 Bot Commands (CLI)

- 🔍 Verify numbers
  ```bash
  /verify
  ```
  Removes non‑Telegram users from `users.txt` and keeps only valid accounts.

- ➕ Add verified members
  ```bash
  /add
  ```
  Adds verified members to the target group with 10s delay.  
  After 100 members, waits 3 hours before continuing automatically.

- 📊 Check status
  ```bash
  /status
  ```
  Shows current time, number of verified accounts, and lists all commands.

---

⚠️ Important Notes

- Only valid Telegram numbers are processed  
- Users with strict privacy settings may be skipped  
- Daily limit of 100 enforced automatically  
- Bot session stays alive 24×7, even during wait periods  

---

🛠 Development Info

- 🟢 Built with Node.js  
- 📦 Powered by GramJS  
- 🧶 Dependency management via Yarn  
- 💻 Cross‑platform: Linux, macOS, Windows, Android (Termux)  

---

<p align="center">
  <img src="https://media.giphy.com/media/26AHONQ79FdWZhAI0/giphy.gif" width="300" />
</p>
