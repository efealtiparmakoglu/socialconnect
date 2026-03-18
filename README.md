# 📱 SocialConnect - Modern Sosyal Medya Platformu

[![React](https://img.shields.io/badge/React-18.0+-61DAFB?logo=react)](https://reactjs.org/)
[![Node.js](https://img.shields.io/badge/Node.js-18.0+-339933?logo=node.js)](https://nodejs.org/)
[![MongoDB](https://img.shields.io/badge/MongoDB-6.0+-47A248?logo=mongodb)](https://mongodb.com/)
[![Socket.io](https://img.shields.io/badge/Socket.io-4.0+-010101?logo=socket.io)](https://socket.io/)

🚀 **SocialConnect**, Instagram ve Facebook'tan ilham alınmış, gerçek zamanlı mesajlaşma, hikayeler ve sosyal etkileşim özellikleri içeren modern bir sosyal medya platformudur.

## ✨ Özellikler

### 📸 Paylaşım Özellikleri
- 📷 **Fotoğraf & Video Paylaşımı** - HD kalitesinde medya yükleme
- 🎞️ **Hikayeler (Stories)** - 24 saatlik geçici içerikler
- 🎬 **Reels** - Kısa video formatı
- 📝 **Metin Gönderileri** - Zengin metin editörü

### 💬 Etkileşim
- 💬 **Gerçek Zamanlı Mesajlaşma** - WebSocket tabanlı anlık mesajlaşma
- 👥 **Grup Sohbetleri** - Çoklu kullanıcı sohbet odaları
- 🔔 **Bildirim Sistemi** - Anlık push bildirimler
- ❤️ **Beğeni & Yorum** - Sosyal etkileşim özellikleri

### 🔍 Keşif
- 🔎 **Geliişmiş Arama** - Kullanıcı ve içerik arama
- 🏷️ **Etiketler** - Konu bazlı içerik keşfi
- 🌟 **Keşfet Sayfası** - Kişiselleştirilmiş içerik akışı

## 🛠️ Teknoloji Stack

### Frontend
- ⚛️ **React 18** - Modern UI kütüphanesi
- 📱 **React Native** - Mobil uygulama (iOS/Android)
- 🎨 **Tailwind CSS** - Utility-first CSS framework
- 🔄 **Redux Toolkit** - State yönetimi
- 🎯 **React Query** - Server state yönetimi

### Backend
- 🟢 **Node.js** - JavaScript runtime
- 🚀 **Express.js** - Web framework
- 🍃 **MongoDB** - NoSQL veritabanı
- ⚡ **Redis** - Önbellek ve real-time data
- 🔌 **Socket.io** - WebSocket iletişimi
- 🔐 **JWT** - Kimlik doğrulama

### DevOps
- 🐳 **Docker** - Containerization
- ☸️ **Kubernetes** - Orchestration
- 📊 **Prometheus + Grafana** - Monitoring
- 🌩️ **AWS** - Cloud infrastructure

## 🚀 Kurulum

### Gereksinimler
- Node.js 18+
- MongoDB 6+
- Redis 7+

### Backend Kurulumu
```bash
# Repoyu klonla
git clone https://github.com/efealtiparmakoglu/socialconnect.git
cd socialconnect

# Bağımlılıkları yükle
npm install

# Ortam değişkenlerini ayarla
cp .env.example .env
# .env dosyasını düzenle

# Sunucuyu başlat
npm run dev
```

### Frontend Kurulumu
```bash
cd client
npm install
npm start
```

## 📁 Proje Yapısı

```
socialconnect/
├── 📁 client/                 # React Frontend
│   ├── 📁 src/
│   │   ├── 📁 components/     # UI Bileşenleri
│   │   ├── 📁 pages/          # Sayfalar
│   │   ├── 📁 store/          # Redux Store
│   │   └── 📁 hooks/          # Custom Hooks
│   └── package.json
├── 📁 server/                 # Node.js Backend
│   ├── 📁 config/             # Yapılandırma
│   ├── 📁 controllers/        # İş Mantığı
│   ├── 📁 models/             # Veritabanı Modelleri
│   ├── 📁 routes/             # API Rotaları
│   ├── 📁 middleware/         # Middleware
│   ├── 📁 utils/              # Yardımcı Fonksiyonlar
│   └── server.js              # Ana Sunucu
├── 📁 socket/                 # WebSocket Sunucusu
└── 📄 docker-compose.yml      # Docker Konfigürasyonu
```

## 🔌 API Endpoints

### Kimlik Doğrulama
| Method | Endpoint | Açıklama |
|--------|----------|----------|
| POST | `/api/auth/register` | Kayıt ol |
| POST | `/api/auth/login` | Giriş yap |
| POST | `/api/auth/social/google` | Google ile giriş |
| GET | `/api/auth/me` | Profil bilgisi |

### Gönderiler
| Method | Endpoint | Açıklama |
|--------|----------|----------|
| GET | `/api/posts` | Akışı getir |
| POST | `/api/posts` | Yeni gönderi |
| POST | `/api/posts/:id/like` | Beğen |
| POST | `/api/posts/:id/comment` | Yorum yap |

### Mesajlaşma
| Method | Endpoint | Açıklama |
|--------|----------|----------|
| GET | `/api/messages/conversations` | Konuşmalarım |
| GET | `/api/messages/:userId` | Mesaj geçmişi |
| POST | `/api/messages` | Mesaj gönder |

## 🧪 Test

```bash
# Unit testler
npm test

# E2E testler
npm run test:e2e

# Coverage raporu
npm run test:coverage
```

## 🚀 Deployment

### Docker ile
```bash
docker-compose up -d
```

### Production Build
```bash
npm run build
npm start
```

## 📝 Ortam Değişkenleri

```env
# Server
PORT=5000
NODE_ENV=production
MONGODB_URI=mongodb://localhost:27017/socialconnect
REDIS_URL=redis://localhost:6379
JWT_SECRET=your-super-secret-key
JWT_EXPIRE=7d

# AWS S3
AWS_ACCESS_KEY_ID=your-access-key
AWS_SECRET_ACCESS_KEY=your-secret-key
AWS_BUCKET_NAME=socialconnect-media
AWS_REGION=eu-west-1

# Firebase (Push Notifications)
FIREBASE_SERVER_KEY=your-firebase-key

# Socket.io
SOCKET_CORS_ORIGIN=http://localhost:3000
```

## 🎯 SEO Optimizasyonları

- ✅ **SSR (Server-Side Rendering)** - React Helmet ile meta tag yönetimi
- ✅ **Open Graph Tags** - Sosyal medya paylaşımları için optimize edilmiş
- ✅ **Structured Data** - Schema.org markup
- ✅ **Lazy Loading** - Görsel optimizasyonu
- ✅ **CDN** - Medya dosyaları için AWS CloudFront
- ✅ **PWA** - Offline çalışma desteği

## 🔒 Güvenlik

- 🔐 **JWT Authentication** - Güvenli kimlik doğrulama
- 🛡️ **Helmet.js** - HTTP header güvenliği
- 🚫 **Rate Limiting** - DDoS koruması
- 📝 **Input Validation** - XSS ve NoSQL injection koruması
- 🔒 **CORS** - Cross-origin kaynak paylaşımı kontrolü

## 📸 Ekran Görüntüleri

```
┌─────────────────────────────────────────────────────────────┐
│  📱 SocialConnect      🔍 🔔 ✉️ 👤                           │
├─────────────────────────────────────────────────────────────┤
│  ┌─────────────────────────────────────────────────────┐   │
│  │           📸 Hikayeler                              │   │
│  │  ┌────┐ ┌────┐ ┌────┐ ┌────┐ ┌────┐              │   │
│  │  │ 👤 │ │ 👤 │ │ 👤 │ │ 👤 │ │ 👤 │              │   │
│  │  │ +  │ │ Ahmet│ │ Zeynep│ │ Can │ │ Mehmet│      │   │
│  │  └────┘ └────┘ └────┘ └────┘ └────┘              │   │
│  └─────────────────────────────────────────────────────┘   │
│                                                             │
│  👤 Ahmet Yılmaz                    ⋮ 🌐 2 saat önce      │
│  ┌─────────────────────────────────────────────────────┐   │
│  │                                                     │   │
│  │         [📸 Muhteşem Manzara Fotoğrafı]            │   │
│  │                                                     │   │
│  └─────────────────────────────────────────────────────┘   │
│  ❤️ 1,234 Beğeni  💬 89 Yorum  ↗️ Paylaş                   │
│  Harika bir gün! 🌅 #manzara #doğa #tatil                  │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

## 🤝 Katkıda Bulunma

1. Fork yapın
2. Feature branch oluşturun (`git checkout -b feature/amazing-feature`)
3. Commit yapın (`git commit -m 'Add amazing feature'`)
4. Push yapın (`git push origin feature/amazing-feature`)
5. Pull Request açın

## 📄 Lisans

Bu proje [MIT](LICENSE) lisansı altında lisanslanmıştır.

## 👨‍💻 Geliştirici

**Efe Altıparmakoğlu**
- 🌐 Website: [bananashosting.com](https://www.bananashosting.com)
- 💼 LinkedIn: [linkedin.com/in/efealtiparmakoglu](https://linkedin.com/in/efealtiparmakoglu)
- 🐦 Twitter: [@efealtiparmak](https://twitter.com/efealtiparmak)
- 📧 Email: efealtiparmakoglu@hotmail.com

---

⭐ **Bu projeyi beğendiyseniz star atmayı unutmayın!**

## 🔗 Bağlantılar

- [🌐 Live Demo](https://socialconnect-demo.vercel.app)
- [📖 Documentation](https://docs.socialconnect.app)
- [🐛 Bug Report](https://github.com/efealtiparmakoglu/socialconnect/issues)
- [💡 Feature Request](https://github.com/efealtiparmakoglu/socialconnect/discussions)

---

<p align="center">
  Made with ❤️ by <a href="https://github.com/efealtiparmakoglu">Efe Altıparmakoğlu</a>
</p>