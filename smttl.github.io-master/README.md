
# Bağıl sistem not aralığı hesaplayıcı


# Kesin CC Hesaplayıcı
Bu proje, derslerde kullanılan T-score tabanlı not hesaplama sistemine göre, en düşük CC (geçme notunu) kolayca ve yüksek doğrulukla hesaplayabileceği bir web uygulamasıdır.

# 🚀 Proje Özellikleri
Kullanıcıdan:

Ders Adı

T-score değeri

Öğrencinin ortalaması

Sınıf ortalaması
bilgilerini alır.

Girilen bilgilere göre:

Standart sapmayı (SS) hesaplar.

En düşük CC (geçme notu) değerini belirler.

Not aralıklarını (AA, BA, BB, CB, CC, DC, FF) tablo şeklinde gösterir.

# 🧮 Hesaplama Mantığı
Yönetmelikte verilen formülde tscore değeri ve ortalama ve sınıf ortalamasından standart sapmayı buluyoruz 
Yönetmelikte verilen tscore hesaplama formülü ve harf aralıklarının denk geldiği tabloya göre bulduğumuz standart sapmayı ve tabloda denk gelen t score aralıklarını tersine çevirip not haline getiriyoruz böylece hangi harf aralığının hangi nota denk geldiğini buluyoruz


# 📌 Standart Sapma
```python

  Standart sapma  = (Öğrencinin ortalaması - Sınıf ortalaması) / ((T-score - 50) / 10) 

```
# 📌 En Düşük CC (Minimum CC):
```python

   Min CC = Sınıf Ortalaması - ((50 - T-score) / 10) * Standart Sapma

```



# 📌 Notlar
Sınıf ortalaması 45’in altında ise, sistem otomatik olarak en düşük CC’yi 45 olarak sabitler.

Standart sapma 8 ile 12 arasında olmalıdır. Sistem bu durumu renkli uyarı ile belirtir.



# Ortalamaya göre harf Aralığı Hesaplayıcı

Bu proje, T-score tabanlı bağıl not sistemine göre, sadece sınıf ortalamasını girerek harf notlarının  hangi aralıklara denk geldiğini hesaplayan bir web uygulamasıdır.

# 🚀 Proje Özellikleri

Yanlızca sınıf ortalamasını girerek:

AA'dan FF'ye kadar tüm not aralıklarını yaklaşık olarak hesaplar.

Hesaplanan aralıkları renkli bir tablo halinde gösterir.

# 🧮 Hesaplama Mantığı

Standart sapma yönetmelik gereği 8 ile 12 arasında olmak zorunda. Formülde standart sapmayı 11 kabul ederek gerçek sonuca yaklaşan bir değeri bulmayı hedefliyoruz.
Yönetmelikte ortalamaya göre tscore sonuçlarının listelendiği tablodan harf aralıklarınının hangi tscore sonucuna denk geldiğini bulup bunu tersine çevirip Harf aralıklarının hangi puanlara denk geldiğini buluyoruz


    Not Eşiği = ((Taban T-score - 50) / 10) * 11 + Sınıf Ortalaması


# ⚠️ Uyarılar
Bu hesaplama tahmine dayalıdır. Gerçek not aralıkları ile farklılık gösterebilir.




