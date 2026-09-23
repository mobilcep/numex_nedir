# Kendi Kendini Doğrulayan Yapay Zeka: Okul, Market ve FinishGate

Büyük dil modellerinin en bilinen zaafı **kendinden emin hatalardır**: yanlış bir cevabı, doğrusu
kadar akıcı söylerler. Numex bu soruna tek bir ilkeyle yaklaşır: **iddia değil, kanıt.** Bu ilke
ekosistemin üç farklı köşesinde, üç farklı biçimde uygulanır.

## 1. Sohbette: Detective Mode™

Kritik bir soru geldiğinde tek model yerine üç yaklaşım çalışır — **hızlı analiz**, **derin analiz**,
**alternatif bakış**. Bir hakem sistemi çözümleri karşılaştırır ve kazananı **gerekçesiyle** sunar.
*"Tek model yanılabilir. Üçü birden yanılmaz."*

## 2. Eğitimde: Numex Okul'un çift doğrulaması

Bir test sorusunun cevap anahtarı yanlışsa, öğrenci doğru bildiği şeyi yanlış öğrenir. Numex Okul'da:

| Soru | Hazırlayan AI | Doğrulayan AI | Sonuç |
|---|---|---|---|
| 1 | B | B | ✅ Onaylandı |
| 2 | C | A | ❌ Elendi → yeni soru üretilir, aynı kontrolden geçer |
| 3 | D | D | ✅ Onaylandı |

İki yapay zekanın bağımsız cevabı uyuşmayan soru **teste girmez**.
→ [okul.numexai.com.tr](https://okul.numexai.com.tr)

## 3. Kodda: FinishGate

Kod ajanlarının klasik hatası: *"Tamamlandı!"* deyip çalışmayan kod teslim etmek. Numex Core'da
**FinishGate** bunu yasaklar. Görev ancak **canlı kanıtla** kapanır:

- sunucu gerçekten **HTTP 200** dönüyor mu,
- **birim testleri** geçiyor mu,
- **DOM** beklenen öğeleri içeriyor mu (Omni-Vision ile tarayıcıda görsel kontrol).

Kanıt yoksa ajan **Self-Healing** döngüsüne döner ve düzeltir.

## Sonuç: Market

Bu ilkenin en görünür çıktısı **Numex Market**: Numex'in otonom ürettiği, çalıştırılıp doğrulanmış
44 uygulama — hepsi açık kaynak. Birini aç (ör. Cyber Beats ritim makinesi), çalıştığını gör, kodunu
Forge'da incele. İddia değil, kanıt.
→ [market.numexai.com.tr](https://market.numexai.com.tr)

## Küçük ama anlamlı bir ayrıntı

Codex IDE'nin token kullanım ekranında şu not yazar: *"Uydurma sayı göstermek yerine bu bölüm gerçek
veri gelene kadar kaldırıldı."* Doğrulama kültürü, en küçük panele kadar iner.

---
*#NumexAI #DetectiveMode #NumexOkul #FinishGate #YapayZekaGüvenilirliği*
