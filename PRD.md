**Product Requirements Document (PRD)**

**Project Title:** Personal Portfolio Website

**Owner:** Bilgisayar Mühendisliği Öğrencisi (Ad Soyad girilecek)

**Purpose:**
Bu proje, kullanıcının yazılım projelerini, deneyimlerini, kendisi hakkındaki bilgileri sergileyeceği modern, şık ve interaktif bir portfolio sitesi oluşturmayı amaçlamaktadır.

***Teknolojiler ve Uygulama Alanları***

|Özellik | Kullanılacak Teknoloji|
|---|---|
| UI oluşturma | React |
|Stil (responsive & theme) | Tailwind CSS |
|Scroll ve hover animasyonlar | Framer Motion |
|Proje başlangıç ve geliştirme ortamı | Vite|
|E-posta ile iletişim formu | EmailJS|
|Ziyaretçi sayacı | IP tabanlı sayaç (örnek JS snippet) |
|Proje filtreleme | React state + Tailwind + JS |
|Light/Dark tema değişimi | Tailwind theme toggle + React state |
|PDF indirme | HTML  tag + static file |
|Logo animasyonu (loading) | CSS / React + SVG |

---

### 1. Genel Bilgiler

- **Dil:** Yalnızca İngilizce
- **Yapı:** Tek sayfa (Single Page Application)
- **Tema:** Dark / Light mode destekli
- **Blog:** Bu sitede yok, ayrı bir platform olacak
- **Admin Panel:** İlk etapta yok, sonradan eklenebilir yapıda olacak

---

### 2. Sayfa Bölümleri

#### 1. Navbar

- Sabit üst menü
- Scroll ile sayfa içi yumuşak geçiş
- Bölümler:
  - About
  - Experience
  - Work
  - Contact
- Resume butonu: Hover'da animasyon, PDF indirme

#### 2. Hero

- "Hi, my name is ..."
- Mesleki tanıtım cümlesi
- Sosyal medya ikonları (GitHub, LinkedIn, vs.)
- Call-to-action butonu

#### 3. About

- Kendini tanıttığı bir metin
- Teknoloji listesi (stack)
- Profil fotoğrafı: Hover ile renk/animasyon efekti

#### 4. Experience

- Solda şirket listesi (buton gibi)
- Sağda şirkete ait detaylar dinamik olarak değişir

#### 5. Featured Projects

- 2-3 proje, büyük görselli kart
- Hover'da görsel filtresi kalkar
- Proje açıklaması + tech stack + GitHub & Live demo linki

#### 6. Other Projects

- 6'li kutu yapısı, hover efektli
- "Show More" ile toplamda 15 projeye kadar görünür

#### 7. Project Archive

- "View archive" linkiyle ulaşılır
- Yıl | Proje Başlığı | Şirket (varsa) | Tech stack | Linkler

#### 8. Contact

- "Get in touch" mesajı
- Mail adresi ve/veya iletişim formu (opsiyonel)

---

### 3. UI/UX Özellikleri

- Dark/Light toggle
- Scroll animasyonları (Framer Motion):
  - Fade in, Slide in, Zoom, Staggered
- Hover efektleri (button, resim, link)
- Responsive tasarım (mobil uyumlu)
- Loading screen (logo animasyonu: altıgen içinde harf)

---

### 4. Ekstra Fonksiyonlar

- Ziyaretçi sayaç (anonim IP-based)
- Dinamik proje filtreleme (teknolojiye göre)
- CV PDF indirilebilir olacak
- İki yanda sabit bilgi:
  - Sol: Sosyal medya ikonları
  - Sağ: E-posta bilgisi


### 5. Kullanılacak Teknolojiler

- **React**: UI komponentleri oluşturmak için
- **Tailwind CSS**: Hızlı ve esnek stil tanımları için
- **Framer Motion**: Animasyon efektleri için
- **Vite**: Proje başlatma ve geliştirme sunucusu
- **EmailJS**: İletişim formu için e-posta gönderimi
- **Github Page**: Yayınlama ve barındırma
- **GitHub**: Versiyon kontrol ve kaynak kod barındırma

---
### 6. Klasör yapısı

/portfolio-site
├── public/
│   ├── index.html
│   └── resume.pdf           # İndirilebilir CV
│
├── src/
│   ├── assets/              # Resimler, SVG'ler, logo vs.
│   ├── components/          # Tüm UI bileşenleri
│   │   ├── Navbar.jsx
│   │   ├── Hero.jsx
│   │   ├── About.jsx
│   │   ├── Experience.jsx
│   │   ├── FeaturedProjects.jsx
│   │   ├── OtherProjects.jsx
│   │   ├── ProjectArchive.jsx
│   │   ├── Contact.jsx
│   │   └── ThemeToggle.jsx
│   │
│   ├── constants/           # Proje verileri (JSON yapılar)
│   │   ├── experiences.js
│   │   ├── projects.js
│   │   └── archive.js
│   │
│   ├── hooks/               # Özel hook'lar (örnek: useDarkMode.js)
│   ├── utils/               # Yardımcı fonksiyonlar (örnek: visitorCounter.js)
│   ├── styles/              # Tailwind, animasyon, özel stiller
│   │   └── globals.css
│   │
│   ├── App.jsx              # Ana uygulama bileşeni
│   ├── main.jsx             # Vite giriş noktası
│   └── config.js            # EmailJS ve diğer sabit ayarlar
│
├── .gitignore
├── package.json
├── tailwind.config.js
├── postcss.config.js
├── README.md


### 9. Yapılacaklar Listesi (To-Do)

- [ ] Logo tasarımı (altıgen içi harf)
- [ ] Proje klasör yapısının oluşturulması (React + Vite)
- [ ] Navbar component'inin yazılması
- [ ] Hero bölümü geliştirme
- [ ] Dark/Light mode toggle oluşturulması
- [ ] Hakkında (About) bölümü yazımı ve profil resmi eklenmesi
- [ ] Experience bölümü için sol menü ve içerik geçişleri
- [ ] Öne çıkan projeler (Featured) bölümü hazırlanması
- [ ] Other Projects grid yapısının kurulması
- [ ] Proje arşivi tablosunun hazırlanması
- [ ] İletişim formu ve e-mail entegrasyonu (EmailJS)
- [ ] Scroll animasyonlarının eklenmesi (Framer Motion)
- [ ] Dinamik filtreleme sisteminin oluşturulması
- [ ] Ziyaretçi sayaç entegrasyonu
- [ ] Resume butonuna PDF bağlantısının eklenmesi

---

### 10. Tamamlanan Görevler

---

**Not:** admin paneli ile genişletilebilecek şekilde kodlanacaktır.
