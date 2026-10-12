# MECHA FLIGHT — QR kumandalı sürüm

## GitHub Pages'e yükleme
1. GitHub'da `afurkan00/Flight` deposunun **Code** sekmesini aç.
2. Mevcut `index.html` dosyasını bu paketteki `index.html` ile değiştir. (Eski sürümün yedeğini alabilirsin.)
3. `controller.html` dosyasını **aynı dizine** ekle.
4. İki dosya da `main` dalının kökünde olmalı. Değişiklikleri commit et.
5. GitHub Actions'da `pages build and deployment` tamamlanınca bilgisayarda `https://afurkan00.github.io/Flight/` aç.
6. Bilgisayarda görünen QR kodu telefonla okut. Telefonda `Hareket sensörlerini aç` butonuna bas (iPhone'da Safari üzerinden izin ver).
7. Bilgisayardaki `UÇUŞA BAŞLA` butonuna bas. Halkadan geçince soru telefonda ve bilgisayarda görünür; cevabı telefondan seç, sonra `UÇUŞA DEVAM ET` de.

## Gereksinimler ve sınırlamalar
- İki cihazda internet; GitHub Pages HTTPS.
- Three.js ve PeerJS CDN üzerinden yüklenir. QR görüntüsü qrserver.com servisinden alınır.
- PeerJS'in genel sinyal sunucusu ve WebRTC veri kanalı kullanılır; ayrı backend / API anahtarı gerekmez.
- Bazı kurumsal ağlar / NAT kombinasyonları WebRTC bağlantısını engelleyebilir; mobil veri/hotspot ile tekrar dene. Bağlantı garantisi yoktur.
- Hareket sensörlerinin eksenleri cihazlara göre değişebilir. Sensör çalışmazsa telefon ekranındaki yön tuşları kullanılabilir.
- İlk bağlantıda yalnızca bir telefon kabul edilir; sonraki oyuncu için bilgisayarda sayfayı yenileyip yeni QR oluştur.
- Kod sözdizimi kontrol edildi, gerçek iPhone + bilgisayar birlikte test edilmedi.
