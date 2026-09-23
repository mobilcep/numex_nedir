# 🔒 Güvenlik, Gizlilik ve KVKK

## Veri nerede?
- Veriler **Türkiye sınırları içinde** işlenir ve saklanır; **KVKK** standartlarına uyumlu.
- **Çift sunucu mimarisi:** her biri 256 GB RAM; biri devre dışı kalırsa diğeri devralır. **SAS + NAS** depolama.
- Global altyapı sağlayıcıları (Google Cloud, Microsoft Azure, Anthropic, Vercel, Meta, MongoDB,
  DeepSeek) yalnızca altyapı sağlar; veri işleme ve saklama **Numex politikasına** tabidir.

![Teknoloji ortakları](../gorseller/teknoloji-ortaklar.png)

## Kimlik ve erişim
- **Google** ve **GitHub** OAuth — tek hesap, tüm ekosistem (Web, CLI, Codex, Hub, Forge).
- CLI için **cihaz kodu** ile tarayıcı onaylı giriş (`numex login`).
- API anahtarları `nx_live_` önekli; bir kez gösterilir; **rotate** ve silme desteklenir.
- Üretimde zayıf JWT anahtarları reddedilir.

## Ajan güvenliği
- **Onay kapısı:** Otonom/Agent modları plan sunar, onay olmadan başlamaz (*"anlaşalım, sonra yapalım"*).
- **Diff önizleme:** Her dosya değişikliği kabul/ret için gösterilir.
- **Geri alma:** `numex undo`, `.numex/checkpoints`, PC Doktoru'nda sistem geri yükleme noktası.
- **Denetim izi:** `.numex/audit/audit-trail.jsonl` — ajanın yaptığı her işlem.
- **FinishGate:** "Bitti" demek için kanıt şart.
- **Komut beyaz listesi** (PC Doktoru).

## Ödeme
İyzico altyapısı · 256-bit SSL · kart bilgisi Numex sunucularında saklanmaz · kredi/banka kartı ve QR.

## Şeffaflık
Detective Mode™ gerekçeli karar · DeepView™ 6 katmanlı düşünce görünümü · gerçek veri yoksa
"uydurma sayı göstermeyen" paneller.

## Erişilebilirlik
Yüksek kontrast, büyük yazı, ekran okuyucu desteği.

---
← [Ürünler](README.md)
