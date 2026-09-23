# Geliştiriciler İçin Numex: CLI, Codex IDE, Agent ve Süper SDK

Numex AI yalnızca bir sohbet arayüzü değil; terminalde, editörde ve kendi uygulamanızda çalışan bir
geliştirici platformu.

## ⌨️ Numex CLI — terminalden otonom asistan

```powershell
irm https://www.numexai.com.tr/install-cli.ps1 | iex   # Node.js 18+
numex --version
numex basla
```

- **Terminal sohbeti:** Proje klasöründe dosya okuma/yazma, git işlemleri ve RAG tabanlı kod arama.
- **Uzaktan PC:** `numex uzak install` ile arka plan köprüsü kurulur (sistem tepsisinde Numex ikonu).
  Artık telefonunuzdan veya başka bir cihazdan kendi bilgisayarınıza klasör oluşturabilir, dosya
  yazabilir ve komut çalıştırabilirsiniz. `numex uzak pause` ile duraklatın.
- Numex hesabınızın token bakiyesi veya API anahtarıyla çalışır.

## 🧩 Numex Codex IDE

VS Code altyapısı üzerine kurulu, yapay zeka entegreli masaüstü editör: sohbet paneli, ajanlar,
satır içi düzenleme ve terminal entegrasyonu tek yerde.

## 🤖 Agent modu — sizin yerinize kodlar, sizin onayınızla

Agent modu öneri vermekle kalmaz, dosyalarınıza doğrudan değişiklik uygular — ama kontrol sizde:

1. **İstek gönder:** *"Login sayfasını düzelt"*
2. **AI planlar:** Hangi dosyaların ve satırların etkileneceğini analiz eder.
3. **Diff göster:** Eski kod kırmızı, yeni kod yeşil — yan yana.
4. **Kabul / reddet:** Tek tek veya toplu; reddederseniz dosyalar eski haline döner.

## 🧠 Profiller

| Profil | Ne zaman? |
|---|---|
| **Numex Code** | Debug, refactor, test ve dokümantasyon |
| **Numex Pro** | 128K bağlamla büyük kod tabanları ve derin analiz |
| **Numex Fast** | Hızlı kod tamamlama ve anlık sorular |
| **Numex Vision** | Ekran görüntüsü / tasarım analizi |

128K bağlam, 300+ sayfalık belge ya da uzun kod tabanlarıyla tek seferde çalışabilmek demektir.

## 🏛️ "Süper SDK" mimarisi

Numex'in geliştirici araçları tek bir çekirdek üzerinde birleşir:

```
                ┌──────────────────────────┐
                │   @numex-ai/core         │  AI bağlantıları, dosya sistemi,
                │   (Süper SDK)            │  telemetri, ajan akışları
                └────────────┬─────────────┘
          ┌──────────────────┼──────────────────┐
     numex-cli          numex-vscode        numexcodex-sdk
   (ince terminal     (ince editör         (uygulamanıza
      kabuğu)            kabuğu)             gömün)
```

Faydası: terminaldeki komut ile editördeki buton **aynı çekirdekten** beslenir — "terminalde
çalışıyor, butonda patlıyor" hataları ortadan kalkar; ajanlar da string ayrıştırmak yerine yapısal
JSON yanıtlarla çalışır.

## 🔌 API

Numex PRO ve Advanced planlarında **CLI + API erişimi** dahildir. Belgeler:
[numexai.com.tr](https://numexai.com.tr) → API Dokümantasyonu.

---
*#NumexAI #DeveloperTools #CLI #AIAgent #VSCode*
