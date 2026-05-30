# Web Design Term Project - Technical Specifications & Prompt

Aşağıda belirtilen tüm teknik isterleri %100 karşılayan, modern, temiz, responsive (mobil uyumlu) ve şık bir HTML-based kafe web sitesi şablonu oluşturmanı istiyorum. Proje tamamen statik (HTML/CSS) olacak ve herhangi bir backend sunucu koduna ihtiyaç duymadan çalışacaktır.

---

## ☕ Proje Konsepti: "Venüs Kafe"
Site, estetik ve retro-modern bir çizgisi olan, nitelikli kahve ve tatlı sunan "Venüs" isimli şık bir kafe için tasarlanacaktır. 

### 🎨 Tasarım, Renk Paleti ve Font İsterleri:
- **Renk Paleti:** Venüs konseptine uygun olarak yumuşak krem/fildişi (arka plan), pastel terracotta/pudra pembe (yardımcı renk), venüs altını/sıcak sarı (vurgu renkleri) ve koyu kahve (metin renkleri) tonları kullanılmalıdır. Görsel olarak premium ve sıcak bir atmosfer hissettirmelidir.
- **Font Kombinasyonu:** Başlıklar için zarif ve estetik bir Serif font (Örn: 'Playfair Display' veya 'Georgia'), gövde metinleri için ise okunaklı, modern bir Sans-serif font (Örn: 'Poppins', 'Montserrat' veya 'Arial') tercih edilmeli ve Google Fonts üzerinden projeye bağlanmalıdır.

---

## 1. Genel Proje Yapısı (Dosya Düzeni)
Proje klasörü şu yapıda kurulmalıdır (Toplam 5 HTML sayfası):
- `/index.html` (Anasayfa - Venüs Kafe Tanıtım, Slogan ve Öne Çıkanlar)
- `/about.html` (Hakkımızda - Kafenin Hikayesi ve Ekip Üyeleri)
- `/menu.html` (Menü - Fiyat Listesi ve Kahve/Tatlı Seçenekleri)
- `/media.html` (Multimedya - Kafe Ambiyansı Ses & Video Galeri)
- `/contact.html` (İletişim & Rezervasyon/Geri Bildirim Formu)
- `/css/style.css` (External/Dış CSS dosyası)

---

## 2. Teknik Kodlama İsterleri (Coding Requirements)

### A. Sayfa Şablonu (Template)
- Tüm sayfalarda tutarlı bir Header (Venüs Kafe Logosu ve Navigasyon Menüsü) ve Footer (Çalışma saatleri, adres ve telif hakkı) yapısı olmalıdır.
- Sayfalar arası geçişler (Linkler) eksiksiz çalışmalıdır.

### B. CSS Kullanım Çeşitleri
Ödev puanlaması için CSS'in üç farklı yöntemi de projede yer almalıdır:
1. **External CSS:** Genel site tasarımı, renk paleti, font tanımlamaları ve grid/flexbox düzenleri `/css/style.css` dosyasında olmalıdır.
2. **Internal CSS:** `media.html` sayfasının `<head>` etiketinin içine, sadece o sayfadaki galeri elementlerine özel küçük bir `<style>` bloğu eklenmelidir.
3. **Inline CSS:** `index.html` içinde ana slogan başlığına veya "Rezervasyon Yap" butonuna doğrudan `style="..."` attribute'u ile satır içi bir stil verilmelidir.

### C. Web Form & E-posta Entegrasyonu (Form Submission)
- `contact.html` sayfasında ad, soyad, e-posta, rezervasyon tarihi/konu ve mesaj alanlarını içeren şık bir iletişim formu bulunmalıdır.
- Backend kodu yazmadan e-posta gönderebilmek için formun `action` özniteliği **Formspree** (`https://formspree.io/f/YOUR_FORM_ID`) altyapısına uygun olarak kurulmalıdır. `method="POST"` kullanılmalıdır.

### D. Tablolar (Tables)
- `menu.html` sayfasında en az 3 sütun (Ürün Adı, İçerik/Boyut, Fiyat) ve yeterli sayıda satırdan oluşan, kenarlıkları ve başlıkları Venüs Kafe renk paletine uygun şekillendirilmiş temiz bir HTML `<table>` yapısı bulunmalıdır. Kahveler ve tatlılar bu tablo düzeninde estetik bir biçimde listelenmelidir.

### E. Medya Bileşenleri (Images, Sound, Video)
- **Görseller (Images):** Sayfalarda kahve, tatlı ve mekan estetiğini yansıtan, `alt` etiketleri tanımlanmış yeterli sayıda görsel yer almalıdır.
- **Ses (Sound):** `media.html` sayfasına HTML5 `<audio controls>` etiketi kullanılarak bir "Kafe Ambiyansı / Sakin Fon Müziği" ses dosyası eklenmelidir.
- **Video:** Aynı sayfaya HTML5 `<video controls>` etiketiyle lokal bir kahve demleme videosu veya `<iframe>` kullanılarak gömülü bir YouTube kahve/kafe videosu yerleştirilmelidir.

---

## 3. Senden Beklenenler (Output Request)

Lütfen bu isterlere uygun olarak:
1. Temiz, modern ve semantic (anlamsız `<div>` yığınları yerine `<header>`, `<nav>`, `<main>`, `<section>`, `<footer>` kullanan) HTML kodlarını "Venüs Kafe" içeriğiyle sayfa sayfa üret.
2. Belirtilen estetik renk paletine ve yazı tiplerine sahip, tamamen responsive (mobil uyumlu) bir `style.css` içeriği yaz.
3. Kodların içine hangi isterin nerede karşılandığını belirten HTML/CSS yorum satırları (``) ekle.