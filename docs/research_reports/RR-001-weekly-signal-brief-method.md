# RR-001: Weekly Signal Brief — Method Research

Status: Complete
Date: 2026-07-27
Mode: Research
Related: SB-001-weekly-signal-brief.md

---

## Araştırılan Soru

Belirli bir konuda haftalık özet üretmek için hangi yöntem (manuel prompt,
otomatik script, mevcut araç) en az efor ile en güvenilir sonucu verir?

---

## Bulgular

Üç yöntem kategorisi tespit edildi:

**1. Hazır ticari araçlar** (Readless, Mailbrew, Meco vb.)
Kaynak toplama, tekrar eleme, reklam temizleme gibi özellikler sunuyor.
Ancak genel newsletter özetlemeye göre tasarlanmış; Studio'nun Strategy
Mode'una özel bir brief formatı üretmiyor.

**2. DIY otomasyon** (n8n, Zapier + LLM, custom script)
2025'te birden fazla kullanıcı topluluğu tartışmasında, bu tür DIY
otomasyonların birkaç hafta içinde terk edildiği belgelenmiş — sebep,
bakım yükünün kazanılan zamandan fazla olması.

**3. Manuel ama yapılandırılmış LLM sorgusu**
Otomasyon yok, ama esneklik ve kontrol yüksek, bakım yükü neredeyse sıfır.
Düzenli aralıklarla (haftalık), sabit bir prompt şablonu ile bir LLM'e
soru sorup yapılandırılmış bir çıktı almak.

---

## Değerlendirme (Evidence First prensibiyle)

- Otomatik/scriptli çözüm: **Risk yüksek** — kanıtlar, bakım yükünün
  zamanla değeri aştığını gösteriyor. Ayrıca şu an kod yazma kapasitesi
  kısıtlı (limit sorunu).
- Manuel + yapılandırılmış prompt: **Risk düşük** — kod gerektirmiyor,
  hemen test edilebilir, bakım yükü yok.

---

## Sonuç

**Kısmen doğrulandı.** Otomatik bir "sinyal takip ajanı" şu an için
doğru çözüm değil. Bunun yerine, en küçük çalışan versiyon (Core First)
şudur:

> Haftada bir, sabit bir prompt şablonuyla, belirli bir konuda
> yapılandırılmış bir özet istemek — kod yazmadan, sadece tekrar
> kullanılabilir bir şablon olarak.

---

## Öneri: Engineering Mode'a Geçiş

Engineering aşaması burada "kod yazmak" değil, **"tekrar kullanılabilir
bir prompt şablonu tasarlamak"** olarak tanımlanmalıdır. Bu, hem mevcut
kısıtla (kod yazmama) uyumludur hem de Core First prensibine sadıktır.

---
End of Document