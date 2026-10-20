# ⚔️ Zindan Ruhu

![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)
![No dependencies](https://img.shields.io/badge/dependencies-none-brightgreen)
![Platform](https://img.shields.io/badge/platform-web%20%7C%20mobile-orange)

Mobilde dikey modda oynanan, tarayıcıda çalışan **metin tabanlı roguelike**. Piksel kahramanınla zindanda otomatik savaş izle, boss'ları yen, eşya topla, karakterini geliştir.

**🎮 Oyna:** `https://<kullanici-adi>.github.io/zindan-ruhu/`

> English: A mobile-first, text-based roguelike with an auto-battling pixel hero, endless dungeon floors, boss fights every 10 floors, loot rarities, a blacksmith, a merchant and a (demo) store. Pure HTML/CSS/JS, zero dependencies.

## Özellikler

- **Sahneler:** Ana menü, Kasaba, Zindan, Demirci, Tüccar, Envanter, Karakter, Skor Tablosu, Mağaza
- **Zindan:** Otomatik savaş döngüsü, her katta daha fazla ve güçlü düşman, her 10. katta boss
- **Eşyalar:** 3 set (Demir, Çelik, Ejder) × kılıç/zırh × 4 nadirlik (Sıradan, Nadir, Destansı, Efsanevi), sınırsız envanter
- **İlerleme:** Seviye başına 3 stat puanı + 1 yetenek puanı, 3 yetenek
- **Ekonomi:** Altın, EXP ve elmas. Demirci eşya yükseltir (elmasla altınsız +15'e kadar)
- **Tüccar:** 8 ürün (6 altın, 2 elmas), ilerledikçe güçlü ürün şansı artar, yenileme 10 elmas
- **Mağaza (demo):** VIP, Savaş Bileti, reklam kaldırma, oto kat atlama, hızlandırma, elmas paketleri
- **Mobil öncelikli:** Dikey ekran, güvenli alan desteği, büyük dokunma alanları
- Yerel kayıt ve skor tablosu (`localStorage`)

## Çalıştırma

Derleme yok. İki yol:

```bash
# 1) Doğrudan aç
open index.html

# 2) Yerel sunucu
python3 -m http.server 8000   # http://localhost:8000
```

## GitHub Pages ile yayınlama

1. Repoyu GitHub'a gönder.
2. **Settings → Pages → Source: GitHub Actions** seç.
3. `main` dalına her push'ta `.github/workflows/pages.yml` siteyi otomatik yayınlar.

## Proje yapısı

```
├── index.html          # Sayfa iskeleti
├── css/style.css       # Stiller
├── js/game.js          # Oyun mantığı ve çizim
├── .github/workflows/  # Pages dağıtımı
├── CHANGELOG.md
├── CONTRIBUTING.md
└── LICENSE
```

## ⚠️ Bilinen sınırlar

- **Mağaza demodur.** Gerçek ödeme alınmaz, satın alınan ürün test için eklenir.
- Tüm veriler tarayıcıda (`localStorage`) tutulur ve oyuncu tarafından değiştirilebilir. Gerçek para ve global skor tablosu için sunucu tarafı (hesap, ödeme doğrulama) gerekir.
- Skor tablosu yalnızca cihaza özeldir.

## Yol haritası

- [ ] Online skor tablosu ve hesaplar
- [ ] Gerçek ödeme entegrasyonu (sunucu doğrulamalı)
- [ ] Günlük görevler, seviyeli Battle Pass
- [ ] Ses ve müzik
- [ ] Sınıflar, pet'ler, yeni setler
- [ ] Çoklu dil

## Lisans

[MIT](LICENSE)
