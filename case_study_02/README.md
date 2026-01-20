# Case Study 02 – Elektrik Tüketimi ve Tahsilat Analizi

Bu proje, **YEDAŞ (Yeşilırmak Elektrik Dağıtım A.Ş.)** tarafından sağlanan gerçek tahakkuk ve tahsilat verileri kullanılarak,
ilçe bazlı elektrik tüketim davranışlarının analiz edilmesini, tüketim desenlerinin ortaya çıkarılmasını
ve bu bulgular üzerinden iş önerileri geliştirilmesini amaçlamaktadır.

Çalışma, uçtan uca bir veri analizi süreci olacak şekilde;
veri keşfi, görselleştirme ve veri hikâyesi adımlarını içermektedir.

---

## 📂 Proje Yapısı

```
case_study_02/
├── README.md
├── data/
│   └── elektrik_veri.xlsx
├── processed_data/
├── notebooks/
│   ├── notebook_01_veri_kesfi.ipynb
│   ├── notebook_02_gorsellestirme.ipynb
│   └── notebook_03_veri_hikayesi.ipynb
├── outputs/
│   ├── figures/  
│   └── figures_nb3/            
└── requirements.txt
```

---

## Notebook Açıklamaları

###  notebook_01_veri_kesfi.ipynb
- Bu notebook’ta veri setinin yapısı incelenmiş, eksik ve tutarsız değerler analiz edilerek temel keşifsel veri analizi gerçekleştirilmiştir.

###  notebook_02_gorsellestirme.ipynb
- İlçe bazlı tüketim ve tahsilat karşılaştırmaları ile mevsimsel ve segment bazlı tüketim eğilimleri görselleştirilmiştir.

###  notebook_03_veri_hikayesi.ipynb
- Analiz sonuçları veri hikayesi yaklaşımıyla yorumlanmış, müşteri segmentasyonu yapılmış, tahsilat riks analizleri gerçekleştirilmiş ve bulgulara dayalı stratejik iş önerileri geliştirilmiştir.

---


## Environment

Proje **Python 3.13** ortamında geliştirilmiştir.

Kullanılan temel kütüphaneler:
- pandas  
- numpy  
- matplotlib  
- seaborn  
- openpyxl  

Projeyi farklı ortamlarda çalıştırabilmek için gerekli minimum sürümler
`requirements.txt` dosyasında belirtilmiştir.

---

## Kurulum ve Çalıştırma

Gerekli kütüphaneleri kurmak için:

```bash
pip install -r requirements.txt
```

Notebook’ları çalıştırmak için:

```bash
jupyter notebook
```

---
### Hazırlayan

**Mehmet Enes Temel**  
Bilgisayar Mühendisi
