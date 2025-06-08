# Yeni Nesil Bankacılık Simulasyonu
## İş Bankası - LUDİ

  İş Bankası'nın yeni nesil bankacılık simulasyon programı Ludi'de yer alana görevlerin yapımında kullandığım veri ve kodları içerir. Proje içerisinde kampanya üretme, müşteri listesi oluşturma ve kredi tahsisi simülasyonunu tarzında programında uygulamalı sunmuştur.

  ### **1. Pazarlama Bölümü**

     
-Uzman yardımcısı olarak bu bölümün ilk kısmında kampanyaların ve yapılan uygulamaların değerlendirilmesi istendi. Sunuma eklenicek bir sayfa üzerinden raporlamanın gösterilmesi beklendi. ✔


-Sonraki kısımda ise excel dosyasındaki müşteri bilgileri ile harcama bilgileri dosylarının incelenerek yeni bir kampanya için ulaşılabilicek yeni müşteri sayısına erişilmesi ve bunun analiz edilmesi istendi. ✔ 

Bu kısımda dosyları python üzerinden pandas library kullanarak yeni dosyalar kısmında klasife ettim ve filtreledim. Bunun üzerine çözümümü sundum. Ancak bu çözüm kısmında hatalı olduğum kısmı ise bu ortaklaşa yapmaya çalıştığım müşteri bulma kısmında filtrelerim çok keskin olduğundan elimde kalan kümede sayı olarak az bir topluluğa eriştiğimi gördüm.
 

### **2. Kredi Tahsisi**

-Tahsis Tutarına Göre Değişen Yetkili Döngüsü

Şube yetkisi->Bölge yetkisi->Genel müdürlükteki X Bölümü (Kobi Bankacılığı Bölümü ya da Ticari Krediler Bölümü)->Genel müdürlükteki Kurumsal Krediler Bölümü->Yönetim Kurulu

-ACME A.Ş istihbarat rapor (İstihbarat çalışmaları ekran istihbaratı ve piyasa istihbaratı olarak iki başlık altında toplanır).

-Kredi nosyonu: getiri çıkar

-Mali analiz çalışması—Bilanço, Gelir tablosu, Likidite, Rasyolar mail—en önemlisi ilk 2. İncelendi ve mail hazırlandı. Excelden işlemler yaparken ortalama konusunda hata yapıldı onun dışında bir sorun yaşanmadı.

-Mailde Nakit Dönüşüm Döngüsü (NDD) Tespitleri, Genel Likidite Yorumu, Karlılık Performansı


* Cari Oran: Dönen varlıkların (nakit, stok, alacak) / Kısa vadeli borçlar. >1.5 idealdir.

* FAVÖK: Şirketin ana faaliyetlerden elde ettiği brüt kâr. Borç yapısı/vergi politikasından bağımsız performansı gösterir.

* NDD: Paranızın "stok → satış → tahsilat → tedarikçi ödeme" döngüsündeki süre. Ne kadar kısa, o kadar iyi.


-Son görevde kredinin teminat koşulları ile bir çalışma yapıldı. 


### **3. Dijital Bankacılık**

-İş Bankası İçCep Hayatım üzerine yeni bir başlık yaratıldı ve özellikler kısmı tasarlandı. 

-5 farklı iş parçası için bir önceliklendirme yapıldı.

* Sanal POS Terminallerinde SKT Kontrolünün Kaldırılması
* Kart Şeması- Processing Integrity Programı Uyum
* Sanal POS’ta ApplePay Desteği Kurulması
* Sanal POS’ta Terminal Bazlı Tekil İşlem Limit Kırılımlarının Arttırılması
* Linkle Tahsilat Eposta Başlığı ve İçerik Düzenlemesi 

Yasal zorunluluklar öncelik verilmiştir. Doğrudan karlılık (ücret optimizasyonu, ApplePay gelir artışı) devamında gelip dolaylı etkiler sona alınmıştır.


### **4. Ödeme Sistemi**

-Pandas ve matplotlib kullanarak Excel dosyasındaki verileri analiz ederek "Issuer Ülke Kodu" ve "Döviz Kodu" bazında işlem hacimlerini inceledim. Özellikle USD cinsinden toplam tutarları dikkate aldım.

-En yüksek hacimli ülke-döviz kombinasyonlarını belirlemek için gruplama yaptım (örneğin, SE-RUB, ZA-JPY gibi).

-Avrupa ülkeleri (DE, GB gibi) ve ZA için alternatif ödeme yöntemlerine yönelik araştırma yaptım, mevcut pazar dinamiklerini ve ödeme tercihlerini değerlendirdim. Dağılım grafikleriyle birlikte yürütüldü.

-Avrupa pazarına odaklanıldı.





