# WS-001: Weekly Signal Brief — Prompt Template

Status: Draft
Date: 2026-07-27
Mode: Engineering
Related: RR-001-weekly-signal-brief-method.md

---

## Ne İnşa Edildi

Kod değil — tekrar kullanılabilir bir **prompt şablonu**.
Haftada bir, bu şablon bir LLM'e verilerek yapılandırılmış bir
Strategic Brief adayı üretilir.

---

## Prompt Şablonu

```
Konu: [BURAYA KONU YAZILIR — örn. "AI araçları"]
Zaman aralığı: Son 7 gün

Görev:
Bu konudaki son 7 gündeki önemli gelişmeleri araştır ve şu formatta özetle:

1. En fazla 5 gelişme, her biri 1-2 cümle
2. Her gelişme için: neden önemli olabilir?
3. Sonunda: "Araştırmaya değer mi?" sorusuna evet/hayır + kısa gerekçe

Kural: İlginç olduğu için değil, Studio için gerçekten araştırmaya 
değer olduğu için seçilecek (bkz. STRATEGY_MODE.md prensipleri).
```

---

## Hangi Varsayım Test Ediliyor

"Sabit bir prompt şablonu, kod/otomasyon olmadan, haftalık olarak 
kullanılabilir kalitede sinyal adayı üretebilir mi?"

---

## Alınan Temel Teknik Kararlar

- Otomasyon yok — manuel tetikleme (haftada 1 kez, kullanıcı başlatır)
- LLM bağımsız — herhangi bir LLM ile kullanılabilir (Claude, ChatGPT, vb.)
- Kod bağımlılığı yok — limit/kaynak kısıtı olan durumlarda bile kullanılabilir

---

## Bilinen Sınırlamalar

- Otomatik değil, hatırlanıp elle çalıştırılması gerekir
- LLM'in kendi bilgi/arama kalitesine bağımlı
- Henüz gerçek kullanımla test edilmedi

---

## Sonraki Adım

Validation Mode: Bu şablon 1-2 hafta gerçekten kullanılıp, ürettiği 
sonucun Strategy Mode için işe yarayıp yaramadığına karar verilecek.

---
End of Document