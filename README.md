# NöbetçiTakvim

**Avukatlar için masaüstü iş, duruşma ve süre takip uygulaması.**  
*Her iş, vaktinde.*

NöbetçiTakvim; duruşmaları, yapılacak işleri, hukuki süreleri, müvekkilleri ve dosyaları tek bir sade çalışma alanında toplar. Amacı yeni bir büro yönetim sistemi kurmak değil; hukuk pratiğinde unutulmaması gereken işi, doğru zamanda ve doğru dosyayla birlikte görünür kılmaktır.

> **Ücretsizdir. Verilerin ana kaydı cihazınızda tutulur.** Bu depo yalnız NöbetçiTakvim'in macOS ve Windows dağıtım paketlerini içerir; kaynak kod içermez.

## Neden NöbetçiTakvim?

Hukuk pratiğinde takip edilmesi gereken şeyler aynı türden değildir: bir dosyada duruşma, diğerinde bilirkişi raporuna beyan, başka bir dosyada tebligata bağlı son gün veya yerine getirilmesi gereken bir ara karar vardır.

NöbetçiTakvim bu farklı işleri tek ve anlaşılır bir akışta bir araya getirir:

- **İş ve süre takibi:** Süreli veya süresiz işleri kaydedin; hatırlatmaları ihtiyacınıza göre yönetin.
- **Duruşma takvimi:** Yaklaşan duruşmaları tarih ve saat sırasıyla tek ekranda görün.
- **UYAP `.ics` içe aktarma:** UYAP Avukat Portal'dan alınan takvim dosyalarını içe aktarın; duruşmalarla birlikte uygun müvekkil ve dosya kartları otomatik oluşturulsun.
- **Bilgi Kartı:** Müvekkilleri ve dosyaları birbirine bağlı, fakat birbirinden bağımsız kayıtlar olarak yönetin.
- **Hukuki süre hesabı:** Tebligata bağlı sürelerde son günü deterministik olarak hesaplayın; hesaplanan tarih kullanıcı onayı olmadan kaydedilmez.
- **Gerçek UYAP evrak türleri:** Hukuk, ceza, idari yargı, icra ve soruşturma dosyalarında UYAP'taki gerçek evrak türlerinden bağlama uygun öneriler alın; isterseniz kendi metninizi yazın.
- **Türkçe arama:** Büyük/küçük harf farkından bağımsız, Türkçe karakterlerle uyumlu arama.
- **Excel dışa aktarımı:** İş listesini ve dosya listesini Excel'e aktarın.
- **Açık ve koyu tema:** Tema tercihi kalıcı olarak saklanır.
- **Erişilebilir kullanım:** Klavye erişimi, görünür odak durumları ve ekran okuyucu etiketleri uygulamanın temel arayüzlerinde korunur.

## Hukuki sürelerde son söz kullanıcıda

NöbetçiTakvim süreyi sizin yerinize "kesinleştirmez". Hesaplamayı açık kurallarla yapar, sonucu gösterir ve **hesaplanan son tarih kullanıcı tarafından doğrulanmadan kaydetmez**.

Bu yaklaşım bilinçlidir: uygulama mekanik işi azaltır; hukuki değerlendirme ve nihai sorumluluk kullanıcıda kalır.

## UYAP ile birlikte, UYAP'ın yerine değil

NöbetçiTakvim UYAP'ın yerini almaya çalışmaz. UYAP Avukat Portal'dan alınan `.ics` takvim dosyalarını yerel çalışma düzeninize taşır ve bunları daha kullanılabilir bir iş/dosya yapısına dönüştürür.

İçe aktarma sırasında:

- vekili olunan taraflardan müvekkil kartları oluşturulabilir,
- mahkeme/kurum ve dosya numarasından dosya kartları oluşturulabilir,
- aynı veri yeniden içe aktarıldığında mükerrer kayıt üretmemeye çalışılır,
- elle eklediğiniz müvekkil bilgileri otomatik içe aktarma nedeniyle ezilmez.

## İndir

En güncel kararlı sürüm için **[Releases](../../releases/latest)** sayfasını açın.

| Platform | Paket |
| --- | --- |
| macOS — Apple Silicon | `NobetciTakvim-<sürüm>-arm64.dmg` |
| Windows — x64 | `NobetciTakvim.Setup.<sürüm>.exe` |

### macOS

macOS paketleri **Apple Developer ID** ile imzalanır ve Apple tarafından **notarize** edilir.

DMG dosyasını açın ve NöbetçiTakvim'i **Applications / Uygulamalar** klasörüne taşıyın.

### Windows

Windows sürümü NSIS kurulum paketi olarak dağıtılır. Mevcut Windows paketi kod imzasız olduğundan SmartScreen ilk kurulumda uyarı gösterebilir.

## Veri yaklaşımı

NöbetçiTakvim **local-first** tasarlanmıştır. Müvekkil, dosya, iş ve takvim verilerinin ana kaydı cihazınızdadır. Uygulama; belge içeriğini analiz etmek, hukuki karar vermek veya kullanıcı verisini uzaktaki bir yapay zekâ servisine göndermek üzerine kurulmamıştır.

Google Takvim bağlantısı kullanılıyorsa bu, isteğe bağlı bir yardımcı kanal olarak çalışır; uygulamanın yerel kayıt yapısının yerini almaz.

## Dosya doğrulama

Her sürümün release notlarında yayımlanan paketler için **SHA-256** özetleri bulunur. İndirdiğiniz dosyanın bütünlüğünü bu değerlerle doğrulayabilirsiniz.

## Dağıtım deposu hakkında

Bu repository yalnız son kullanıcıya sunulan NöbetçiTakvim paketlerinin dağıtımı içindir.

**Kaynak kod bu depoda yayımlanmaz.**

---

**NöbetçiTakvim** — *Her iş, vaktinde.*  
© 2026 Raci Çetin Yüksekbaş
