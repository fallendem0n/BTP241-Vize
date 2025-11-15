# btp2.4.1_h4ndshake.sme

---
## Kullanıcı Sözleşmesi
** Bu sayfaya erişen herkes şartları okuyup kabul etmiş sayılır.
** Vizeden 80 aşağısı almanız takdirde sınıfa ilk derste tatlı almanız zorunludur.
** Aşağıdaki sayfayı öğrenip ezberlemenize rağmen bu sorular çıkmazsa tazminat olarak herkese yemek ısmarlayacağım. Tazminat ödemeleri için hkurtogluirl@gmail.com adresinden iletişime geçebilirsiniz.


### 1. Sunucu-İstemci Mimarisi
| Soru | Cevap |
| :--- | :--- |
| **Sunucu – istemci mimarisinin sağladığı yarar nedir?** | Bağlanılabilirlik ve iletişim tek bir kaynak üzerinden dağıtılabilir. İnternet erişimi sağlanır ve paylaştırılabilir. Veri güvenliğinin sağlanması daha kolaydır. Başarım iyileştirilmesi yapılabilir ve yük denegeleme daha kolaylıkla gerçekleştirilir. Ağın büyüklüğüne bağlı olarak maliyet avantajı sağlayabilir. |
| **Eşler arası ağın sağladığı yararlar nelerdir?** | Ağı oluşturan bilgisayarların tümü hem sunucu hem de istemci rolünü üstlenebilir. Verilerin paylaşılmasını kolaylaştırır. Maliyeti görece olarak azdır. |

---

### 2. Bilgisayar Ağlarının Genel Etkileri
| Soru | Cevap |
| :--- | :--- |
| **Bir bilgisayar ağının sağladığı yararlar nelerdir?** | Bağlanabilirlik ve iletişim, veri paylaşımı, donanım paylaşımı, internet erişimi ve paylaştırılması, veri güvenliği ve yönetimi, başarımda iyileştirme ve yük dengeleme, eğlence. |
| **Bir bilgisayar ağının olumsuz yanları nelerdir?** | Ağ donanımı, yazılımı ve kurulum maliyetleri, donanım, yazılım yönetim ve işletim maliyetleri, istenmeyen paylaşımlar, veri güvenliğinin sağlanması. |

---

### 3. Mimari ve Modeller
| Soru | Cevap |
| :--- | :--- |
| **Ağ mimarisi kavramını açıklayınız.** | Mimari, donanım ve yazılımın birlikte çalışması ile ortaya çıkan katmanlardan oluşan bir yapıyı ve yapının işleyişini düzenleyen kuralların tanımlanmasıdır. |
| **Ağ modeli kavramını açıklayınız.** | Bir model ağdaki katmanları, katmanların görevlerini ve aralarındaki etkileşimin nasıl gerçekleştiğini tanımlar. Tüm taraflar tarafından üzerinde uzlaşılmış olan bir model hem donanım hem de yazılımın beklendiği gibi çalışmasını sağlar. |

---

### 4. Protokol Kavramı
| Soru | Cevap |
| :--- | :--- |
| **Bilgisayar ağları için protokol kavramını açıklayınız.** | Bilgisayar ağları için protokol, ağdaki aygıtlar arasındaki iletişimi ve etkileşimi düzenleyen kurallar kümesidir. |
| **Bilgisayar ağlarında protokolün görevi nedir?** | Bilgisayar ağlarında ise protokol, tüm aygıtların ağ haberleşmesi süresince çeşitli eylemleri nasıl yürüteceklerini belirtir. |

---

### 5. Anahtarlama Mekanizmaları
| Soru | Cevap |
| :--- | :--- |
| **Devre anahtarlama nasıl işler?** | İki uç arasında iletişimin sağlanabilmesi için iletişim gerçekleşmesini sağlayan bir bağlantının (devre) kurulmuş olması zorunludur. İletişimin sürdüğü süre boyunca devre bu iki uç arasındaki veri iletişimini yürütür. Bir ağ üzerinde birçok iletişim hattı bulunmasına karşılık, devre anahtarlamada iletişim kuran iki uç için sadece bir bağlantı kullanılır. |
| **Paket anahtarlama nasıl işler?** | Bu ağlarda veri haberleşmesi için önceden bir bağlantının kurulması gerekli değildir. Bunun yerine iletilecek veri, **paket** adı verilen küçük parçalara ayrılıp ağ üzerinden hedefine gönderilir. Paketler varış noktasında yeniden birleştirilip mesajın ilk şekli elde edilir. |

### 6. Bağlantı Gereksinimi (TCP/IP)
| Soru | Cevap |
| :--- | :--- |
| **Hangi TCP/IP protokolü mantıksal bir bağlantı kurulmuş olmasını gerektirmez?** | **IP**, **UDP** |
| **Hangi TCP/IP protokolü mantıksal bir bağlantı kurulmuş olmasını gerektirir?** | **TCP** |

---

### 7. Katmanlar Arası Mesajlaşma
| Soru | Cevap |
| :--- | :--- |
| **Aynı katmanda çalışan protokoller arasında alınan ve gönderilen mesajlara ne denir?** | Bir **PDU** (Protokol Veri Birimi) aynı katmanda çalışan iki protokol arasındaki gönderilen ve alınan mesajın adıdır. |
| **Alt katmanda çalışan bir protokolün üst katmanda çalışan bir protokole gönderdiği mesajlara ne denir?** | **SDU** (Hizmet Veri Birimi) bir alt katmandaki protokolün bir üst katmana gönderdiği mesajın adıdır. |

---

### 8. İletişim Şekli
| Soru | Cevap |
| :--- | :--- |
| **Aynı ağ üzerinde bulunan iki bilgisayar arasında gerçekleşen haberleşme hangi tür haberleşmedir?** | **UNICAST** haberleşmedir. |

---

### 9. Performans Etkenleri
| Soru | Cevap |
| :--- | :--- |
| **Aşağıda verilen etkenlerden hangisi ağ performansına etki eder?** | Hız, bant genişliği, gecikme. |
| **Aşağıda verilen etkenlerden hangisi ağ performansına etki etmez?** | Tasarım ve kurulum maliyeti, kalite, standartlar, genişletilebilirlik ve güncellenebilirlik, yönetim ve bakım kolaylığı. |

---

### 10. Hız Kavramları
| Soru | Cevap |
| :--- | :--- |
| **İtibari hız (rated) kavramı nedir?** | İtibari hız, bir ağ donanımının erişebileceği teorik hız değeridir. |
| **Bant genişliği (bandwidth) kavramı nedir?** | Bir veri ileten ortamın veya bir bilgisayar ağının veri iletim kapasitesini tanımlayan bir terimdir. Bir noktadan birim zamanda taşınabilecek olan verinin miktarıdır. |
