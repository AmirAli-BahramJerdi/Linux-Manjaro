# فصل ۴ – مدیریت پکیج‌ها در مانجارو (pacman و yay)

## 🎯 هدف
- یادگیری نصب، حذف و آپدیت نرم‌افزارها
- کار با مخازن (Repositories)
- استفاده از AUR (Arch User Repository)

---

## 📌 ۱. pacman – ابزار اصلی مدیریت پکیج
```bash
sudo pacman -Syu          # آپدیت کل سیستم
sudo pacman -S firefox    # نصب برنامه
sudo pacman -R firefox    # حذف برنامه
sudo pacman -Ss keyword   # جستجو در مخازن
sudo pacman -Qi firefox   # نمایش اطلاعات پکیج
sudo pacman -Qdt          # لیست پکیج‌های یتیم (orphan)
sudo pacman -Rns package  # حذف کامل پکیج به همراه کانفیگ
```

---

## 📌 ۲. کش (Cache) پکیج‌ها
```bash
sudo paccache -r        # پاک کردن کش پکیج‌های قدیمی
sudo pacman -Sc         # پاک کردن کش بدون نیاز
```

---

## 📌 ۳. مخازن (Repositories)
- فایل اصلی: `/etc/pacman.conf`
- لیست mirrorها: `/etc/pacman.d/mirrorlist`

تغییر mirror به نزدیک‌ترین سرور:
```bash
sudo pacman-mirrors --fasttrack
```

---

## 📌 ۴. AUR و yay
- AUR یک مخزن کاربری است که نرم‌افزارهای غیررسمی در آن هستند.
- برای نصب نیاز به yay داریم:

```bash
sudo pacman -S yay        # نصب yay (معمولاً از قبل نصب است)
yay -S google-chrome      # نصب نرم‌افزار از AUR
yay -R google-chrome      # حذف نرم‌افزار
yay -Ss keyword           # جستجو در AUR
```

---

## 📌 ۵. آپدیت کامل سیستم
```bash
sudo pacman -Syu       # آپدیت رسمی
yay -Syu               # آپدیت به همراه AUR
```

---

## 📝 نکته
- همیشه قبل از نصب نرم‌افزار جدید، بهتر است `sudo pacman -Syu` را اجرا کنید.
- از `yay` فقط برای پکیج‌های AUR استفاده کنید، برای پکیج‌های رسمی `pacman` سریع‌تر و مطمئن‌تر است.