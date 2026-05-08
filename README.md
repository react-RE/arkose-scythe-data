# arkose-scythe-data

**Arkose Labs JS bundle and API data archive / Arkose Labs JS bundle ve API veri arşivi**

[English](#english) | [Türkçe](#türkçe)

---

## English

### Overview

This repository stores Arkose Labs JS bundles, API responses, and payloads collected by [Scythe-Reaper](https://github.com/react-RE/arkose-scythe). Data is updated every hour.

### Contents

```
bundles/2026-05-08T12-00-00Z/
├── metadata.json   # Session info, captured files list
├── js/             # Arkose JS bundles (game-core, enforcement, audio-ui)
├── api/            # API responses (gfct, gt2, ca)
├── payloads/       # POST payloads
└── media/          # Audio files (MP3)
```

### Collect Your Own

```bash
git clone https://github.com/react-RE/arkose-scythe.git
cd arkose-scythe
npm install
node src/scythe.mjs
```

### License

AGPL-3.0

---

## Türkçe

### Genel Bakış

Bu repo, [Scythe-Reaper](https://github.com/react-RE/arkose-scythe) aracı tarafından toplanan Arkose Labs JS bundle'larını, API yanıtlarını ve payload'larını içerir. Veriler her saat başı güncellenir.

### İçerik

```
bundles/2026-05-08T12-00-00Z/
├── metadata.json   # Session bilgisi, yakalanan dosyaların listesi
├── js/             # Arkose JS bundle'ları (game-core, enforcement, audio-ui)
├── api/            # API yanıtları (gfct, gt2, ca)
├── payloads/       # POST payload'ları
└── media/          # Audio dosyaları (MP3)
```

### Kendi Verini Topla

```bash
git clone https://github.com/react-RE/arkose-scythe.git
cd arkose-scythe
npm install
node src/scythe.mjs
```

### Lisans

AGPL-3.0