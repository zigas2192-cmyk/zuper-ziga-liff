# Zuper ZIGA Bot — LIFF App

LINE LIFF App สำหรับบันทึกความสนใจสินค้า Zuper Ziga  
งานวันกุ้ง 2026 · สุราษฎร์ธานี · 19–21 พ.ค. 2026

## Setup

### 1. แก้ไข `index.html`

เปิดไฟล์และแก้ค่าต่อไปนี้:

```javascript
var LIFF_ID = '2010023092-EqIxfEch';           // ← LIFF ID (ถูกต้องแล้ว)
var N8N_URL = 'https://primary-production-4fbc.up.railway.app/webhook/ziga-liff-submit'; // ← ตรวจ path ให้ตรงกับ n8n
```

### 2. Push ขึ้น GitHub

```bash
git init
git add .
git commit -m "init: ZIGA LIFF app"
git branch -M main
git remote add origin https://github.com/[YOUR_USERNAME]/zuper-ziga-liff.git
git push -u origin main
```

### 3. เปิด GitHub Pages

GitHub repo → Settings → Pages → Source: **GitHub Actions**

URL จะเป็น: `https://[YOUR_USERNAME].github.io/zuper-ziga-liff/`

### 4. อัพเดต LINE LIFF Endpoint

LINE Developers Console → ZIGA LIFF (ID: `2010023092-EqIxfEch`)  
→ Endpoint URL → ใส่ URL จาก GitHub Pages  
→ Save

## Stack

- LINE LIFF SDK v2
- Vanilla HTML/CSS/JS (no build step)
- Deploy: GitHub Pages via GitHub Actions

## Project

`ZIGA-LINEBOT-2026-001` · ZIGA Innovation Pcl.
