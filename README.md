# GitHub Actions Feature Sample

This project demonstrates how to use **GitHub Actions** to run Python scripts for free, serverless automation tasks—such as weather notifications, reward collection, and daily sign-ins.


## Part 1: Draw Heart Executables

👉 **Fork** this repository first.

### 🖥️ Build on Windows
1. Go to **Actions** → **Draw Heart for Windows**
2. Click **Run Workflow**
3. After completion, go to **Artifacts** and download `love_heart`

### 🐧 Build on Ubuntu
1. Go to **Actions** → **Draw Heart for Ubuntu**
2. Click **Run Workflow**
3. After completion, go to **Artifacts** and download `love_heart`

### 🍎 Build on macOS
1. Go to **Actions** → **Draw Heart for macOS**
2. Click **Run Workflow**
3. After completion, go to **Artifacts** and download `love_heart`

---

## Part 2: Weather Notification via WeChat

### ✳️ Apply for a WeChat Test Account

Scan with WeChat to log in:  
👉 https://mp.weixin.qq.com/debug/cgi-bin/sandbox?t=sandbox/login

After logging in, collect the following four values:
- `appID`
- `appSecret`
- `openId` (recipient user ID)
- `template_id`

> 📌 Anyone who should receive messages must scan the QR code so they appear in the user list and expose their `openId`.

To create a template, use the following format:

```text
Today: {{date.DATA}}  
Location: {{region.DATA}}  
Weather: {{weather.DATA}}  
Temperature: {{temp.DATA}}  
Wind: {{wind_dir.DATA}}  
Message: {{today_note.DATA}}

