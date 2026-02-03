![Conduit Pro](./assets/preview.png)

# Conduit Pro for Android

Conduit Pro is an Android application that allows you to quickly deploy and manage a **Conduit server** on your own VPS with just a few taps — no Linux or SSH experience required.

---

## 🦁🌞👑 راهنمای نصب و راه‌اندازی Conduit Pro (فارسی)

### Conduit Pro چیست؟
**Conduit Pro** یک اپلیکیشن اندرویدی است که به شما اجازه می‌دهد تنها در چند دقیقه یک سرور **Conduit** را روی VPS خودتان راه‌اندازی و مدیریت کنید.

این سرور پس از راه‌اندازی، توسط کاربران از طریق اپلیکیشن **Psiphon** قابل استفاده خواهد بود.

---

## بخش اول: خرید و ساخت سرور (VPS)

برای استفاده از Conduit Pro، به یک سرور لینوکسی نیاز دارید.  
در این راهنما دو سرویس پیشنهادی معرفی شده‌اند.

---

### گزینه ۱: DigitalOcean (یکی از این دو گزینه را انتخاب کنید)

🌐 وب‌سایت:  
https://www.digitalocean.com/

#### مراحل ساخت سرور:
1. وارد سایت DigitalOcean شوید و یک حساب کاربری بسازید.
2. از منوی بالا روی **Create → Droplets** کلیک کنید.
3. تنظیمات زیر را انتخاب کنید:
   - **Image:** Ubuntu 22.04 (LTS)
   - **Plan:**  
     - Basic  
     - Shared CPU  
     - پلن **۴ یا ۶ دلار در ماه**
   - **Region:**  
     - فرقی ندارد (مثلاً یکی از ریجن‌های آمریکا)
   - **Authentication:**  
     - حتماً **Password** را انتخاب کنید (نه SSH Key)
4. یک پسورد برای سرور تعیین کنید.
5. روی **Create Droplet** کلیک کنید.

بعد از چند ثانیه:
- یک **IP Address** دریافت می‌کنید
- این IP و پسورد را نگه دارید (در اپلیکیشن استفاده می‌شود)

---

### گزینه ۲: Hetzner Cloud (جایگزین)

🌐 وب‌سایت:  
https://www.hetzner.com/cloud

#### به‌صورت خلاصه:
1. در سایت Hetzner اکانت بسازید.
2. یک Cloud Server جدید ایجاد کنید.
3. سیستم‌عامل: **Ubuntu 22.04**
4. یک پلن ارزان انتخاب کنید (مثل CX11)
5. احراز هویت با **Password**
6. IP و پسورد سرور را ذخیره کنید.

---

## بخش دوم: دانلود و نصب اپلیکیشن

📦 لینک دانلود رسمی:
https://github.com/mehrdadsml/conduitpro/releases

### مراحل نصب:
1. وارد لینک بالا شوید.
2. آخرین نسخه فایل **APK** را دانلود کنید.
3. فایل را روی گوشی اندروید نصب کنید.

⚠️ **نکته مهم:**  
از آن‌جایی که اپلیکیشن از Google Play نصب نمی‌شود:
- ممکن است هشدار امنیتی نمایش داده شود
- گزینه‌هایی مثل **Install anyway** یا **Allow from this source** را تأیید کنید

این موضوع طبیعی است.

---

## بخش سوم: اتصال به سرور و نصب Conduit

1. اپلیکیشن **Conduit Pro** را باز کنید.
2. مقادیر پیش‌فرض از قبل تنظیم شده‌اند:
   - **Port:** 22
   - **Username:** root
3. فقط این موارد را وارد کنید:
   - **IP Address** سرور
   - **Password** سرور
4. روی **Connect & Monitor** بزنید.

---

### نصب خودکار Conduit
- اگر Conduit روی سرور نصب نباشد، اپلیکیشن به‌صورت خودکار تشخیص می‌دهد.
- یک صفحه نصب نمایش داده می‌شود.
- از شما فقط این موارد پرسیده می‌شود:
  - حداکثر تعداد کاربران متصل
  - محدود یا نامحدود بودن پهنای باند
- نیازی به تغییر تنظیمات نیست، فقط تأیید کنید.

⏳ زمان نصب:
- حدود **۱ تا ۲ دقیقه**

---

### بعد از نصب
- سرور شما آماده است
- ممکن است تا **۲۴ ساعت** طول بکشد تا کاربران بتوانند از طریق Psiphon به سرور متصل شوند
- پس از آن، سرور به‌صورت پایدار قابل استفاده خواهد بود

---

## 🇬🇧 Conduit Pro – Installation & Setup Guide (English)

### What is Conduit Pro?
**Conduit Pro** is an Android app that lets you deploy and manage a **Conduit server** on your own VPS in just a few minutes — no Linux or SSH knowledge required.

Users can connect to the deployed server using **Psiphon**.

---

## Part 1: Buying a VPS Server

You need a Linux VPS to use Conduit Pro.  
Two recommended providers are listed below.

---

### Option 1: DigitalOcean (Choose one of these two options.)

🌐 Website:  
https://www.digitalocean.com/

#### Steps:
1. Create an account on DigitalOcean.
2. Go to **Create → Droplets**.
3. Select the following:
   - **Image:** Ubuntu 22.04 (LTS)
   - **Plan:**  
     - Basic  
     - Shared CPU  
     - **$4 or $6/month**
   - **Region:**  
     - Any (e.g. United States)
   - **Authentication:**  
     - **Password (required)**
4. Set a root password.
5. Click **Create Droplet**.

After creation:
- You’ll receive a **server IP**
- Save the IP and password for the app

---

### Option 2: Hetzner Cloud (Alternative)

🌐 Website:  
https://www.hetzner.com/cloud

Quick overview:
1. Create an account.
2. Create a new cloud server.
3. OS: **Ubuntu 22.04**
4. Choose a low-cost plan (CX11 or similar).
5. Use **password authentication**.
6. Save the server IP and password.

---

## Part 2: Downloading the App

📦 Official download link:
https://github.com/mehrdadsml/conduitpro/releases

### Installation:
1. Download the latest **APK**.
2. Install it on your Android device.

⚠️ **Note:**  
Because the app is not from Google Play:
- Android may show a security warning
- Choose **Install anyway** or **Allow from this source**

This is expected behavior.

---

## Part 3: Connecting & Installing Conduit

1. Open **Conduit Pro**.
2. Default values are already set:
   - **Port:** 22
   - **Username:** root
3. Enter only:
   - **Server IP**
   - **Server Password**
4. Tap **Connect & Monitor**.

---

### Automatic Installation
- If Conduit is not installed, the app detects it automatically.
- An installation sheet appears.
- You’ll be asked to confirm:
  - Max connected users
  - Limited or unlimited bandwidth
- No changes needed — just confirm.

⏳ Installation time:
- About **1–2 minutes**

---

### After Installation
- Your server is ready
- It may take up to **24 hours** before users can connect via Psiphon
- After that, the server works normally
