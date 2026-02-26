1) **Sisteme Kayıt Olma**  

   **API Metodu:** POST /api/auth/register  

   **Açıklama:** Kullanıcı, e-posta ve şifre bilgilerini girerek sistemde yeni bir kullanıcı profili oluşturur.  


2) **Kullanıcı Girişi Yapma**  

    **API Metodu:** POST /api/auth/login  

    **Açıklama:** Daha önce kayıt olmuş kullanıcılar, e-posta ve şifre bilgileriyle sisteme erişim sağlar.  


3) **Kullanıcı Hesabını Silme**  

   **API Metodu:** DELETE /api/users/profile  

   **Açıklama:** Kullanıcı, dilediği zaman sistemdeki tüm verilerini ve profilini kalıcı olarak sistemden kaldırır.  


4) **Ülke İsmiyle Arama Yapma**  

   **API Metodu:** GET /api/countries/search?name={ulke_adi}  

   **Açıklama:** Kullanıcı, arama çubuğuna bir ülke ismi yazarak o ülkeye ait güncel vize bilgilerini sunucudan çeker.  


5) **Dünya Haritası Üzerinde Görselleştirme**  

   **API Metodu:** GET /api/countries/map-data  

   **Açıklama:** Seçilen pasaportun vize durum verileri veritabanından okunarak harita üzerinde anlamlı renkli bir şekilde sunulur.  


6) **Ülke Karşılaştırması Yapma**  

   **API Metodu:** GET /api/countries/compare?c1={ulke1}&c2={ulke2}  

   **Açıklama:** Kullanıcı, seçtiği iki farklı ülkenin vize güçlerini ve rejimlerini karşılaştırmak için gerekli verileri görüntüler.  


7) **Vize Türüne Göre Filtreleme**  

   **API Metodu:** GET /api/countries/filter?type={vize_turu}  

   **Açıklama:** Kullanıcı; sadece vizesiz, kapıda vize veya e-vize olan ülkeleri listelemek için verileri kriterlere göre süzer.  


8) **Favori Ülkeleri Listeye Ekleme**  

   **API Metodu:** POST /api/favorites  

   **Açıklama:** Kullanıcı, gitmeyi planladığı ülkeleri profilindeki özel listeye yeni bir kayıt olarak ekler.  


9) **Kayıtlı Ülke Notunu Güncelleme**  

   **API Metodu:** PUT /api/favorites/{id}/note  

   **Açıklama:** Kullanıcı, favori listesinde kayıtlı olan bir ülke için daha önce yazdığı hatırlatıcı notları değiştirir.  


10) **Favori Listesinden Ülke Çıkarma**  

    **API Metodu:** DELETE /api/favorites/{id}  

    **Açıklama:** Kullanıcı, artık ilgilenmediği bir ülkeyi kişisel favori listesinden tamamen siler.  


11) **Vize Ücreti ve Döviz Hesaplama**  

    **API Metodu:** GET /api/services/exchange-rates?country={id}  

    **Açıklama:** Kullanıcı, hedef ülkenin güncel vize maliyetlerini ve döviz kuru bilgilerini sistemden okuyarak görüntüler.  


12) **Kullanıcı İstatistiklerini Görüntüleme**  

    **API Metodu:** GET /api/stats/popular  

    **Açıklama:** En çok aranan ülkeler ve popüler rotalar gibi sistem verileri sunulur.  


13) **Ülke Detay ve Görsel Bilgilerini Gösterme**  

    **API Metodu:** GET /api/countries/{id}/details  

    **Açıklama:** Seçilen bir ülkenin pasaport görseli, kalış süresi sınırı ve gerekli temel belgeler veritabanından çekilerek  
     listelenir.

14) **Vize Başvuru Merkezi Konumlarını Listeleme**  

    **API Metodu:** GET /api/services/visa-centers?country={id}  

    **Açıklama:** Kullanıcı, vize alması gereken ülkelerin resmi başvuru merkezlerine ait iletişim ve adres bilgilerini görüntüler.  


15) **Kullanıcı Profil Bilgilerini Güncelleme**  

    **API Metodu:** PUT /api/users/profile  

    **Açıklama:** Kullanıcı, sistemde kayıtlı olan e-posta, şifre veya isim gibi üyelik bilgilerini dilediği zaman günceller.  


