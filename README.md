# internet-programciligi
# Haber Portalı Projesi

Dudidem Zehra Yüksekkolaşin
Öğrenci no: 22480717
Tc: 10493451760

Projenin Amacı
Bu proje, güncel haberlerin paylaşılabileceği, kullanıcıların yorum yapabileceği ve birbirleriyle mesajlaşabileceği modern bir haber portalı web uygulaması olarak geliştirilmiştir. Proje, günümüz web teknolojilerini kullanarak hızlı, güvenli ve kullanıcı dostu bir haber platformu sunmayı amaçlamaktadır.

Proje, aşağıdaki problemlere çözüm sunmaktadır:
Haber Erişimi: Kullanıcıların güncel haberlere kategorilere göre kolayca erişebilmesi
Etkileşim: Kullanıcıların haberler hakkında yorum yapabilmesi ve tartışabilmesi
İletişim: Kullanıcılar arası doğrudan mesajlaşma imkanı
İçerik Yönetimi: Admin kullanıcıların içerikleri kolayca yönetebilmesi
Rol Tabanlı Erişim: Farklı kullanıcı rollerine göre özelleştirilmiş erişim kontrolü
Genel İşleyiş
Sistem, rol tabanlı bir erişim kontrolü ile çalışmaktadır:
Ziyaretçiler: Kayıt olmadan haberleri görüntüleyebilir
Normal Kullanıcılar: Haberlere yorum yapabilir, diğer kullanıcılarla mesajlaşabilir ve kendi profillerini düzenleyebilir
Admin Kullanıcılar: Haberleri ekleyebilir/düzenleyebilir/silebilir, kategorileri yönetebilir, kullanıcıları yönetebilir ve sistem istatistiklerini görüntüleyebilir

Kullanılan Teknolojiler
Next.js 14: React tabanlı modern web framework
Prisma ORM: Tip güvenli veritabanı işlemleri için
SQLite: Hafif, dosya tabanlı veritabanı
TailwindCSS: Hızlı ve responsive tasarım için
NextAuth.js: Kimlik doğrulama ve oturum yönetimi
Rapor, ZIP dosyasına eklenmiştir ve hocanız için detaylı bilgileri içermektedir.

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

ADIM 4: Veritabanının Oluşturulması
Aşağıdaki komutu çalıştırarak veritabanını oluşturun:
npx prisma migrate dev
Komut çalıştırıldığında migration için bir isim girmeniz istenebilir, herhangi bir isim girebilirsiniz
(örneğin "initial").
ADIM 5: Projeyi Çalıştırma
Aşağıdaki komutu çalıştırarak geliştirme sunucusunu başlatın:
npm run dev
Tarayıcınızda http://localhost:3000 adresine giderek projeyi görüntüleyebilirsiniz.
ADIM 6: Admin Girişi
Admin paneline erişmek için:
E-posta: admin@example.com
Şifre: admin123
