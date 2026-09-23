<div align="center">

# ◆ Numex AI

### Türkiye'nin yerli yapay zeka ekosistemi

**Sohbet · Kod · Ajanlar · Belge analizi · Web araması — Türkçe'ye ve Türk kullanıcısına özel.**

[![Web](https://img.shields.io/badge/web-numexai.com.tr-1de9b6)](https://numexai.com.tr)
[![Kuruluş](https://img.shields.io/badge/kuruluş-2021%20·%20İstanbul-0b1f3a)](#-hikaye)
[![KVKK](https://img.shields.io/badge/KVKK-uyumlu-22c55e)](#-gizlilik-ve-altyapı)
[![Lisans](https://img.shields.io/badge/lisans-MIT-blue)](LICENSE)

[**🚀 Ücretsiz başla**](https://numexai.com.tr) ·
[**💳 Planlar**](#-planlar) ·
[**⌨️ CLI**](#️-numex-cli) ·
[**📚 Makaleler**](makaleler/)

</div>

---

> *"Türkçe konuşan, Türk kültürünü anlayan bir yapay zeka neden yok?"*
> Numex AI bu soruyla 2021'de yola çıktı.

## İçindekiler

- [Numex AI nedir?](#-numex-ai-nedir)
- [Neden farklı?](#-neden-farklı)
- [Ürün ailesi](#-ürün-ailesi)
- [Teknoloji](#-teknoloji)
- [Numex profilleri](#-numex-profilleri)
- [Türkçe karakter sistemi](#-türkçe-karakter-sistemi)
- [Planlar](#-planlar)
- [Gizlilik ve altyapı](#-gizlilik-ve-altyapı)
- [Hikaye](#-hikaye)
- [Makaleler](#-makaleler)
- [İletişim](#-iletişim)

---

## ◆ Numex AI nedir?

**Numex AI**, 2021'den beri İstanbul'da geliştirilen, **Türkçe'ye ve Türk kullanıcısına özel tasarlanmış**
bir yapay zeka platformudur. Amaç basit: yapay zekayı **anlaşılır, erişilebilir ve faydalı** kılmak.

| | |
|---|---|
| **2021** | Kuruluş yılı · İstanbul |
| **9+** | Yapay zeka modülü, tek platformda |
| **2 × 256 GB** | RAM — çift sunucu altyapısı |
| **%100** | KVKK uyumlu · Türkiye altyapısı |

Aynı motor web'de, terminalde ve editörde çalışır: **nerede çalışıyorsanız Numex oradan devam eder.**

## ✨ Neden farklı?

**Ham API değil, Türkçe'ye özel işlenmiş bir sistem.** Numex her isteği doğrudan bir modele iletmek
yerine kendi motorlarından geçirir:

| | Özellik | Ne yapar? |
|---|---|---|
| ⚡ | **Pipeline Motoru** | Her istek 5 katmandan geçer: prompt güçlendirme → AI işleme → Türkçe düzeltme → format ayarı → kalite kontrol. |
| 🕵️ | **Detective Mode™** | Kritik sorularda birden fazla model aynı soruyu bağımsız çözer; bir **hakem sistemi** en doğru yanıtı seçer. |
| 🤖 | **Multi-Agent** | Orkestratör karmaşık isteği alt görevlere böler, uzman ajanlara dağıtır, sonucu tek tutarlı yanıtta birleştirir. |
| 🇹🇷 | **Türkçe DNA** | *"Yapılmaktadır"* değil, *"yapılır"* diyen bir yapay zeka. Doğal, günlük Türkçe. |
| 🔍 | **Numex DeepView™** | Yapay zekanın ne söylediğini değil, **nasıl düşündüğünü** 6 katmanda görselleştiren şeffaf mimari. |

## 🧩 Ürün ailesi

| Ürün | Açıklama |
|---|---|
| 🌐 **Numex AI — Web & PWA** | Kayıt olmadan tarayıcıdan deneyin; giriş yaptıktan sonra mobil/masaüstüne uygulama olarak ekleyin. Sohbet, kod, görsel, ses, belge analizi ve web araması. |
| ⌨️ **Numex CLI** | Terminalden çalışan otonom kodlama asistanı. **Uzaktan PC** köprüsü ile web'den ya da telefondan kendi bilgisayarınıza komut gönderin. |
| 🧩 **Numex Codex IDE** | VS Code altyapılı, yapay zeka entegreli masaüstü editör: sohbet, ajanlar, satır içi düzenleme ve terminal bir arada. |
| 🤖 **Numex Agent** | Çok adımlı görevlerde planlayan ve dosyalarınıza doğrudan değişiklik uygulayan ajan. Her değişiklik **diff** olarak gösterilir, siz kabul/ret edersiniz. |
| 🩺 **[PC Doktoru Süper Ajan](https://pcdoktoru.com.tr)** | Windows için yapay zeka destekli, portable bakım, teşhis ve tamir asistanı. ([Kaynak](https://github.com/mobilcep/pcdoktoru)) |
| 🧭 **PusulamX** | İşletmeler için Numex gücü: KOBİ'lerin ön muhasebe ve POS süreçlerinde "X" çarpanıyla büyümesi. *(2026)* |
| 🎓 **Numex Okul** | Yapay zeka destekli eğitim ve içerik üretimi. |

### ⌨️ Numex CLI

```powershell
# Windows (PowerShell) — Node.js 18+ gerekir
irm https://www.numexai.com.tr/install-cli.ps1 | iex
numex basla          # tarayıcıda giriş + menü
numex uzak install   # arka plan köprüsü (sistem tepsisinde Numex ikonu)
```

- 💬 **Terminal sohbeti:** Proje klasöründe ajan tabanlı asistan — dosya okuma/yazma, git, RAG arama.
- 🖥️ **Uzaktan PC:** Telefondan veya başka bir cihazdan kendi PC'nize klasör, dosya ve shell komutu gönderin.
- 🔑 Numex hesabınızın token bakiyesini veya API anahtarını kullanır.

## ⚙️ Teknoloji

```
 👤 Kullanıcı ──▶ ⚡ Boru 1 ──▶ 🤖 AI Motor ──▶ ✨ Boru 2A ──▶ 🧠 Boru 2B ──▶ ✅ Son yanıt
                 prompt       iş ortağı        Türkçe düzeltme   kalite kontrol
                 güçlendirme  modeli           format · ton      doğrulama
```

**Detective Mode™ — "Tek model yanılabilir. Üçü birden yanılmaz."**

```
                     Kullanıcı sorusu
          ┌──────────────┼──────────────┐
     ⚡ Hızlı analiz  🧠 Derin analiz  🎯 Alternatif bakış
          └──────────────┼──────────────┘
                ⚖️ Numex Hakem Sistemi
                         ▼
               🏆 Kazanan çözüm + gerekçe
```

**Altyapı sağlayıcıları:** Google Cloud, Microsoft Azure, Anthropic, Vercel, Meta, MongoDB, DeepSeek.
Veri işleme ve saklama Numex politikasına tabidir.

**Geliştirici katmanı:** Node.js · Express · MongoDB · Vercel (fra1) · JWT/OAuth (Google, GitHub) · İyzico.
`@numex-ai/core` çekirdeği CLI, VS Code eklentisi ve SDK tarafından ortak kullanılır (*"Süper SDK"* mimarisi).

→ Ayrıntılar: [Pipeline, Detective Mode ve Multi-Agent](makaleler/02-pipeline-detective-multi-agent.md)

## 🧠 Numex profilleri

| Profil | Kullanım | Öne çıkan |
|---|---|---|
| 🧠 **Numex Pro** | Genel amaçlı birincil profil | 128K bağlam, derin analiz |
| ⚡ **Numex Fast** | Anlık sohbet, hızlı kod tamamlama | Düşük gecikme |
| 👁️ **Numex Vision** | Görsel analiz ve açıklama | Görsel anlama |
| 💻 **Numex Code** | Debug, refactor, test, dokümantasyon | Kod odaklı |

**Araçlar:** 🌐 Web arama · ⚙️ Kod çalıştırma (beta) · 📄 Belge analizi (PDF/Word) · 🤖 Agent modu

## 🇹🇷 Türkçe karakter sistemi

Türk kültürüne özel eğitilmiş **9 uzman karakter** — `@` ile çağrılır:

`@FatmaAna` · `@Üstat` · `@LokmanHekim` · `@HaciBayramHoca` · `@Kod` · …

> *"FatmaAna karakteri müthiş! Annem bile kullanıyor artık. Yemek tariflerinden ev ekonomisine kadar her şeyi soruyor."* — Bireysel kullanıcı

## 💳 Planlar

KDV dahil, şeffaf fiyatlandırma. Yıllık ödemede **2 ay bedava**.

| Plan | Fiyat | Mesaj | Bağlam | Öne çıkanlar |
|---|---|---|---|---|
| 🆓 **Ücretsiz** | ₺0 | 15/gün | 8K | Numex Hızlı model, günde 3 web araması, temel CLI |
| ⚡ **Başlangıç PRO** | ₺99/ay | 50/gün | 32K | Gelişmiş model, belge analizi, 3 karakter, tam CLI |
| 🚀 **Numex PRO** ⭐ | ₺399/ay | Limitsiz | 128K | Öncelikli kuyruk, CLI + API, tüm karakterler, beta erişimi |
| 💎 **Advanced** | ₺599/ay | Limitsiz | 128K | En yüksek öncelik, özel karakter, 3 alt hesap, WhatsApp destek |

**Numex Kredisi** (12 ay geçerli): Mini ₺25 · Standart ₺75 · Büyük ₺175 · Mega ₺450
**Zaman bazlı bilet** (otomatik yenilenmez): Gece 8 sa ₺29 · Günlük ₺49 · Sprint 72 sa ₺99 · Haftalık ₺169

Ödemeler İyzico altyapısıyla; kart bilgileri Numex sunucularında saklanmaz.
*Güncel fiyatlar için [numexai.com.tr](https://numexai.com.tr) esastır.*

## 🔒 Gizlilik ve altyapı

- 🇹🇷 **Veriler Türkiye'de:** İşleme ve saklama Türkiye sınırları içinde, **KVKK** standartlarına uygun.
- 🖥️ **Çift sunucu mimarisi:** Her biri 256 GB RAM'li iki sunucu; biri devre dışı kalırsa diğeri devralır.
- 🔍 **Şeffaflık:** Detective Mode ve DeepView ile karar süreci izlenebilir.
- ✅ **Kontrol sizde:** Agent modu değişiklikleri diff olarak sunar; onayınız olmadan uygulanmaz.

## 🏔️ Hikaye

| Yıl | Kilometre taşı |
|---|---|
| **2021** | *Bir soru ile başlangıç.* İlk satırlar Panorama İstanbul fotoğraf stüdyosunun arka odasında yazıldı. |
| **2023** | **Pipeline Motoru** — her yanıtı Türkçe'ye özel katmanlardan geçiren çok aşamalı işleme. |
| **2024** | **Detective Mode™** — çoklu model tartışma ve hakem sistemi. |
| **2025** | **Tam ekosistem** — sohbet, kod, belge analizi, sesli konuşma ve 9 Türkçe karakter. |
| **2026** | **PusulamX** ve **PC Doktoru Süper Ajan** — işletmeler ve Windows kullanıcıları için Numex gücü. |

**Kurucu:** Nurullah Şahin — Kurucu & AI Mimarı. Sivas Gürün kökenli, İstanbul'da yaşayan teknoloji girişimcisi.

> *"Yapay zeka insanı desteklemeli, yerini almamalı. Anadolu'nun bilgeliğiyle İstanbul'un dinamizmini
> harmanlayarak, herkes için anlaşılır ve faydalı bir yapay zeka inşa ediyoruz."*

**Değerlerimiz:** 🌱 Erişilebilirlik · 🔍 Şeffaflık · 🤝 İnsan merkezli · 🏔️ Kültürel bağlam · 🔒 Gizlilik · 🌿 Sürdürülebilirlik

## 📚 Makaleler

| # | Makale |
|---|---|
| 1 | [Numex AI: Türkçe düşünen yapay zeka](makaleler/01-numex-ai-tanitim.md) |
| 2 | [Pipeline, Detective Mode™ ve Multi-Agent nasıl çalışır?](makaleler/02-pipeline-detective-multi-agent.md) |
| 3 | [Geliştiriciler için Numex: CLI, Codex IDE, Agent ve Süper SDK](makaleler/03-gelistiriciler-icin-numex.md) |
| 4 | [Veri Türkiye'de kalır: KVKK ve Numex altyapısı](makaleler/04-kvkk-ve-altyapi.md) |
| 5 | [Numex ekosistemi: PC Doktoru, PusulamX ve ötesi](makaleler/05-numex-ekosistemi.md) |

## 🤝 Katkı

Bu depo Numex AI'ın **açık tanıtım ve dokümantasyon** deposudur. Yazım düzeltmeleri, çeviriler,
kullanım örnekleri ve yeni makaleler için Pull Request açabilirsiniz. Hata ve önerileriniz için
[Issues](../../issues) sekmesini kullanın.

## 📬 İletişim

- 🌐 [numexai.com.tr](https://numexai.com.tr)
- 📧 destek@numexai.com.tr
- 📸 [Instagram](https://instagram.com/numexai) · 💼 [LinkedIn](https://linkedin.com/company/numexai) · 🐦 [X / Twitter](https://twitter.com/numexai)

<div align="center">

---

**◆ Numex AI** — Dünya devleriyle inşa ettik. Anadolu için yoğurduk.<br>
🇹🇷 İstanbul'da geliştirildi

</div>
