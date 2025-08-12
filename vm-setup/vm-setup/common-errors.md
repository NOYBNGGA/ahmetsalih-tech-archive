# Common VM Setup Errors | Yaygın VM Kurulum Hataları

This document lists common issues encountered during VM setups and their solutions.  
Bu belge, VM kurulumları sırasında karşılaşılan yaygın sorunları ve çözümlerini listeler.

---

## ❌ Error: pacstrap failed to fetch packages  
## ❌ Hata: pacstrap paketleri indiremedi

**Cause | Sebep:** Network mirror is slow or misconfigured  
**Fix | Çözüm:** Use `reflector` to update mirror list  
`reflector` komutu ile hızlı ve güncel mirror listesi oluşturulabilir.

---

## ❌ Error: grub-install failed  
## ❌ Hata: grub-install başarısız

**Cause | Sebep:** UEFI/BIOS mismatch or missing EFI partition  
**Fix | Çözüm:** Ensure correct partitioning and boot mode  
UEFI/BIOS uyumu ve EFI bölümü kontrol edilmeli.

---

## ❌ Error: X11 not starting  
## ❌ Hata: X11 başlatılamıyor

**Cause | Sebep:** Missing display manager or misconfigured `.xinitrc`  
**Fix | Çözüm:** Install `lightdm` or configure `.xinitrc` properly  
`lightdm` kurulmalı veya `.xinitrc` dosyası doğru yapılandırılmalı.
