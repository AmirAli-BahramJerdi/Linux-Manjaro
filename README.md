# 🐧 دوره آموزشی لینوکس مانجارو (به سبک LPIC ولی ساده)

این دوره برای یادگیری **لینوکس مانجارو (GNOME)** طراحی شده و شامل همه دستورات و ترفندهای ضروری است.
هدف: یادگیری ساده، کاربردی، و آماده شدن برای مباحث امنیت و هک.

---

## 📚 سرفصل‌ها
### 🔹 بخش ۱ – مقدمات  
1. معرفی لینوکس و تفاوت با ویندوز  
2. ساختار فایل‌سیستم لینوکس (FHS)  
3. آشنایی با مانجارو و محیط GNOME  

### 🔹 بخش ۲ – دستورات پایه ترمینال  
1. حرکت بین پوشه‌ها (pwd, cd, ls)  
2. مدیریت فایل‌ها (touch, cat, nano, less, head, tail)  
3. جابجا/کپی/حذف (mv, cp, rm)  
4. جستجو در فایل‌ها (grep, find, locate)  

### 🔹 بخش ۳ – کاربر و دسترسی‌ها  
1. یوزر و گروه‌ها (adduser, passwd, id)  
2. دسترسی‌ها و chmod/chown  
3. sudo و root  

### 🔹 بخش ۴ – مدیریت نرم‌افزار  
1. pacman (نصب، حذف، آپدیت)  
2. yay (AUR)  
3. جستجو و اطلاعات پکیج‌ها  

### 🔹 بخش ۵ – پروسس و سرویس‌ها  
1. مدیریت پروسس‌ها (ps, top, htop, kill)  
2. مدیریت سرویس‌ها (systemctl)  
3. Startup و Runlevels  

### 🔹 بخش ۶ – شبکه و امنیت پایه  
1. نمایش و تست شبکه (ip, ping, curl)  
2. پورت‌ها و پروسس‌ها (netstat, ss)  
3. فایل‌های شبکه (hosts, resolv.conf)  

### 🔹 بخش ۷ – ترفندها و نکات حرفه‌ای  
1. تاریخچه و !! , !n , Ctrl+R  
2. Alias و Bashrc  
3. اجرای پس‌زمینه/پیش‌زمینه (&, jobs, fg, bg)  
4. Pipe و Redirect (|, >, >>, <)  

### 🔹 بخش ۸ – ابزارهای امنیتی و هک پایه  
1. نصب ابزارها (nmap, wireshark, tcpdump)  
2. ساخت یوزر جدا برای pentest  
3. شروع با tmux  

---

## 📂 ساختار پروژه
```bash
linux-manjaro-course/
├── README.md               # توضیحات اصلی (سرفصل‌ها + لینک‌ها)
├── 01_intro/
│   ├── notes.md             # یادداشت‌های فصل ۱
│   └── exercises.md         # تمرین‌ها
├── 02_commands/
│   ├── notes.md
│   └── exercises.md
├── 03_users_permissions/
│   ├── notes.md
│   └── exercises.md
├── 04_package_management/
│   ├── notes.md
│   └── exercises.md
├── 05_process_services/
│   ├── notes.md
│   └── exercises.md
├── 06_networking/
│   ├── notes.md
│   └── exercises.md
├── 07_tips_tricks/
│   ├── notes.md
│   └── exercises.md
└── 08_security_tools/
    ├── notes.md
    └── exercises.md
```

---

## 🚀 شروع
1. این ریپازیتوری را کلون کنید یا دانلود کنید.  
2. فصل‌ها را به ترتیب مطالعه کنید.  
3. تمرین‌ها را در ترمینال انجام دهید.  
4. برای مرور سریع همیشه به README برگردید.  
