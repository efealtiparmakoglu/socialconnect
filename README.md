# 📱 SocialConnect

Full-stack sosyal medya platformu. Instagram/Facebook tarzı.

## Özellikler
- 📸 Fotoğraf/video paylaşımı
- 💬 Gerçek zamanlı mesajlaşma (Socket.io)
- 🔔 Bildirim sistemi
- 🔍 Keşfet sayfası
- 👥 Grup oluşturma
- 📊 Hikayeler (Stories)
- ❤️ Beğeni ve yorum

## Teknolojiler
- React Native + React Web
- Node.js + Express
- MongoDB + Redis
- Socket.io
- AWS S3

## Kurulum
```bash
npm install
npm run dev
```

## API
```javascript
POST /api/posts
GET /api/feed
POST /api/messages
```

## Ekran Görüntüsü
```
┌─────────────────────────────────────┐
│  📱 SocialConnect      🔍 🔔 ✉️ 👤  │
├─────────────────────────────────────┤
│  ┌─────────────────────────────┐   │
│  │    📸 Hikayeler            │   │
│  │  [👤][👤][👤][👤][👤]      │   │
│  └─────────────────────────────┘   │
│                                     │
│  👤 Ahmet                    ⋮     │
│  ┌─────────────────────────────┐   │
│  │                             │   │
│  │      [📸 Fotoğraf]         │   │
│  │                             │   │
│  └─────────────────────────────┘   │
│  ❤️ 234  💬 45  ↗️                │
│  Harika bir gün! 🌞                │
│                                     │
└─────────────────────────────────────┘
```

**Efe Altıparmakoğlu** - 2024
