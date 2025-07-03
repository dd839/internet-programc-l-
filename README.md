# internet-programc-l-
# Haber Portalı Projesi

Bu proje, Next.js kullanılarak geliştirilmiş bir haber portalı web sitesidir.

## Özellikler

- Kullanıcı kaydı ve girişi
- Rol tabanlı erişim kontrolü (admin/normal kullanıcı)
- Haber yönetimi (ekleme, düzenleme, silme)
- Kategori yönetimi
- Yorum sistemi
- Kullanıcılar arası mesajlaşma

## Teknolojiler

- Next.js 14
- Prisma ORM
- SQLite veritabanı
- Tailwind CSS
- NextAuth.js (kimlik doğrulama)

## Kurulum

1. Bağımlılıkları yükleyin:
npm install

2. Veritabanını oluşturun:
npx prisma migrate dev

3. Geliştirme sunucusunu başlatın:
npm run dev

4. Tarayıcınızda http://localhost:3000 adresine gidin.
5. HABER PORTALI PROJESİ KURULUM ADIMLARI
=====================================
ADIM 1: Node.js Kurulumu
-----------------------
Eğer bilgisayarınızda Node.js kurulu değilse, https://nodejs.org adresinden indirip kurmanız gerekiyor.
(LTS sürümünü indirmeniz önerilir)

ADIM 2: Proje Dosyalarının Çıkarılması
-------------------------------------
haber-portal-projesi-final.zip dosyasını bir klasöre çıkarın.

ADIM 3: Bağımlılıkların Yüklenmesi
---------------------------------
Komut istemcisini açın (CMD veya PowerShell) ve projenin bulunduğu klasöre gidin:
cd "projenin_bulunduğu_klasör_yolu"

Ardından aşağıdaki komutu çalıştırın:
npm install

Bu komut, package.json dosyasında belirtilen tüm bağımlılıkları yükleyecektir.
