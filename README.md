# arkose-scythe-data

[Scythe-Reaper](https://github.com/react-RE/arkose-scythe) aracı tarafından toplanan Arkose Labs bundle ve API verilerinin depolandığı repodur.

## İçerik

Her klasör bir session'u temsil eder:

```
bundles/2026-05-08T12-00-00Z/
├── metadata.json   # Session bilgisi, yakalanan dosyaların listesi
├── js/             # Arkose JS bundle'ları (game-core, enforcement, audio-ui)
├── api/            # API yanıtları (gfct, gt2, ca)
├── payloads/       # POST payload'ları
└── media/          # Audio dosyaları (MP3)
```

## Veri Toplama

Veriler [Scythe-Reaper](https://github.com/react-RE/arkose-scythe) tarafından GitHub signup akışı tetiklenerek toplanır. GitHub Actions ile her saat başı otomatik olarak çalışır.

Kendi verinizi toplamak için:

```bash
git clone https://github.com/react-RE/arkose-scythe.git
cd arkose-scythe
npm install
node src/scythe.mjs
```

Detaylı bilgi için: [github.com/react-RE/arkose-scythe](https://github.com/react-RE/arkose-scythe)

## Dosya Yapısı

Her session'da metadata.json dosyası yakalanan tüm verilerin detaylı listesini içerir:

```json
{
  "session": { "success": true, "retryCount": 0 },
  "captures": [
    { "url": "...", "label": "game-core", "size": 452301, "headers": {...}, "timing": {...} }
  ],
  "frames": [
    { "url": "...", "type": "arkose" }
  ]
}
```

## Lisans

AGPL-3.0
