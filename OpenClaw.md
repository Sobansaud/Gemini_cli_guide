# 🚀 Welcome To CodeVerse Soban

👍 Like & Subscribe for more amazing tutorials!

---

# 🚀 OpenClaw Tutorial – Installation & WhatsApp Integration

Learn how to install OpenClaw from scratch and connect it with WhatsApp to create your own AI Employee.

---

## 📌 What You Will Learn

- Install OpenClaw (step-by-step)
- Fix common installation errors
- Connect WhatsApp (QR method)
- Send your first message
- Understand the core setup pattern

---

## ⚙️ Requirements

- Node.js v22+
- Terminal / PowerShell
- Google Account
- WhatsApp / Telegram / Discord

---

## 📥 Step 1: Install OpenClaw

### Windows (Run PowerShell as Admin)

```powershell
iwr -useb https://openclaw.ai/install.ps1 | iex
```

### What happens:
- Installs dependencies
- Sets up OpenClaw
- Starts setup wizard

---

## 🔁 Fallback Install

```bash
npm install -g openclaw@latest
openclaw
```

Restart wizard:
```bash
openclaw setup --wizard
```

---

## 🔐 Security Notice

⚠️ Always read warnings carefully before continuing setup.

---

## 🧠 AI Setup

Recommended model:
```
google/gemini-3.1-flash-lite-preview
```

---

## 💬 Step 2: WhatsApp Integration

- Open WhatsApp
- Settings → Linked Devices
- Scan QR code from terminal

---

## ⚙️ Recommended Settings

- Phone: Personal (for learning)
- DM Policy: Pairing Mode
- allowFrom: Unset

---

## ⚠️ Warning

WhatsApp automation uses unofficial API and may risk account restrictions.

---

## 🧪 Step 3: Test

Send:
```
Hello, what can you help me with?
```

---

## 📊 Dashboard

```bash
openclaw dashboard
```

---

## 🔍 Troubleshooting

```bash
openclaw doctor
```

Logs:
```bash
tail -f ~/.openclaw/logs/gateway.log
```

---

## 🔁 Fix Crash Loop

```bash
openclaw config set gateway.mode local
openclaw gateway restart
```

---

## 🎯 Final Message

You are now running your AI Employee 🚀

---

# 👍 Thanks for Watching
Subscribe to CodeVerse Soban for more tutorials!
