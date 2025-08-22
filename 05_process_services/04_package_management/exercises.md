# تمرین‌های فصل ۵ – مدیریت سرویس‌ها

### تمرین ۱: وضعیت سرویس sshd را بررسی کن
```bash
systemctl status sshd
```

### تمرین ۲: سرویس sshd را فعال کن
```bash
sudo systemctl start sshd
sudo systemctl enable sshd
```

### تمرین ۳: سرویس sshd را ری‌استارت کن
```bash
sudo systemctl restart sshd
```

### تمرین ۴: همه سرویس‌های فعال را لیست کن
```bash
systemctl list-units --type=service
```

### تمرین ۵: لاگ‌های بوت فعلی را ببین
```bash
journalctl -b
```

### تمرین ۶: سطح اجرای سیستم را تغییر بده (بدون GUI)
```bash
sudo systemctl set-default multi-user.target
```
