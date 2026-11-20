[English](../../README.md) | [Português (Brasil)](README.pt-BR.md) | [Español](README.es.md) | [Català](README.ca.md) | [Italiano](README.it.md) | [简体中文](README.zh-CN.md) | [Русский](README.ru.md) | [Bahasa Indonesia](README.id.md) | [Polski](README.pl.md) | [日本語](README.ja.md) | [العربية](README.ar.md) | **Türkçe**

# Hakkında

AnyPS5 çalıştırılabilir dosyaları (ör: *.exe) Linux'a veya Windows'a portlayan bir araçdır.

Yalnızca yeniden bağlantı kurma özelliğine sahip sürüm, Apple Silicon dahil olmak üzere macOS üzerinde çalışır.

[**Web Çevirme Aracı**](https://boykopovar.github.io/AnyPS5/) - dosyalar bilgisayarınızda kalır.

![anyps5_collage1](https://github.com/user-attachments/assets/ed2f0b2d-33d3-46d7-ab88-767ca872fc99)

Yürütülebilir dosyayı (ör: *.exe) hedef sistemin yerel formatına dönüştüren bir [Yeniden Bağlayıcı](core/relinker) ve dinamik bağlantılar için [Sistem prx Kütüphaneleri](core/libs/prx) içerir. Önyüklemesi veya ayrı bir çalışma parçacığı bulunmamaktadır.

[**Discord**](https://discord.gg/x9naWVzC6A), [Kullanımı](docs/user/USAGE.md), [Derleme Talimatları](docs/dev/BUILD.md), [Yapı](docs/dev/ARCHITECTURE.md), [Projenin Teknik Dezavantajları](docs/dev/TechnicalDebt.md), [Kod Stili Kuralları](docs/dev/CONVENTIONS.md), [Katkıda Bulunanlar](CONTRIBUTING.md)

## Durum
[![libraries](https://boykopovar.github.io/AnyPS5/badge-libraries.svg)](https://boykopovar.github.io/AnyPS5/progress.html) [![RDNA2 referans gölgeleyici formlarının çözümlenmesi
](https://boykopovar.github.io/AnyPS5/badge-shaders.svg)](https://boykopovar.github.io/AnyPS5/progress.html) [![gfx1013 referans gölgeleyici formlarının çözümlenmesi](https://boykopovar.github.io/AnyPS5/badge-shaders-gfx1013.svg)](https://boykopovar.github.io/AnyPS5/progress.html) [![7 gün içerisinde gerçekleştirildi](https://boykopovar.github.io/AnyPS5/badge-week.svg)](https://boykopovar.github.io/AnyPS5/history.html)

[![Süreç Haritası](https://boykopovar.github.io/AnyPS5/progress.svg)](https://boykopovar.github.io/AnyPS5/progress.html)

[Süreç Geçmişi](https://boykopovar.github.io/AnyPS5/history.html)

<sub>* Sistem Kütüphaneleri: projenin bu güne kadar bilinen fonksiyonları  [core/libs/prx](core/libs/prx)'de tanımlandı), her PS5 sistem fonksiyonu için geçerli değildir. Toplam değer yeni fonksiyon tanımladıkça büyümektedir.</sub>

Desteklenmeyen veya beklenmeyen durumlar C++ istisna(exception) verirler. Bu istisnalar genellikle `std::runtime_error`dur. Hiç bir değer döndürmeyen istisnalar ise `what()` değerini stderr'e yazdırır ve işlemi sonlandırır..

[Gölge Derleyicisi](core/shader/recompiler/Recompiler.cpp) `ANYPS5_ENABLE_SPIRV_TOOLS` aracıyla derlendiğinde başarıyla SPIR-V (ile doğrulandı: [Spirv-Tools](3rdparty/SPIRV-Tools) üretmektedir.

## Uyumluluk

Oyun bazlı testler ve raporlar canlı olarak [Oyun başlatma](https://github.com/boykopovar/AnyPS5/discussions/categories/game-bring-up)'da tartışmalar halinde her oyuna özel başlık altında gözükmektedir.

## Oyun Girdileri

SDL tabanlı girdiler analog çubukları ve tetikleyiciler dahil desteklenmektedir. Klavye ve fareler ise `anyps5-input.ini` dosyası ile birlikte ayarlanabilmektedir.
[Oyun girdileri](docs/user/INPUT_MAPPING.md) kısmından desteklenen cihazlar ve desteklenen ayarlar gözükmektedir.

## Yasal Uyarı

Bu proje, birlikte çalışabilirlik, araştırma, koruma ve uyumluluk amaçları için tasarlanmıştır. Telif hakkıyla korunan yazılım, donanım yazılımı, şifreleme anahtarları veya tescilli kütüphaneleri içermez, dağıtmaz veya gerektirmez. Kullanıcılar, bu projeyle kullanılan ikili dosyaların ilgili yasalara ve ilgili lisans koşullarına uygun olarak elde edildiğinden ve kullanıldığından emin olmakla sorumludur.

AnyPS5 bağımsız bir projedir ve Sony Interactive Entertainment ile bağlantılı değildir, onun tarafından yetkilendirilmemiştir veya onaylanmamıştır. "PlayStation" ve "PS5" Sony Interactive Entertainment Inc.'in ticari markalarıdır.

## License

Bu proje sadece GNU General Public License version 2 altında lisanslanmıştır.


