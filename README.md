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

## Task Listesi

### 1. Temel CRUD İşlemleri
- [ ] User modeli için CRUD endpoint'leri oluşturun (create, read, update, delete)
- [ ] Item modeli için CRUD endpoint'leri oluşturun
- [ ] Kullanıcıya özel item'ları listeleyen endpoint ekleyin

### 2. Authentication ve Authorization
- [ ] JWT token tabanlı authentication sistemi implementasyonu
- [ ] Password hashing ve doğrulama
- [ ] Protected route'lar oluşturun
- [ ] Token yenileme mekanizması ekleyin

### 3. Validation ve Error Handling
- [ ] Input validation için Pydantic modellerini genişletin
- [ ] Custom exception handler'lar ekleyin
- [ ] Rate limiting implementasyonu yapın

### 4. Database ve Migration
- [ ] Alembic ile database migration sistemi kurun
- [ ] Seed data oluşturun
- [ ] Database backup sistemi ekleyin

### 5. Testing
- [ ] Unit testler yazın
- [ ] Integration testler ekleyin
- [ ] API endpoint'leri için test coverage raporu oluşturun

### 6. API Geliştirmeleri
- [ ] Pagination implementasyonu
- [ ] Filtering ve sorting özellikleri ekleyin
- [ ] API versiyonlama sistemi kurun

### 7. Güvenlik
- [ ] CORS ayarlarını yapılandırın
- [ ] Rate limiting ekleyin
- [ ] Input sanitization implementasyonu yapın

### 8. Monitoring ve Logging
- [ ] Logging sistemi kurun
- [ ] Performance monitoring ekleyin
- [ ] Health check endpoint'lerini genişletin

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
