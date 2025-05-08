# FastAPI Template Project

Bu proje, FastAPI kullanarak bir REST API geliştirmek için temel bir şablon içerir.

## Özellikler

- 🔐 JWT tabanlı kimlik doğrulama sistemi
- 👤 Kullanıcı yönetimi (kayıt, giriş, profil)
- 📝 Item CRUD işlemleri
- 🗄️ SQLAlchemy ORM ile veritabanı yönetimi
- ✅ Pydantic ile veri doğrulama
- 📚 Swagger/OpenAPI otomatik dökümantasyonu
- 🔒 Güvenli şifre hashleme
- 🚀 Yüksek performanslı async yapı
- 🛠️ Modüler ve genişletilebilir mimari

## Kurulum

1. Gerekli paketleri yükleyin:
```bash
pip install -r requirements.txt
```

2. Uygulamayı çalıştırın:
```bash
uvicorn main:app --reload
```

3. API dokümantasyonuna erişin:
- Swagger UI: http://localhost:8000/docs
- ReDoc: http://localhost:8000/redoc

## Task Listesi ve İlerleme Durumu

### 1. Temel CRUD İşlemleri ✅
- ✅ User modeli için CRUD işlemleri
- ⬜ Item modeli için CRUD işlemleri
- ⬜ Kullanıcıya özel item'ları listeleme

### 2. Authentication ve Authorization ⏳
- ⬜ JWT token tabanlı authentication sistemi
- ⬜ Password hashing ve doğrulama
- ⬜ Protected route'lar
- ⬜ Token yenileme mekanizması

### 3. Validation ve Error Handling ⏳
- ⬜ Input validation için Pydantic modellerini genişletme
- ⬜ Custom exception handler'lar
- ⬜ Rate limiting implementasyonu

### 4. Database ve Migration ⏳
- ⬜ Alembic ile database migration sistemi
- ⬜ Seed data oluşturma
- ⬜ Database backup sistemi

### 5. Testing ⏳
- ⬜ Unit testler
- ⬜ Integration testler
- ⬜ API endpoint'leri için test coverage

### 6. API Geliştirmeleri ⏳
- ⬜ Pagination implementasyonu
- ⬜ Filtering ve sorting özellikleri
- ⬜ API versiyonlama sistemi

### 7. Güvenlik ⏳
- ⬜ CORS ayarları
- ⬜ Rate limiting
- ⬜ Input sanitization

### 8. Monitoring ve Logging ⏳
- ⬜ Logging sistemi
- ⬜ Performance monitoring
- ⬜ Health check endpoint'leri

## Proje Yapısı

```
.
├── main.py           # Ana uygulama dosyası
├── database.py       # Database konfigürasyonu
├── models.py         # SQLAlchemy modelleri
├── schemas.py        # Pydantic şemaları
├── requirements.txt  # Proje bağımlılıkları
└── README.md         # Proje dokümantasyonu
```

## API Endpoints

### User Endpoints
- `POST /users/` - Yeni kullanıcı oluşturma
- `GET /users/` - Tüm kullanıcıları listeleme
- `GET /users/{user_id}` - Belirli bir kullanıcının bilgilerini getirme
- `PUT /users/{user_id}` - Kullanıcı bilgilerini güncelleme
- `DELETE /users/{user_id}` - Kullanıcı silme

## Notlar

- Her task'ı tamamladıktan sonra test etmeyi unutmayın
- Kod kalitesi ve best practice'lere dikkat edin
- Her değişikliği commit'leyin ve açıklayıcı commit mesajları yazın
