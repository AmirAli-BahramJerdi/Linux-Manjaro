# فصل ۵ – مدیریت سرویس‌ها با systemd

## 🎯 هدف
- یادگیری مدیریت سرویس‌ها (start, stop, enable, disable)
- آشنایی با journalctl برای مشاهده لاگ‌ها
- مدیریت سطح اجرای سیستم (runlevels / targets)

---

## 📌 ۱. سرویس‌ها در لینوکس (systemd)
systemd مدیریت سرویس‌ها و پروسه‌های سیستمی را برعهده دارد.

```bash
systemctl status service      # وضعیت سرویس
systemctl start service       # شروع سرویس
systemctl stop service        # توقف سرویس
systemctl restart service     # ری‌استارت سرویس
systemctl enable service      # فعال‌سازی هنگام بوت
systemctl disable service     # غیرفعال‌سازی
```

مثال:
```bash
sudo systemctl status sshd
sudo systemctl start sshd
sudo systemctl enable sshd
```

---

## 📌 ۲. مشاهده همه سرویس‌ها
```bash
systemctl list-units --type=service
systemctl list-unit-files --type=service
```

---

## 📌 ۳. لاگ‌های سیستم (journalctl)
```bash
journalctl -u sshd.service       # لاگ‌های مربوط به سرویس sshd
journalctl -xe                   # نمایش خطاهای اخیر
journalctl -b                    # لاگ‌های بوت فعلی
```

---

## 📌 ۴. سطوح اجرا (Targets)
- جایگزین runlevels در systemd

```bash
systemctl get-default            # نمایش سطح اجرای فعلی
systemctl set-default multi-user.target   # تغییر سطح اجرا به حالت بدون GUI
systemctl set-default graphical.target    # تغییر سطح اجرا به حالت گرافیکی
```

---

## 📌 ۵. ریبوت و شات‌داون با systemd
```bash
systemctl reboot
systemctl poweroff
```

---

## 📝 نکته
- همیشه قبل از فعال کردن سرویس جدید، وضعیت آن را با `systemctl status` بررسی کنید.
- برای دیباگ بهتر است از `journalctl -xe` استفاده کنید.