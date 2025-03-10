# Reportlab-projects

Bu proje, ReportLab kütüphanesini kullanarak sertifikalar ve yaka kartları oluşturan iki farklı Jupyter Notebook dosyasını içerir.

## 📌 İçindekiler
- `createCertificate.ipynb`: Excel'deki katılımcı listesinden isimleri alarak sertifika PDF'leri oluşturur.
- `createBadge.ipynb`: Katılımcılar için QR kod içeren yaka kartları oluşturur.
- `requirements.txt`: Proje için gerekli Python kütüphanelerini içerir.

## ⚙️ Kurulum
Projeyi çalıştırmadan önce aşağıdaki bağımlılıkları yükleyin:

```bash
pip install -r requirements.txt
```

## 📜 Kullanım

### 1. Sertifika Oluşturma (`createCertificate.ipynb`)
Bu notebook, `certificate.xlsx` dosyasındaki isimleri alarak `Certificate.pdf` şablonu üzerine yazdırır ve çıktı olarak `sertifikalar.pdf` dosyasını üretir.

**Süreç:**
- Excel dosyasından katılımcı bilgileri okunur.
- ReportLab ile her katılımcının adı, soyadı ve diğer bilgileri sertifika şablonuna eklenir.
- Hazırlanan sertifikalar tek bir PDF dosyasında birleştirilerek `sertifikalar.pdf` olarak kaydedilir.


### 2. Yaka Kartı Oluşturma (`createBadge.ipynb`)
Bu notebook, `Badge_list.xlsx` dosyasındaki bilgilerle QR kodlar üreterek `Badge.pdf` şablonu üzerine ekler ve `badge_created.pdf` dosyasını oluşturur.

**Süreç:**
- Excel dosyasından katılımcı bilgileri (Ad, Soyad, Kurum, Katılımcı Türü vb.) okunur.
- Katılımcı bilgileri kullanılarak bir QR kod oluşturulur.
- QR kod ve katılımcının temel bilgileri yaka kartı şablonuna yerleştirilir.
- Tüm yaka kartları birleştirilerek `badge_created.pdf` adlı dosya oluşturulur.




