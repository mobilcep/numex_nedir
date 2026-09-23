# 🗺️ Yol Haritası ve Sürüm Notları

## Zaman çizelgesi

| Dönem | Sürüm | Öne çıkanlar |
|---|---|---|
| 2021 | — | Fikir: *"Türkçe konuşan, Türk kültürünü anlayan bir yapay zeka neden yok?"* |
| 2023–2024 | v2.x | İlk prototip → üretim; ilk Pipeline prototipi (prompt güçlendirme), temel sohbet ve kullanıcı sistemi, Detective Mode konsepti |
| 2025 | **v3.0** | Sıfırdan yeniden yazım: Türkçe odaklı altyapı, Pipeline (Boru Sistemi), sohbet + kod + belge analizi, karakter sistemi, KVKK uyumlu işleme, planlar (Free/Basic/Pro/Advanced/Kurumsal), Dış API (`/v1/chat/completions`), admin paneli, çift sunucu, çoklu sağlayıcı, Serper web arama |
| Mart 2025 | DeepView v1.0 | Çoklu uzman orkestratörü, 6 katmanlı görselleştirme |
| Şubat 2026 | **v3.1** | İlk genel kullanıcı sürümü (aşağıda) |
| 2026 | Aile | Codex IDE v2.9.59, CLI v3.3.10, Okul, Market, Numexpedia, Hub & Forge, Oyun Bahçesi, Pusulam, PC Doktoru v3.1 |

## v3.1 — Şubat 2026

**✦ Yeni özellikler**
- Numex **Pro, Fast, Vision ve Code** profilleri — Pipeline ile güçlendirilmiş 4 model
- Web arama modu (chip seçiciler)
- Paylaşılabilir sohbet linkleri
- Uygulama içi bildirim sistemi
- Misafir kullanımı — kayıt olmadan günde 5 mesaj
- Google ve GitHub OAuth girişi
- Codex — gelişmiş kod editörü ve syntax highlighting
- Web cache — daha hızlı açılış

**↑ İyileştirmeler**
- Boru 2A — Türkçe çıktı kalitesi **%30** iyileşti
- Sohbet arayüzü yeniden tasarlandı
- Karakterler daha doğal yanıt veriyor
- API ortalama yanıt süresi **0,8 s → 0,5 s**
- Erişilebilirlik: yüksek kontrast, büyük yazı, ekran okuyucu

**⚑ Düzeltmeler**
- Uzun sohbetlerde bellek sızıntısı
- Mobilde klavye açılınca giriş alanının kayması
- Markdown kod bloklarının kırılması

## Numex Core seviyeleri

| Seviye | Durum |
|---|---|
| 1 — CLI | ✅ |
| 2 — Chat + Tools | ✅ |
| 3 — RAG + Context | ✅ |
| 4 — Otonom kodlama (scaffold, E2E deploy) | ✅ |
| 5 — Swarm Council | ✅ |
| 6 — Sentetik Mimar (meta-reasoning, 12 sektör, öz-eğitim) | ✅ geliştirme ortamında |
| 7–8 | Vizyon aşamasında |
