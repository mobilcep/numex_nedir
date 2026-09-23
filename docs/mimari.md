# 🏗️ Numex Mimarisi

## Katmanlar

```mermaid
flowchart TB
  subgraph Istemciler[İstemciler]
    W[🌐 Web / PWA]
    CX[🧩 Codex Web · IDE · VS Code]
    CLI[⌨️ CLI]
    SDK[🧰 SDK / API istemcileri]
    OK[🎓 Okul]
    HUB[📦 Hub]
  end
  subgraph Sunucu[Numex Sunucu Katmanı · Türkiye]
    AUTH[🔐 OAuth · JWT · API anahtarları · cihaz kodu]
    ROUTER[🧭 Router · plan ve profil seçimi]
    PIPE[⚡ Pipeline · Boru 1 → Motor → Boru 2A → Boru 2B]
    DET[🕵️ Detective Mode™]
    MA[🤖 Multi-Agent Orkestratör]
    DV[🔬 DeepView™]
    TOOLS[🧰 Araçlar · web arama · kod çalıştırma · belge · vision · görsel · embedding]
  end
  subgraph Core[🏛️ Numex Core · istemci tarafı ajan motoru]
    SW[Swarm Council]
    FG[FinishGate]
    SH[Self-Healing]
    MEM[Self-Evolving Memory · .numex/]
    INF[3 katmanlı çıkarım · ONNX WASM → Ollama → Bulut]
  end
  subgraph Veri[Veri & Git]
    DB[(MongoDB)]
    FORGE[(🏗️ Forge · Gitea)]
  end
  subgraph Saglayici[Model sağlayıcıları]
    LLM[Google Cloud · Azure · Anthropic · Meta · DeepSeek]
  end

  W & SDK & OK & HUB --> AUTH --> ROUTER
  CX & CLI --> Core
  Core --> ROUTER
  ROUTER --> PIPE --> LLM
  PIPE --> DET & MA
  MA --> DV
  ROUTER --> TOOLS
  ROUTER --> DB
  HUB --> FORGE
  CX --> FORGE
```

## Bir isteğin yolculuğu

1. **Kimlik:** OAuth oturumu, JWT veya `nx_live_` API anahtarı doğrulanır.
2. **Router:** Kullanıcının planı ve seçtiği profil (Pro/Fast/Vision/Code) tespit edilir; istek uygun
   işlem hattına yönlendirilir.
3. **Boru 1:** Prompt güçlendirme, bağlam ekleme, uzman talimatları; `@karakter` varsa profil yüklenir.
4. **Mod tespiti:** Kritik soru → **Detective Mode**; çok alanlı soru / 2+ `@uzman` → **DeepView /
   Multi-Agent**; araç gerekiyorsa (web, kod, belge) → **araçlar**.
5. **AI Motor:** İş ortağı model(ler) yanıt üretir.
6. **Boru 2A:** Türkçe düzeltme, format, ton.
7. **Boru 2B:** Kalite kontrol ve doğrulama.
8. **Yanıt:** Akışlı (stream) olarak istemciye; sohbet geçmişi saklanır.

## Ajan tarafı (Core)

Codex ve CLI'de ajan **kullanıcının bilgisayarında** çalışır: dosyaları okur/yazar, komut çalıştırır,
testleri koşar. Sunucudan yalnızca model çağrısı alır. Plan → onay → uygula → **FinishGate kanıtı**
→ hafızaya kaydet döngüsü izlenir. Proje hafızası `.numex/` klasöründe açık dosyalar olarak durur.

## Teknoloji yığını

| Katman | Teknoloji |
|---|---|
| Sunucu | Node.js, Express, MongoDB, Redis, JWT, Passport (Google/GitHub OAuth) |
| Barındırma | Vercel (fra1) + Türkiye'de çift sunucu (2×256 GB RAM, SAS + NAS) |
| Ödeme | İyzico |
| Web arama | Serper |
| Ajan motoru | `@numex-ai/core` — Node 22+, `node:sqlite`, ONNX WASM, Ollama, Playwright |
| Editör | VS Code / VSCodium tabanlı Codex IDE; Monaco (Codex Web); tree-sitter |
| Git | Gitea (Forge) |
