# تمرین‌های فصل ۲ – دستورات ترمینال

### تمرین ۱: یک پوشه بساز و داخلش برو
```bash
mkdir test_dir
cd test_dir
pwd
```

### تمرین ۲: فایل بساز و محتوا اضافه کن
```bash
echo "Hello Linux" > hello.txt
cat hello.txt
```

### تمرین ۳: ۵ خط اول فایل passwd را نمایش بده
```bash
head -n 5 /etc/passwd
```

### تمرین ۴: فایل را کپی کن و نامش را تغییر بده
```bash
cp hello.txt copy.txt
mv copy.txt renamed.txt
```

### تمرین ۵: جستجو در فایل
```bash
grep "root" /etc/passwd
```

### تمرین ۶: نمایش درختی پوشه home
```bash
tree ~
```
