# Kartify – Dijital Kart Web Sitesi

## Proje Hakkında

Bu projede, dijital kartvizit hizmeti sunan kurgusal bir marka için modern ve responsive bir kurumsal web sitesi tasarladım.

Tasarıma yön verirken verilen referans web sitesinin genel tasarım yaklaşımını, bölüm sıralamasını, kart yapısını, boşluk kullanımını, tipografik hiyerarşisini ve responsive davranışını analiz ettim. Ancak referans sitenin içeriğini ve tasarımını birebir kopyalamak yerine kendi marka adımı, metinlerimi, renklerimi ve kart yapılarımı oluşturdum.

Projenin temel amacı; profesyonel dijital kart kullanımını sade, modern ve anlaşılır bir arayüz üzerinden tanıtmaktır.

---

## Kullanılan Teknolojiler

- HTML5
- CSS3
- CSS Grid
- CSS Flexbox
- CSS Media Queries
- CSS Animations
- CSS Transitions
- HTML `<details>` elementi

Projede Bootstrap, Tailwind veya başka bir hazır CSS framework'ü kullanılmadı.

---

## 1. Tasarımı Ana Bölümlere Nasıl Ayırdım?

Web sitesini aşağıdaki ana bölümlere ayırdım:

### Header / Navbar

Sayfanın üst kısmında marka logosu, navigasyon bağlantıları ve ana aksiyon butonu bulunuyor.

Mobil görünümde navigasyon yapısının kullanılabilir kalması için CSS ve HTML `<details>` yapısını kullandım.

### Hero Bölümü

Kullanıcıya sitenin temel amacını ilk bakışta anlatmak için kullandım.

Bu bölümde:

- Ana başlık
- Açıklama
- İki adet buton
- Özellik kısa bilgileri
- Dijital kart önizlemesi

bulunuyor.

### Dijital Kart Bölümü

Dijital kartın temel özelliklerini dört ayrı kart halinde gösterdim.

Bu bölümde kart yapısını daha anlaşılır hale getirmek için Grid kullandım.

### Nasıl Çalışır

Kullanıcının sistemi nasıl kullanacağını üç adım halinde anlattım:

1. Profilini oluşturma
2. Profilini yayınlama
3. Kartı paylaşma

### Özellikler

Dijital kart sisteminin sunduğu özellikleri ayrı kartlar halinde gösterdim.

Kartların daha hareketli ve modern görünmesi için hover animasyonları kullandım.

### Karşılaştırma

Dijital kartı mobil uygulama ve basılı kart ile karşılaştırdım.

Bu bölüm responsive tasarım açısından özellikle önemlidir.

Masaüstünde dört sütunlu bir yapı kullandım. Mobilde ise sütunları gizlemek yerine her karşılaştırma satırını ayrı bir karta dönüştürdüm.

Bu sayede mobil görünümde içerik azaltılmadı.

### Dijital Kart Nedir?

Dijital kart kavramını açıklayan ayrı bir bölüm oluşturdum.

Ayrıca kullanıcı adı oluşturma alanını bu bölüm içerisinde gösterdim.

### Ücretsiz Araçlar

E-posta imzası, QR kart, toplantı arka planı ve LinkedIn banner gibi yardımcı araçları kart yapısında gösterdim.

### SSS

Sık sorulan sorular bölümünde HTML `<details>` elementi kullandım.

Bu sayede JavaScript kullanmadan soruların açılıp kapanmasını sağladım.

### CTA

Sayfanın sonunda kullanıcıyı dijital kart oluşturmaya yönlendiren güçlü bir çağrı alanı oluşturdum.

### Footer

Footer bölümünü ürün, araçlar ve şirket bağlantıları şeklinde gruplara ayırdım.

---

## 2. Responsive Tasarım Yaklaşımım

Siteyi dört temel ekran genişliğini dikkate alarak tasarladım:

- 1440px masaüstü
- 1024px laptop
- 768px tablet
- 375px mobil

Responsive tasarım sırasında amacım içeriği azaltmak değil, içeriğin yerleşimini değiştirmek oldu.

Örneğin masaüstünde dört sütun halinde gösterilen kartlar mobilde tek sütuna geçiyor.

Böylece kullanıcı mobil cihazda da masaüstünde bulunan bütün içeriği görebiliyor.

---

## 3. En Zor Responsive Bölüm

Projedeki en zor responsive bölüm karşılaştırma alanı oldu.

Masaüstünde dört sütunlu bir karşılaştırma yapısı kullanmak kolay olsa da bu yapı mobil ekranda yatay taşmaya neden olabilirdi.

Bu nedenle mobilde yatay scroll oluşturmak yerine karşılaştırma satırlarını dikey kart yapısına dönüştürdüm.

Örneğin masaüstünde:

| Özellik | Mobil Uygulama | Dijital Kart | Basılı Kart |
|---|---|---|---|

şeklinde gösterilen yapı mobilde her özelliğin kendi kartı olacak şekilde düzenlendi.

Bu yöntemde hiçbir sütunu veya içeriği gizlemedim.

---

## 4. Flexbox Nerelerde Kullanıldı?

Flexbox'ı daha çok tek boyutlu hizalama gereken yerlerde kullandım.

Örneğin:

- Header içerisindeki logo ve navigasyon
- Buton grupları
- Hero altındaki kısa özellik bilgileri
- Footer alt bölümü
- Mobil menü
- Bazı kart içi hizalamalar

Flexbox'ın yatay veya dikey hizalama işlemlerinde daha uygun olduğunu düşündüğüm için bu alanlarda kullandım.

---

## 5. Grid Nerelerde Kullanıldı?

Grid'i daha çok iki boyutlu kart ve bölüm düzenlerinde kullandım.

Örneğin:

- Hero bölümü
- Dijital kart bilgi kartları
- Nasıl çalışır kartları
- Özellik kartları
- Ücretsiz araçlar
- Footer
- Karşılaştırma tablosu

Grid sayesinde sütun sayısını responsive ekranlarda kolayca değiştirebildim.

Örneğin:

```css
grid-template-columns: repeat(4, 1fr);
