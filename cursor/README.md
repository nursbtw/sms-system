# SMS Gönderim Sistemi

Web tabanlı SMS gönderim sistemi. Excel veya TXT dosyasından toplu numara yükleme ve manuel numara girişi destekler.

## 📱 Sistem Özellikleri

- Excel veya TXT dosyasından toplu numara yükleme
- Manuel numara girişi
- Gerçek zamanlı SMS durum takibi
- Geçersiz numara kontrolü
- Karakter sayısı kontrolü
- Otomatik numara formatı düzeltme

## 🌐 Kullanım

1. [SITE_URL] adresine gidin
2. SMS göndermek için:
   - Mesaj metnini girin
   - Telefon numaralarını manuel olarak girin veya dosya yükleyin
   - Gönder butonuna tıklayın
   - Gönderim durumlarını takip edin

## 📄 Dosya Formatları

### TXT Dosyası
Her satıra bir numara yazın:
```
05051234567
5051234567
+905051234567
```

### Excel Dosyası
- İlk sütuna numaraları yazın
- İlk satıra "Telefon" yazabilirsiniz (opsiyonel)

## ☎️ Desteklenen Numara Formatları

- 05051234567
- 5051234567
- +905051234567
- 905051234567

## ❗ Önemli Notlar

- Geçersiz numaralar otomatik tespit edilir ve ayrı bir tabloda gösterilir
- Uzun mesajlar birden fazla SMS olarak gönderilir
- Gönderim durumları otomatik güncellenir

## 🔒 Güvenlik

- Numaralarınız ve mesajlarınız güvenli bir şekilde işlenir
- Verileriniz üçüncü taraflarla paylaşılmaz

## 🆘 Destek

Sorun yaşarsanız:
- [DESTEK_EMAIL] adresine mail atın
- [TELEFON] numarasını arayın

## Kurulum

1. Python'u yükleyin (3.8 veya üzeri)
2. Projeyi indirin:
```bash
git clone [REPO_URL]
cd sms-sender
```

3. Sanal ortam oluşturun ve aktif edin:
```bash
python -m venv venv
# Windows için:
venv\Scripts\activate
# Linux/Mac için:
source venv/bin/activate
```

4. Gerekli paketleri yükleyin:
```bash
pip install -r requirements.txt
```

5. config.py dosyasını oluşturun ve API bilgilerinizi girin:
```python
SMS_API_CONFIG = {
    'API_URL': 'https://yurticisms1.com/sms_api',
    'USERNAME': 'KULLANICI_ADINIZ',
    'PASSWORD': 'SIFRENIZ',
    'DATACODING': 'turkish'
}
```

## Hata Durumları

- Geçersiz numara formatları otomatik tespit edilir
- Hatalı numaralar ayrı bir tabloda gösterilir
- API hataları kullanıcıya bildirilir

## Bakım ve Güncelleme

Güncellemeler için:
```bash
git pull
pip install -r requirements.txt
```

## Lisans

Bu proje [LİSANS_ADI] lisansı ile lisanslanmıştır. 