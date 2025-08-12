# Arch VM Installation Guide

This document contains the step-by-step process I followed during my 13-day Arch VM setup journey.  
Bu belge, 13 günlük Arch VM kurulum sürecimde izlediğim adımları içerir.

---

## 🧱 Setup Steps

1. ISO indirme ve doğrulama  
2. VirtualBox VM oluşturma  
3. Disk bölümlendirme (`cgdisk`, `mkfs`)  
4. Base sistem kurulumu (`pacstrap`, `genfstab`)  
5. Chroot ile yapılandırma  
6. Bootloader kurulumu (`grub`)  
7. Ağ ve kullanıcı ayarları  
8. X11 ve masaüstü ortamı kurulumu  
9. ClamAV testleri ve güvenlik yapılandırmaları  
10. Belgelerin arşivlenmesi ve GitHub’a aktarımı

---

## 🧩 Notes & Observations

- `pacstrap` bazen ağ hatası veriyor → çözüm: `reflector` ile hızlı mirror seçimi  
- `grub-install` hatası → UEFI/BIOS uyumsuzluğu kontrol edilmeli  
- Terminal çıktıları `common-errors.md` dosyasında arşivlenecek
