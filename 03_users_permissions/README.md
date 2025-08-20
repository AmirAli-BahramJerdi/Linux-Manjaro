# فصل ۳ – کاربر و دسترسی‌ها

## 🎯 هدف
- مدیریت کاربرها و گروه‌ها
- تغییر رمز عبور
- درک سطوح دسترسی (Permissions)
- کار با sudo و root

---

## 📌 ۱. مدیریت کاربرها
```bash
whoami              # نمایش کاربر فعلی
id                  # UID و GID و گروه‌ها
sudo su             # ورود به کاربر root
adduser test        # ساخت کاربر جدید
passwd test         # تغییر رمز کاربر
deluser test        # حذف کاربر
```
> در مانجارو معمولا به جای `adduser` باید از `useradd` استفاده کنید.

---

## 📌 ۲. مدیریت گروه‌ها
```bash
groupadd hackers         # ساخت گروه
usermod -aG hackers test # اضافه کردن کاربر به گروه
groups test              # نمایش گروه‌های کاربر
deluser test hackers     # حذف کاربر از گروه
```

---

## 📌 ۳. دسترسی‌ها (Permissions)
هر فایل ۳ بخش دسترسی دارد:  
`rwxr-xr--`

- User (صاحب فایل) → `rwx`  
- Group (گروه فایل) → `r-x`  
- Others (بقیه) → `r--`  

📦 تغییر دسترسی‌ها:
```bash
chmod 755 file   # u=rwx g=rx o=rx
chmod 644 file   # u=rw g=r o=r
```

📦 تغییر مالکیت:
```bash
chown user:group file
```

---

## 📌 ۴. sudo و root
- کاربر root → همه کار می‌تواند بکند.  
- sudo → اجرای یک دستور با دسترسی root.  
- sudo !! → اجرای آخرین دستور با دسترسی root.

---

## 📝 نکته
- UID کاربر root همیشه 0 است.  
- اگر فایلی فقط برای root است، برای خواندنش باید از sudo استفاده کنید.  