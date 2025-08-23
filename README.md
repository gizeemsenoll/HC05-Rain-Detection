# 🌧️ HC-05 Bluetooth Modülü ile Yağmur Algılama ve Bildirim Sistemi

## 📌 Proje Tanımı
Bu projede, analog çıkışlı bir yağmur sensörü kullanılarak ortamda yağmur olup olmadığı tespit edilmekte ve durum bilgisi, **HC-05 Bluetooth modülü** aracılığıyla kablosuz olarak cep telefonuna iletilmektedir. Aynı zamanda bir **buzzer** yardımıyla sesli uyarı verilmektedir. Sensörden gelen değerler analiz edilerek yalnızca belirli koşullar sağlandığında uyarı verilmesi sağlanmıştır.

## 🎯 Proje Amacı
Dış ortamda yağmur algılandığında kullanıcıyı hem sesli hem de kablosuz (Bluetooth) olarak uyarmak.  
Bu proje, **stajım sırasında bilgi işlem sorumlumun yönlendirmesiyle** gerçekleştirilmiş olup, sensör kullanımı ve veri analizi konusunda deneyim kazandırmıştır.

## 🔌 Kullanılan Malzemeler
- Arduino UNO  
- HC-05 Bluetooth modülü  
- Yağmur sensörü (analog çıkışlı)  
- Buzzer  
- Jumper kablolar  
- Breadboard  

## 📲 Kullanılan Uygulama
Bluetooth verilerini okumak için Android işletim sistemli telefona **Serial Bluetooth Terminal** uygulaması yüklenmiştir. Arduino üzerinden gönderilen veriler bu uygulama aracılığıyla anlık olarak takip edilmiştir.

## ⚙️ Sistem İşleyişi
1. Yağmur sensöründen gelen analog değerler Arduino tarafından okunur.  
2. Değerlerdeki değişim oranı belli aralıklarla değerlendirilir.  
3. Eğer ani ve yüksek değer artışları varsa ve bu değerler belirli bir eşik değerin (örn. 500) üzerindeyse:  
   - Buzzer devreye girer  
   - HC-05 üzerinden cep telefonuna **“Yağmur tespit edildi”** mesajı gönderilir.  
4. Yağmur durduğunda buzzer kapanır ve telefon uygulamasına güncel durum bilgisi iletilir.  

## 🖥️ Kod
- Proje kodları `code/rain_detection.ino` dosyasında bulunmaktadır.

## 📷 Görseller
- Devre şeması  
- Serial Bluetooth Terminal uygulamasından alınan ekran görüntüleri
- Projenin görselleri 'images' dosyasında bulunmaktadır. 

## 🔍 Gözlemler
- Dış ortamda gerçek zamanlı yağmur durumu takibi başarıyla yapılmıştır.  
- Sistem yalnızca anlamlı değişimlerde tepki verdiğinden yanlış alarmlar önlenmiştir.  

---
✍️ **Hazırlayan:** Gizem Şenol  
📅 **Yıl:** 2025
