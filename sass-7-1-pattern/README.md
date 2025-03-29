# Sass 7-1 Pattern Yapısı

Bu proje, **Sass 7-1 pattern** (7 klasör, 1 dosya) yapısına göre düzenlenmiş bir SCSS projesi örneğidir. Sass kodlarını daha okunabilir, sürdürülebilir ve modüler hale getirmek amacıyla bu yapı kullanılmıştır.

## 📁 Klasör Yapısı

```
sass/
│
├── abstracts/      // Değişkenler, mixinler, fonksiyonlar
├── base/           // Reset, base stil, tipografi vb.
├── components/     // Buton, kart, modal gibi küçük bileşenler
├── layout/         // Header, footer, sidebar, grid vb.
├── pages/          // Sayfa bazlı özel stiller
├── themes/         // Tema renkleri, dark/light modlar
├── vendors/        // Üçüncü parti kütüphaneler veya eklentiler
└── main.scss       // Tüm dosyaların import edildiği ana dosya
```

## 🛠 Kurulum

1. Bu repoyu klonlayın:
   ```bash
   git clone https://github.com/osmanelmaa/SASS7-1PATTERNTURKCEORNEKK
   ```

2. `main.scss` dosyasını `sass/` klasörü içinde bulabilir ve kendi projenize dahil edebilirsiniz.

## 📦 Kullanım

`main.scss` dosyası içinde şu şekilde import edilmiştir:

```scss
@use 'abstracts/variables';
@use 'abstracts/functions';
@use 'abstracts/mixins';

@use 'base/reset';
@use 'base/typography';
@use 'base/base';

@use 'layout/header';
@use 'layout/footer';
@use 'layout/grid';

@use 'components/button';
@use 'components/card';

@use 'pages/home';
@use 'pages/about';

@use 'themes/default';

@use 'vendors/bootstrap-overrides';
```

## 🎯 Amaç

- Kod tekrarını önlemek
- Daha düzenli ve okunabilir Sass dosyaları oluşturmak
- Büyük projelerde ekip çalışmasını kolaylaştırmak

## 📄 Lisans

Bu proje MIT lisansı ile lisanslanmıştır.
