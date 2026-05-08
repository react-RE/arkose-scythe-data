# arkose-scythe-data

**Arkose Labs bundle and API data archive / Arkose Labs bundle ve API veri arşivi**

[English](#english) | [Türkçe](#türkçe)

---

## English

### Overview

This repository stores Arkose Labs JS bundles, API responses, and payloads collected by [Scythe-Reaper](https://github.com/react-RE/arkose-scythe).

### Contents

Each directory represents a collection session:

```
bundles/2026-05-08T12-00-00Z/
├── metadata.json   # Session info, captured files list
├── js/             # Arkose JS bundles (game-core, enforcement, audio-ui)
├── api/            # API responses (gfct, gt2, ca)
├── payloads/       # POST payloads
└── media/          # Audio files (MP3)
```

### Data Collection

Data is collected by [Scythe-Reaper](https://github.com/react-RE/arkose-scythe) by triggering GitHub signup flow. The tool runs automatically every hour via GitHub Actions.

To collect your own data:

```bash
git clone https://github.com/react-RE/arkose-scythe.git
cd arkose-scythe
npm install
node src/scythe.mjs
```

For details: [github.com/react-RE/arkose-scythe](https://github.com/react-RE/arkose-scythe)

### File Structure

Each session includes a `metadata.json` with detailed capture information:

```json
{
  "session": { "success": true, "retryCount": 0 },
  "captures": [
    { "url": "...", "label": "game-core", "size": 452301, "headers": {...}, "timing": {...} }
  ],
  "frames": [
    { "id": "...", "url": "...", "type": "arkose" }
  ]
}
```

### License

AGPL-3.0

---

## Türkçe

### Genel Bakış

Bu repo, [Scythe-Reaper](https://github.com/react-RE/arkose-scythe) aracı tarafından toplanan Arkose Labs JS bundle'larını, API yanıtlarını ve payload'larını içerir.

### İçerik

Her klasör bir collection session'ını temsil eder:

```
bundles/2026-05-08T12-00-00Z/
├── metadata.json   # Session bilgisi, yakalanan dosyaların listesi
├── js/             # Arkose JS bundle'ları (game-core, enforcement, audio-ui)
├── api/            # API yanıtları (gfct, gt2, ca)
├── payloads/       # POST payload'ları
└── media/          # Audio dosyaları (MP3)
```

### Veri Toplama

Veriler [Scythe-Reaper](https://github.com/react-RE/arkose-scythe) tarafından GitHub signup akışı tetiklenerek toplanır. GitHub Actions ile her saat başı otomatik olarak çalışır.

Kendi verinizi toplamak için:

```bash
git clone https://github.com/react-RE/arkose-scythe.git
cd arkose-scythe
npm install
node src/scythe.mjs
```

Detaylı bilgi için: [github.com/react-RE/arkose-scythe](https://github.com/react-RE/arkose-scythe)

### Dosya Yapısı

Her session'da metadata.json dosyası yakalanan tüm verilerin detaylı listesini içerir:

```json
{
  "session": { "success": true, "retryCount": 0 },
  "captures": [
    { "url": "...", "label": "game-core", "size": 452301, "headers": {...}, "timing": {...} }
  ],
  "frames": [
    { "id": "...", "url": "...", "type": "arkose" }
  ]
}
```

### Lisans

AGPL-3.0
