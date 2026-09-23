# Geliştiriciler İçin Numex: Codex, CLI, SDK, API, Hub ve Forge

> **Editörüne Türkçe düşünen bir kod ajanı.** İste, yazsın, çalıştırsın — iş bitene kadar.
> — [codex.numexai.com.tr](https://codex.numexai.com.tr)

Numex'in geliştirici tarafı tek bir fikre dayanır: **aynı çekirdek, her yerde.** Terminaldeki komut,
editördeki buton, tarayıcıdaki sohbet ve sizin uygulamanızdaki SDK çağrısı aynı `@numex-ai/core`
motorunu çalıştırır.

## 1. Codex — üç kapı, tek ajan

| | Kurulum | Ne zaman? |
|---|---|---|
| 🌐 **Codex Web** | Yok, tarayıcıda | Hızlı prototip; *"hesap makinesi yap"* → dosyalar editöre yazılır, önizleme güncellenir, **Yayınla** |
| 🧩 **Codex IDE** (v2.9.59, ~162 MB) | Windows masaüstü | Günlük profesyonel geliştirme |
| 🧩 **VS Code eklentisi** | Mevcut VS Code'a | Alışkanlığınızı bozmadan |

IDE'deki asistan **Numex Çözüm** dört modda çalışır: **Sohbet** (soru-cevap), **Plan** (kod
değiştirmeden yol haritası), **Otonom** (plan → onay → uygula → doğrula) ve **Hata Avcısı** (log ve
çıktıdan kök neden). Yanında: `Ctrl+K` satır içi düzenleme, `Tab` ile sonraki düzenleme, Kod Lens,
anlamsal arama, commit mesajı / PR üretimi, arka plan ve bulut ajanları, SSH/WSL.

Ajan ne bildiğini ve ne yaptığını gizlemez: her projede açık bir **`.numex/`** klasörü tutar — RAG
indeksi, denetim izi (`audit-trail.jsonl`), geri alma noktaları, öğrenilen hatalar, token kullanımı.

## 2. CLI — terminal ve uzak PC

```bash
npm i -g @numexai/cli
numex login
numex                                   # terminal sohbeti
numex plan "ödeme modülü ekle"          # sadece plan
numex mission "testleri yeşile çek"     # uzun süreli otonom misyon
numex undo                              # son turu geri al
numex --offline "yerel Ollama ile yaz"  # internetsiz
numex uzak install                      # telefondan PC'ye komut köprüsü
```

Öne çıkan mühendislik: diff hunk'larıyla **cerrahi yama**, arka plan süreç hatalarını ~2 sn'de
yakalayan **subshell intercept**, **BM25 + AST** kod indeksi, **MCP** istemcisi ve kanıtsız "bitti"
dedirtmeyen **FinishGate**.

## 3. SDK ve API

```javascript
const { Numex } = require('numexcodex-sdk');
const numex = new Numex({ apiKey: process.env.NUMEX_API_KEY });
await numex.chat.completions.create({ messages: [{ role: 'user', content: 'Merhaba' }] });
```

Modeller: `numex-pro` (128K, function calling) · `numex-fast` (~3× hızlı) · `numex-think`
(chain-of-thought) · `numex-vision` (OCR) · `numex-code` (64K, 25+ dil). Uç noktalar: chat, stream,
agent, vision, images, embeddings, search. İlk kayıtta **100.000 token** hediye.

SDK'nın **CLI Bridge**'i ile CI hattınıza ya da kendi aracınıza CLI'nin tüm otonom gücünü tek satırla
gömebilirsiniz.

## 4. Hub ve Forge — kodun evi

- **Forge** ([forge.numexai.com.tr](https://forge.numexai.com.tr)): Gitea tabanlı, Türkçe Git sunucusu —
  konular, değişiklik istekleri, kilometre taşları, keşfet.
- **Hub** ([hub.numexai.com.tr](https://hub.numexai.com.tr)): Deponu bilen yapay zeka. *"README'yi
  güncelle"* dersin, önerir, **Uygula** dersin, Forge'a commit'lenir. **Topluluk Vitrini**'nde trend
  depolar, canlı akış ve tek tıkla **çatalla**.

## 5. Market — ne üretebildiğinin kanıtı

[market.numexai.com.tr](https://market.numexai.com.tr): Numex'in sıfırdan, otonom ürettiği **44
açık kaynak uygulama**. Canlı dene (ör. saf Web Audio API ile çalışan ritim makinesi **Cyber Beats**),
kodunu Forge'da incele, Hub'da çatalla, Codex'te değiştir.

---
*#NumexAI #Codex #DeveloperTools #CLI #AIAgent*
