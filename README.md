First Create KEY TOP account via link https://www.key.top/#/pages/index/index/?k=SEVX1DGR

```markdown
# 🤖 Keytop Referral & Auto-Mining Bot

This bot allows you to:
- Automatically register Keytop accounts using [Temp Mail](https://mail.tm)
- Use your referral link (`?k=YOURCODE`)
- Automatically click the “Start Mining” button
- Repeat the mining process every 24 hours
- Run efficiently on a VPS (headless)

---

## ✨ Features

✅ Register Keytop accounts with disposable email  
✅ Auto-fill referral code via link  
✅ Auto click the "Start Mining" button  
✅ Scheduled mining every 24 hours  
✅ Supports bulk account creation  
✅ Stores email & password in `akun.json`

---

## 📁 Project Structure

```

keytop\_bot/
├── main.py           # Account registration
├── miner.py          # Auto-mining logic
├── tempmail.py       # Handles mail.tm account creation
├── utils.py          # Password generator & account storage
├── akun.json         # Stores generated accounts

````

---

## 🚀 How to Use (VPS / Ubuntu)

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/keytop-bot.git
cd keytop-bot
````

### 2. Install Dependencies

```bash
sudo apt update
sudo apt install python3 python3-pip unzip chromium-browser -y
pip3 install selenium schedule undetected-chromedriver
```

### 3. Register Accounts

Open `main.py` and edit:

```python
referral = "SEVX1DGR"  # Replace with your own referral code
jumlah = 3             # Number of accounts to create
```

Run the bot:

```bash
python3 main.py
```

---

## ⛏️ Run Auto-Mining Every 24 Hours

```bash
python3 miner.py
```

To keep the bot running in the background, use `screen`:

```bash
sudo apt install screen
screen -S keytopminer
python3 miner.py
# Press Ctrl+A then D to detach
```

To return:

```bash
screen -r keytopminer
```

---

## 📝 Important Notes

* `akun.json` stores all generated emails and passwords
* Keep this file secure and **do not upload** it publicly
* If the Keytop website changes, you may need to update XPaths in `main.py` or `miner.py`
* Temp mails are disposable; they may expire after 24 hours

---

## 🔒 Recommended .gitignore

To prevent sensitive files from being pushed:

```
__pycache__/
*.pyc
akun.json
.env
```

---

## 📮 Contact

Made by \[Your Name].
Feel free to open an issue or PR if you have suggestions or improvements!

```

---

Let me know if you want me to:
- Insert your GitHub username into the repo URL
- Replace `[Your Name]` with your real name or alias
- Automatically include this README in your `keytop_bot.zip`

Ready to go?
```
