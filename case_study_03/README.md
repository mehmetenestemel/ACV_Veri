# YEDAŞ – Enerji Tüketim Verilerinde Anomali Analizi

## Proje Amacı
Bu proje, YEDAŞ’a ait gerçek elektrik tüketim verileri üzerinden **kaçak kullanım, sayaç hatası ve şebeke problemlerini** tespit etmek ve **yönetim ile saha ekipleri için karar destek sağlayan bir Power BI dashboard’u** oluşturmak amacıyla hazırlanmıştır.

---

## Kullanılan Veri
Çalışmada aşağıdaki bilgileri içeren tüketim verileri kullanılmıştır:
- Aktif ve reaktif tüketim değerleri
- Faz bazlı akım ve gerilim ölçümleri
- Abone grubu, il ve ilçe bilgileri
- Sayaç marka ve model bilgileri
- Tarih ve saat bilgileri

---

## Veri Hazırlama (Power Query)
Power Query aşamasında aşağıdaki işlemler gerçekleştirilmiştir:
- Eksik (null) değerlerin tespiti ve flag’lenmesi
- Negatif ve sıfır tüketim kayıtlarının kontrolü
- Tarih alanından gün, ay, gün adı, mesai / mesai dışı ve gece / gündüz kırılımlarının türetilmesi
- Fazlardan birinin sürekli sıfır olduğu durumların belirlenmesi
- Gerilim verisi olmadan devam eden tüketimlerin tespiti
- Uzun süre sabit tüketim gösteren tesisatların işaretlenmesi

---

## Anomali ve Risk Yaklaşımı
Analizlerde her abone;
- Kendi abone grubu
- Kendi il / ilçe ortalamaları

ile karşılaştırılarak değerlendirilmiştir.

Kullanılan başlıca risk kriterleri:
- Akım ve gerilim sapmaları
- Faz dengesizliği
- Gece saatlerinde olağandışı tüketim
- Uzun süre sabit tüketim
- Yüksek reaktif – düşük aktif tüketim
- Gerilim verisi eksikken devam eden tüketim

Bu kriterler birleştirilerek aboneler **Normal / Orta Risk / Yüksek Risk** olarak sınıflandırılmıştır.

---

## Dashboard İçeriği

- İl / ilçe bazında anomali sayısı ve dağılımı
- Abone grubu ve sayaç özelliklerine göre risk profili
- Gün bazlı anomali frekans analizi
- En çok anomali üreten ilk 10 tesisat
- Tesisat bazında risk türleri
---

![Dashboard Genel Bakış](dashboard.png)
