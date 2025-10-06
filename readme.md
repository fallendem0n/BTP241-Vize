### I. Ağlara Giriş ve Temel Kavramlar

#### 1. Ağ Kavramı ve Yararları

Bir bilgisayar ağı, bilgi ve kaynak paylaşımını sağlamak amacıyla **iki veya daha fazla bilgisayarın bir iletişim kanalı üzerinden birbirine bağlanmasıdır.**

* **Ağın Olumlu Yanları (Soru 2 ile ilişkili):**
    * **Bağlanabilirlik ve İletişim:** Kullanıcılar ve aygıtlar arasında veri alışverişi.
    * **Veri Paylaşımı:** Merkezi depolama ve erişim kolaylığı.
    * **Donanım Paylaşımı:** Yazıcı, tarayıcı gibi pahalı çevre birimlerinin ortak kullanımı.
    * **İnternet Erişimi ve Paylaştırılması.**
    * **Veri Güvenliği ve Yönetimi:** Merkezi kontrol.
    * **Başarımda İyileştirme ve Yük Dengeleme.**

* **Sunucu - İstemci Mimarisi Yararları (Soru 1):**
    * **Bağlanılabilirlik ve iletişim tek bir kaynak üzerinden dağıtılabilir.**
    * Veri güvenliğinin sağlanması daha kolaydır.
    * Başarım iyileştirmesi ve yük dengeleme yapılması daha kolaylıkla gerçekleştirilir.

#### 2. Protokol Kavramı

* **Protokol (Soru 4):** Bilgisayar ağları için protokol, **ağdaki aygıtlar arasındaki iletişimi ve etkileşimi düzenleyen kurallar kümesidir.** Protokoller, haberleşmenin nasıl başlayacağını, verinin nasıl paketleneceğini, iletileceğini ve sonlandırılacağını tanımlar.

#### 3. Ağ Mimarisi (Soru 3)

* **Ağ Mimarisi:** Mimari, **donanım ve yazılımın birlikte çalışması ile ortaya çıkan katmanlardan oluşan bir yapıyı ve yapının işleyişini düzenleyen kulların tanımlanmasıdır.** (Örn: OSI Modeli, TCP/IP Modeli).

### II. Ağların Karakteristik Özellikleri ve İletişim Yöntemleri

#### 1. İletişim Türleri ve Bağlantı Yapısı

* **Unicast Haberleşme (Soru 8):** Aynı ağ üzerinde bulunan iki bilgisayar arasında gerçekleşen, **kaynaktan tek bir hedefe** yönelik haberleşmedir. (Point-to-Point)
* **Multicast Haberleşme:** Kaynaktan **bir gruba** ait tüm hedeflere yönelik haberleşmedir.
* **Broadcast Haberleşme:** Kaynaktan **ağdaki tüm cihazlara** yönelik haberleşmedir.

#### 2. Anahtarlama Yöntemleri

* **Devre Anahtarlama (Soru 5):**
    * İki uç arasında iletişimin sağlanabilmesi için iletişimin gerçekleşmesini sağlayan **bir bağlantının önceden kurulmuş olması zorunludur.**
    * Kurulan bu bağlantı, iletişim süresince **sadece o iki uç tarafından kullanılır** ve başkası kullanamaz.
    * Örnek: Geleneksel telefon hatları.

* **Paket Anahtarlama:**
    * Veri haberleşmesi için **önceden bir bağlantının kurulması gerekli değildir.**
    * İletilecek olan veri, **paket adı verilen küçük parçalara ayrılıp** ağ üzerinden hedefine gönderilir.
    * Paketler farklı bağlantılar üzerinden iletilebilir. Varış noktasında ise paketler yeniden birleştirilip mesajın ilk şekli elde edilir.

#### 3. Bağlantılı ve Bağlantısız Protokoller

* **Bağlantılı İletişim Protokolleri (Connection-Oriented) (Soru 6):**
    * İletişimin başlaması için öncelikle **mantıksal bir bağlantının kurulmuş olması gerekir.**
    * Paketlerin **doğru sırada** ve **hatasız** iletilmesini garanti eder.
    * Örnek: **TCP** (Transmission Control Protocol).

* **Bağlantısız İletişim Protokolleri (Connectionless):**
    * Bağlantı kurulması gerekmez; paketler doğrudan hedefe gönderilir.
    * Hata veya sıra garantisi yoktur, daha hızlıdır.
    * Örnek: UDP (User Datagram Protocol), IP (Internet Protocol).

### III. Performans, Mesaj Biçimi ve Kalite

#### 1. Ağ Performansına Etki Eden Etkenler (Soru 9)

Ağ performansına doğrudan etki eden üç ana faktör şunlardır:

1.  **Hız.**
2.  **Bant Genişliği (Bandwidth).**
3.  **Gecikme (Latency).**

#### 2. Bant Genişliği (Soru 10)

* **Bant Genişliği (Bandwidth):** **Bir veri ileten ortamın veya bir bilgisayar ağının veri iletim kapasitesini tanımlayan bir kavramdır.** Genellikle saniyedeki bit (bps) cinsinden ifade edilir.

#### 3. Mesajlar ve Veri Birimleri

* **SDU (Service Data Unit) (Soru 7):** Bir alt katmanda çalışan protokolün, **üst katmanda çalışan protokole gönderdiği mesajın adıdır.**
* **Mesaj Biçimlendirme:** Ağdaki mesajlar, iletişim katmanlarına göre farklı isimler alır (PDU). Temelde 3 kısımdan oluşur:
    * **Başlık (Header):** Kontrol bilgileri.
    * **Gövde (Payload):** Asıl veri.
    * **Son (Trailer):** Hata kontrol bilgileri (Örn: Çerçeve Kontrol Dizisi - FCS).
* **Veri Birimi İsimleri:**
    * **Paket:** Ağ Katmanı (Network Layer) veri birimi.
    * **Çerçeve:** Veri Bağlantı Katmanı (Data Link Layer) veri birimi.
    * **Datagram:** Bağlantısız protokollerin (Örn: IP/UDP) kullandığı veri birimi.
    * **Hücre:** ATM gibi ağlarda kullanılan sabit boyutlu veri birimi.
