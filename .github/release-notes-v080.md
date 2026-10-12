# NöbetçiTakvim v0.8.0

> **Daha sade bir arayüz, daha güçlü dosya takibi ve daha güvenilir senkronizasyon.**

NöbetçiTakvim; işleri, duruşmaları, keşifleri ve toplantıları tek yerde takip etmek için geliştirdiğim **yerel öncelikli (local-first)** masaüstü uygulaması.  
UYAP Avukat Portal’dan indirilebilen `.ics` takvim dosyalarını içe aktarabilir, kayıtları isteğe bağlı olarak Google Takvim’e yansıtabilir.

**0.8.0**, yeni özellik eklemekten çok günlük kullanımı daha anlaşılır, daha hızlı ve daha güvenilir hâle getiren bir sürüm.

## ✨ Öne çıkan yenilikler

### 🎨 Dosya renkleri
Dosyalara **Kırmızı, Turuncu, Sarı, Yeşil, Mavi veya Mor** renk atanabiliyor.  
Aynı dosyaya bağlı kayıtlar listelerde daha kolay ayırt ediliyor; seçilen renk ilgili Google Takvim kayıtlarına da yansıyor.

### 🏠 Yenilenen Anasayfa
Anasayfa artık yalnız bir özet ekranı değil, günlük çalışma masası:

- **Geciken işler**
- **Bugün**
- **Süresiz işler**
- **Yarın**
- **Yaklaşan kayıtlar**
- **Notlar**

tek ekranda görülebiliyor.

### 📊 Klasik / Görsel İş Öncelik Matrisi
İşler için iki görünüm arasında seçim yapılabiliyor:

- **Klasik:** Geciken · Son Gün · Yarın · 2–3 Gün · 4–6 Gün · 7+ Gün · Süresiz
- **Görsel:** 0–3 · 4–7 · 8–10 · 11–14 gün

Geciken, 14 günden uzun süreli ve süresiz işler ayrıca gösteriliyor; hiçbir açık iş görünüm dışında kalmıyor.

### ⚖️ Duruşma / Keşif Yakınlık Matrisi
Yaklaşan duruşma ve keşifler **Geçmiş · Bugün · Yarın · 2–3 Gün · 4–7 Gün · 8+ Gün** aralıklarında tek bakışta görülebiliyor.

### 🧭 Daha sade kenar çubuğu
Kenar çubuğu yeniden düzenlendi ve sıkılaştırıldı.  
Temel gezinme, aktarım araçları, tema ve ayarlar daha belirgin bir hiyerarşiye kavuştu; dar görünümde de temel işlevler erişilebilir kalıyor.

### 👤 Daha fazla dosya bağlamı
İş listelerinde artık ilgili **müvekkil, dosya numarası ve mahkeme** bilgileri doğrudan görülebiliyor.  
Kayıtlara sol tıklamak ayrıntıyı açıyor; sağ tık menüsü görüntüleme, düzenleme, tamamlama ve çöpe taşıma gibi hızlı işlemleri sunuyor.

## 🔔 Hatırlatmalar ve Google Takvim

- Dosyaya özel **Google Takvim hatırlatma profilleri** tanımlanabiliyor.
- İşler, duruşma/keşifler, toplantılar ve diğer kayıtların Google’a aktarımı ayrı ayrı açılıp kapatılabiliyor.
- Tamamlanıp yeniden açılan kayıtlarda ikinci Google etkinliği oluşmasına yol açabilecek senkronizasyon kenar durumları giderildi.
- Dosyadaki Google’ı etkilemeyen değişiklikler artık gereksiz toplu yeniden senkronizasyon başlatmıyor.
- Toplantı hatırlatma arayüzü gerçek davranışla uyumlu hâle getirildi.

## 🔐 Mahremiyet ve güvenlik

NöbetçiTakvim’in temel yaklaşımı değişmedi: **mesleki veriler geliştirici tarafa gönderilmez.**

- Yerel **Uygulama Kilidi** ile uygulama isteğe bağlı parola ile korunabiliyor.
- UYAP’tan içe aktarılan **Vekili Olunan Taraflar** ve **Diğer Taraflar** bilgileri artık Google Takvim açıklamalarına gönderilmiyor.
- Yerel ham UYAP kaydı ise bilgisayarda korunmaya devam ediyor.
- Uygulama Kilidi, cihaz başında mahremiyet içindir; **veritabanı şifrelemesi değildir.**

## 🧹 Sadeleştirmeler ve küçük iyileştirmeler

- Kullanıcıya gerçek bir davranış kazandırmayan **Hedef Gün** alanı kaldırıldı; eski veriler silinmedi.
- Notlara hızlı ve onaylı silme eklendi.
- İşlem Kanıtı alanı çoklu giriş destekleyecek şekilde geliştirildi.
- Kenar çubuğuna yerel tarih ve saat göstergesi eklendi.
- Süre hesabında **Ay** birimi kullanılabilir hâle geldi.
- Uygulama gece yarısını açık geçirdiğinde veya bilgisayar uykudan uyandığında “bugün”e bağlı ekranlar otomatik olarak yeni güne güncelleniyor.
- Ayarlar; **Genel · Bildirimler · Google Takvim · Gizlilik ve Güvenlik · Veri ve Yedekleme** şeklinde yeniden düzenlendi.

---

## 💻 İndirme

### macOS — Apple Silicon
**Dosya:** `NobetciTakvim-0.8.0-arm64.dmg`

Developer ID ile imzalıdır ve Apple tarafından **notarize** edilmiştir.

```text
SHA-256: ddc378ee8d41a5e4aaaf889b7628874e104684c99c83d85c8e70ddd8749259e8
```

### Windows — x64
**Dosya:** `NobetciTakvim.Setup.0.8.0.exe`

NSIS tabanlı kullanıcı kurulumu içerir.

```text
SHA-256: ef8bb4d3fc4bcc48bd3a3292d2f7bc392bdb555f41699074bca789987177708b
```

> **Windows notu:** Bu sürümün Windows paketi henüz kod imzalı değildir. Bu nedenle Windows SmartScreen ilk çalıştırmada uyarı gösterebilir.

---

**NöbetçiTakvim 0.8.0:** daha az gürültü, daha açık mekanizma, daha öngörülebilir davranış.
