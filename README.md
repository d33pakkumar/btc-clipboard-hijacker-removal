# 🧹 Clipboard Hijacker Removal Guide

This is a simple, manual method to remove clipboard hijacker malware that replaces copied Bitcoin addresses with a malicious address.

---

## 🛑 Symptom

When copying a crypto wallet address (e.g. Bitcoin), it gets instantly replaced with:

1DL4pRCKKmg238fsCU6i7ZYEStP9fL9o4q


This is a known malicious Bitcoin address used in clipboard hijacker attacks.

---

## ✅ How to Manually Remove the Malware

### 1. Delete Suspicious Registry Entry

- Press `Windows + R`, type `regedit`, and press Enter
- Navigate to:

HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Run

- Look for a key like:
EPLTargetP0000... pointing to E_YATIN0E.EXE

- Delete the entry

---

### 2. Boot into Safe Mode

- Press `Windows + R`, type `msconfig`, press Enter
- Go to **Boot** tab → Check ✅ **Safe boot → Minimal**
- Click Apply → Restart

---

### 3. Delete the Malware File

In Safe Mode, go to:

C:\Windows\System32\spool\DRIVERS\x64\3\


- Find and delete:

E_YATIN0E.EXE


---

### 4. Reboot Normally

- Open `msconfig` again
- Uncheck ✅ **Safe boot**
- Restart your PC

---

### 5. Test Your Clipboard

Copy this test Bitcoin address:

1BoatSLRHtKNngkdXEeobR76b53LETtpyT (not mine just random)

Paste it in your browser or a form — if it doesn't change, you're clean 🎉

---

## 🧠 Why This Works

This hijacker installs itself as a fake printer driver in the `spool\DRIVERS` folder and autostarts using a registry key.

By removing the registry key and deleting the file from Safe Mode, you cut off its ability to run or infect again.

---

## 💬 Contribute

If you find other clipboard hijacker variants or BTC addresses, feel free to open a pull request or issue.

---

## ✅ Confirmed Malicious BTC Address

- `1DL4pRCKKmg238fsCU6i7ZYEStP9fL9o4q`

---

## 🛡 Stay Safe

Never send crypto without triple-checking the address. Use QR codes or hardware wallets whenever possible.

---

## 💖 Support This Project

If this guide helped you recover or save your funds or remove the malware successfully, and you'd like to support my work:

### 🟧 BTC Donation Address:

bc1qz67nnrhvxjrd5hey27pefzcdmdhpkk4qep7kf0

Any amount is appreciated 🙏 — it motivates me to create more helpful guides like this one.


