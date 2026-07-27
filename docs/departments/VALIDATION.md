# VALIDATION MODE
Version: 0.1
Status: Draft
Last Updated: 2026-07-27

---

## Purpose
Engineering modunun ürettiği Working Solution'ın gerçekten hedeflenen
problemi çözüp çözmediğini, gerçek dünya koşullarında test etmek.

---

## Core Principle

Studio'nun amacı her projeyi yaşatmak değildir.
Amaç: doğru olanı büyütmek, yanlış olanı erken durdurmaktır.

Bu nedenle Validation modunun görevi sadece "doğrulamak" değil,
gerektiğinde net bir şekilde **durdurma kararı almaktır.**
Bir çözümü, işe yaramadığı belli olduğu halde sürdürmek başarısızlıktır —
erken ve net bir şekilde terk etmek ise doğru bir sonuçtur.

---

## Entry Questions

- Working Solution hangi varsayımı test ediyordu?
- Bunu doğrulamak için hangi kanıt yeterli olur? (kullanım, sonuç, geri bildirim)
- Test gerçek koşullarda mı yapılıyor, yoksa varsayımsal mı?

---

## Exit Criteria

- Çözümün işe yarayıp yaramadığı net bir şekilde belirlenmiş olmalı
- Sonuç kanıta dayalı olmalı, izlenime dayalı değil

---

## Decision Point: Devam mı, Geri Dönüş mü, Terk mi

Validation'ın sonunda üç olası karar vardır:

1. **Product'a geç** — çözüm işe yaradığı doğrulandı, değer üretmeye hazır.
2. **Research'e geri dön** — varsayım kısmen doğru ama eksik/yanlış anlaşılmış,
   yeniden araştırma gerekiyor.
3. **Terk et** — çözüm işe yaramadı, varsayım çürütüldü. Proje burada durur.
   Bu bir başarısızlık değil, doğru zamanda alınmış doğru bir karardır.

Bu üç seçenekten biri **mutlaka** seçilmelidir. Belirsiz bırakılıp
"bir süre daha devam edelim" denmemelidir — bu, Studio'nun verimlilik
ilkesini zayıflatır.

---

## Output

**Validation Result** — kısa, şunları içeren:
- Test edilen varsayım
- Kullanılan yöntem/kanıt
- Sonuç: doğrulandı / doğrulanmadı / kısmen doğrulandı
- Karar: Product'a geç / Research'e dön / Terk et

---
End of Document