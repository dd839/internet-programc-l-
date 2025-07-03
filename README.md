# internet-programciligi
# Haber Portalı Projesi

Dudidem Zehra Yüksekkolaşin
Öğrenci no: 22480717
Tc: 10493451760


Günümüzde bilgiye hızlı, güvenilir ve kolay erişim büyük önem taşımaktadır. Dijitalleşmenin hızla arttığı bu çağda, kullanıcıların güncel haberlere anında ulaşabileceği platformlara olan ihtiyaç da her geçen gün artmaktadır. Bu ihtiyaca yönelik olarak geliştirdiğimiz Haber Portalı, kullanıcı dostu bir arayüzle, farklı kategorilerdeki haberleri tek bir platformda toplayan dinamik ve etkileşimli bir web uygulamasıdır.

Bu proje, “İnternet Programcılığı” dersi kapsamında gerçekleştirilmiştir. Temel hedefimiz, kullanıcıların güncel haberleri okuyabileceği, yönetici paneli sayesinde içeriklerin kolayca eklenip düzenlenebileceği bir sistem oluşturmaktır.

Projemizin Başlıca Özellikleri:
	•	Güncel haberlerin listelenmesi (Teknoloji, Spor, Ekonomi, Sağlık vb.)
	•	Haber detay sayfası ile haber içeriklerinin okunması
	•	Yönetici paneli ile haber ekleme, silme ve düzenleme işlemleri
	•	Kategori bazlı filtreleme
	•	Modern ve mobil uyumlu tasarım
	•	Kullanıcı deneyimi odaklı yapı
Bu proje, Next.js kullanılarak geliştirilmiş bir haber portalı web sitesidir.
Planlama ve Geliştirme Süreci

Proje bireysel olarak yürütülmüştür. Geliştirme süreci aşağıdaki aşamalardan oluşmuştur:
	•	Araştırma ve Planlama: Kullanıcı rolleri, veri modeli ve temel ihtiyaçlar belirlendi.
	•	Kurulum: Next.js, Tailwind CSS, Prisma ve SQLite ile proje iskeleti oluşturuldu.
	•	Veritabanı Tasarımı: 5 ilişkili tablo planlandı ve Prisma ile şeması yazıldı.
	•	Kullanıcı İşlemleri: Kayıt, giriş, profil görüntüleme ve güncelleme modülleri geliştirildi.
	•	Yetkilendirme: Admin ve kullanıcı rolleri belirlendi, middleware ile koruma eklendi.
	•	İçerik Yönetimi: Haber paylaşımı, kategori sistemi ve admin haber onayı eklendi.
	•	Mesajlaşma: Kullanıcılar arası metin mesajlaşma sistemi geliştirildi.
	•	Test ve Hata Ayıklama: İşlevlerin çalışırlığı kontrol edildi, hatalar giderildi.

Modüller ve İşlevleri
Modül	Açıklama
Kullanıcı Yönetimi	Kayıt, giriş, çıkış, profil güncelleme işlemleri
Admin Paneli	Kullanıcıları listeleme, silme, rol değiştirme, haber onayı, kategori yönetimi
Haber Sistemi	Kullanıcıların haber eklemesi, haberlerin admin tarafından onaylanması
Kategori Yönetimi	Admin’in haber kategorilerini tanımlaması
Mesajlaşma	Kullanıcıların birbirine metin mesajı gönderebilmesi

Kodlama Yapısı

Teknolojiler:
	•	Frontend & Backend: Next.js (App Router)
	•	Veritabanı: SQLite
	•	ORM: Prisma
	•	Stil: Tailwind CSS

Klasör Yapısı (Özet):

/app
  /api
    /auth → login, register
    /admin → kullanıcı işlemleri
    /messages → mesajlaşma API
  /profile
  /news
  /categories

/lib
  prisma.ts → Prisma Client

/prisma
  schema.prisma → Veritabanı şeması

/styles
  globals.css

Kazanımlar ve Değerlendirme

Bu projede şunlar öğrenilmiştir:
	•	Next.js App Router yapısı ve API route oluşturma
	•	Prisma ile ilişkisel veritabanı tasarımı ve veri sorgulama
	•	Orta düzey kullanıcı yetkilendirme sistemleri (middleware ile)
	•	CRUD işlemlerinin güvenli ve yapısal biçimde nasıl geliştirileceği
	•	Arayüzde Tailwind CSS ile sade ve tutarlı tasarım geliştirme

Bileşenlerin Genel İşleyişi (Teknik Özet)
	•	Register & Login: bcrypt ile şifrelenmiş kullanıcı kaydı, JWT ile session kontrolü
	•	Middleware: Admin kontrolü için özel middleware yazıldı (isAdmin)
	•	Profil Sayfası: /profile altında kullanıcı bilgileri görüntülenebilir ve güncellenebilir
	•	Admin Paneli: /admin altında kullanıcı yönetimi, haber onayı ve kategori işlemleri yapılabilir
	•	Mesajlaşma: /messages API üzerinden POST/GET istekleriyle mesajlar gönderilir ve görüntülenir
	•	Veritabanı: 5 tablo (User, Profile, Message, News, Category) birbirine ilişkili şekilde tanımlanmıştır.

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
