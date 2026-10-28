# 📡 MeshChat - İnternetsiz Eşler Arası (P2P) Mesajlaşma Uygulaması

<div align="center">

[![Android Studio](https://img.shields.io/badge/Android%2520Studio-3DDC84?style=for-the-badge&logo=android-studio&logoColor=white)](https://developer.android.com/)
[![Kotlin](https://img.shields.io/badge/Kotlin-0095D5?style=for-the-badge&logo=kotlin&logoColor=white)](https://kotlinlang.org/)
[![Jetpack Compose](https://img.shields.io/badge/Jetpack%2520Compose-4285F4?style=for-the-badge&logo=jetpack-compose&logoColor=white)](https://developer.android.com/jetpack/compose)
[![API 26+](https://img.shields.io/badge/API-26%2B%20%2F%2F%20Android%2017-orange?style=for-the-badge&logo=android&logoColor=white)](https://developer.android.com/)

**İnternete, baz istasyonuna veya modeme ihtiyaç duymadan; tamamen çevrimdışı, WhatsApp hızında ve uzun menzilli mesajlaşma deneyimi.**

</div>

---

## 🚀 Proje Hakkında

**MeshChat**, mobil cihazlar arasında hiçbir hücresel veri veya Wi-Fi ağına bağlanmadan, doğrudan donanım düzeyinde haberleşmeyi sağlayan modern bir Android uygulamasıdır. 

Uygulama; **Google Nearby Connections API** altyapısını kullanarak **Bluetooth LE (Düşük Enerji)** ile cihazları saniyeler içinde keşfeder ve bağlantıyı otomatik olarak **Wi-Fi Direct (P2P)** protokolüne yükseltir. Ayrıca sahip olduğu **Multi-Hop (Çoklu Atlama / Röle)** algoritması sayesinde, doğrudan menzil dışındaki cihazlara bile aradaki diğer telefonlar üzerinden köprü kurarak mesaj iletebilir.

---

## ✨ Öne Çıkan Özellikler

* **🌐 %100 İnternetsiz Çalışma:** Mobil veri, SIM kart, modem veya internet erişimi gerektirmez.
* **⚡ WhatsApp Hızında Arayüz:** Jetpack Compose ile tasarlanmış modern, şık ve akıcı koyu tema (`Dark Mode`) arayüzü.
* **🔄 Multi-Hop (Mesh Röle) Desteği:** Menzil dışındaki cihazlara, aradaki diğer telefonlar üzerinden mesaj aktarımı (otomatik paket sıçratma).
* **📱 Geniş Android Uyumluluğu:** **Android 8.0 (API 26)** sürümünden en yeni **Android 17 (API 37)** sürümüne kadar tüm telefonlarda kusursuz çalışır.
* **🤝 Otomatik Eşleşme:** Kullanıcıyı onay pencereleriyle uğraştırmadan etraftaki cihazları arka planda otomatik bulur ve bağlar.
* **🛡️ Döngü Koruma Mimarisi:** Benzersiz mesaj ID'leri (`msgId`) ve TTL (Time-To-Live) mekanizması ile sonsuz ağ döngülerini engeller.

---

## 🛠️ Kullanılan Teknolojiler

* **Dil:** Kotlin
* **Arayüz:** Jetpack Compose & Material 3
* **Ağ Motoru:** Google Play Services Nearby Connections API (P2P Cluster Strategy)
* **Mimari:** Reaktif Durum Yönetimi (Stateful UI & Coroutines)

---

## 📋 Gereksinimler ve İzinler

Uygulamanın düzgün çalışabilmesi için cihazlarda şu donanım anahtarlarının açık olması gerekir (İnternet kapalı olsa dahi):
* **Bluetooth** (Cihaz keşfi için)
* **Wi-Fi** (Yüksek hızlı P2P veri aktarımı için - ağa bağlanmak gerekmez)
* **Konum / GPS** (Android işletim sistemi kablosuz tarama yapabilmek için konum iznini zorunlu kılar)

### Desteklenen İzinler (`AndroidManifest.xml`):
* `BLUETOOTH_SCAN`, `BLUETOOTH_CONNECT`, `BLUETOOTH_ADVERTISE`
* `NEARBY_WIFI_DEVICES` (Android 13+)
* `ACCESS_LOCAL_NETWORK` (Android 17 / API 37+)

---

## 📥 Kurulum ve Kullanım

1. **APK'yı İndirin:** Projenin [Releases](../../releases) sayfasından en güncel `app-debug.apk` dosyasını telefonunuza indirin ve kurun.
2. **Bağlantıları Açın:** Telefonunuzda **Wi-Fi, Bluetooth ve Konum** servislerini açın (Mobil veriyi kapatabilirsiniz).
3. **Uygulamayı Başlatın:** İki veya daha fazla telefonda uygulamayı açın. Otomatik olarak bağlanacak ve üst barda bağlı cihaz sayısını göreceksiniz.
4. **Mesajlaşmaya Başlayın:** Alttaki mesaj kutusunu kullanarak internetsiz ve sınırsız şekilde sohbet edin!

---

## 👨‍💻 Geliştirici

Bu proje, modern mobil ağ teknolojileri ve çevrimdışı haberleşme sistemleri (Mesh Networks) üzerinde pratik yapmak amacıyla geliştirilmiştir. Katkıda bulunmak veya geliştirmek istiyorsanız depoyu fork'layabilir ya daissue açabilirsiniz.


<div align="center">

<a href="https://github.com/eymen55kaya52-star/OfflineMeshChat/releases/latest/download/meshtr.apk">
  <img src="https://img.shields.io/badge/📥%20APK%20İNDİR-EN%20SON%20SÜRÜM-00A884?style=for-the-badge&logo=android&logoColor=white" alt="APK İndir" height="50"/>
</a>

</div>
