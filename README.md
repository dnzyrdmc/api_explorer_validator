# ⬡ API Explorer & Validator

Bu araç, geliştiricilerin ve veri analistlerinin bilinmeyen bir API'den gelen veriyi, kendi projelerine dahil etmeden önce **güvenli ve şeffaf** bir şekilde incelemelerini sağlayan hafif bir "kum havuzu" (sandbox) çözümüdür. Geliştirme aşamasında claude ve gemini tarafından yardım alınmıştır.

## Neden Kullanmalıyım?

Bir API'yi sisteminize bağlamadan önce şu sorulara yanıt bulmanızı sağlar:

* **Veri İçinde Ne Var?** Karmaşık ve iç içe geçmiş (nested) JSON yapılarını düzleştirerek okunabilir, düzenli tablolara dönüştürür.
* **Gizli Tehlike Var mı?** Beklenmedik alanları, anormal veri tiplerini veya zararlı olabilecek içerikleri önceden tespit etmenizi sağlar.
* **Bilgisayarım Güvende mi?** Veriyi kodunuzun içinde değil, izole bir arayüzde çalıştırarak sistem güvenliğinizi korur.
* **Yapı Analizi:** API'nin döndürdüğü veri tiplerini (boolean, string, number) anında analiz ederek dökümantasyon tutarlılığını kontrol eder.

## Temel Özellikler

* ** CORS Bypass (Proxy):** Tarayıcıların güvenlik engellerine takılmadan herhangi bir online URL'den veri çekebilir.
* ** Auto-Flatten:** Derin derin objeleri (Örn: `user.profile.meta.id`) otomatik olarak düzleştirir ve sütunlara ayırır.
* ** Dinamik Filtreleme:** Saniyeler içinde binlerce satır veri arasında anlık arama yapmanıza olanak tanır.
* ** Sıfır Kurulum:** Tek bir HTML dosyasıdır; veritabanı, sunucu veya `npm install` gerektirmez.

##  Nasıl Çalıştırılır?

1.  `index.html` dosyasını indirin.
2.  Dosyayı herhangi bir modern tarayıcıda (Chrome, Firefox, Edge) çift tıklayarak açın.
3.  **URL'den Getir** kısmına API adresini yazın veya **JSON Yapıştır** kısmına ham verinizi ekleyin.
4.  Eğer online bir URL'den veri gelmiyorsa (CORS hatası), **"Proxy ile Çek"** butonunu kullanın.

##  Test İçin Örnek API'ler

Hızlıca denemek için aşağıdaki popüler test adreslerini kopyalayabilirsiniz:
* `https://dummyjson.com/products`
* `https://jsonplaceholder.typicode.com/users`
* `https://fakestoreapi.com/products`

---

> **  ÖNEMLİ NOT:** Bu proje tamamen **istemci taraflı (client-side)** çalışır. Çektiğiniz veya yapıştırdığınız veriler hiçbir sunucuya gönderilmez veya kaydedilmez. Her şey sadece tarayıcınızın belleğinde gerçekleşir.

---
