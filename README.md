### HTML Temel Etiketler

- `<footer>`: Sayfanın alt bilgisini belirtir, genellikle telif hakkı bilgileri, yasal uyarılar veya iletişim bilgileri içerir.
- `<div>`: Blok düzeyinde bir bölüm oluşturur, genellikle stil veya komut dosyaları ile gruplandırma yapmak için kullanılır.
- `<section>`: Belgenin belirli bir bölümünü tanımlar, genellikle başlık içerir ve tematik olarak ilgili içerikleri gruplar.
- `<caption>`: Tabloya başlık ekler, genellikle tablonun üstünde yer alır ve tablonun içeriğini açıklar.
- `<thead>`: Tablo başlık satırlarını gruplar.
- `<tbody>`: Tablo gövde satırlarını gruplar.
- `<tfoot>`: Tablo alt bilgi satırlarını gruplar.
- `<colgroup>`: Tablo sütunlarını gruplar ve sütunlara stil veya özellikler ekler.
- `<col>`: Tek bir tablo sütununa stil veya özellikler ekler.
- `<html>`: HTML belgesinin kök etiketidir.
- `<head>`: Belge hakkında meta bilgileri içerir.
- `<title>`: Belgenin başlığını belirtir.
- `<body>`: Belgenin içeriğini barındırır.

### Etiketlere Ait Parametreler

- `<a href="url" target="_blank">`: Bağlantı etiketi, `href` parametresi ile bağlantı adresi belirlenir, `target` parametresi ile bağlantının yeni bir sekmede açılması sağlanır.
- `<img src="image.jpg" alt="description" width="500" height="300">`: Görsel etiketi, `src` parametresi ile görsel kaynağı, `alt` parametresi ile alternatif metin, `width` ve `height` parametreleri ile görsel boyutları belirlenir.

## Tablo, Listeleme ve Form

### Tablo

- `<table border="1" cellpadding="10" cellspacing="0">`: Tablo oluşturur, `border` parametresi ile kenarlık kalınlığı, `cellpadding` parametresi ile hücre içi boşluk, `cellspacing` parametresi ile hücreler arası boşluk belirlenir.
- `<tr>`: Tablo satırı oluşturur.
- `<td align="center">`: Tablo hücresi oluşturur, `align` parametresi ile yatay hizalama belirlenir.
- `<th>`: Tablo başlık hücresi oluşturur.
- `<caption>`: Tabloya başlık ekler, genellikle tablonun üstünde yer alır ve tablonun içeriğini açıklar.
- `<colgroup span="2">`: Tablo sütunlarını gruplar ve sütunlara stil veya özellikler ekler, `span` parametresi ile gruptaki sütun sayısı belirlenir.
- `<col span="2" style="background-color: #f2f2f2;">`: Tek bir tablo sütununa stil veya özellikler ekler, `span` parametresi ile sütun sayısı, `style` parametresi ile CSS stilleri belirlenir.
- `<td colspan="2" rowspan="2" align="center">`: Tablo hücresi oluşturur, `colspan` parametresi ile hücrenin kapladığı sütun sayısı, `rowspan` parametresi ile hücrenin kapladığı satır sayısı, `align` parametresi ile yatay hizalama belirlenir.

### Listeleme

- `<ul class="circle-list">`: Sırasız liste oluşturur.
- `<ol class="roman-list" start="3">`: Sıralı liste oluşturur, `start` parametresi ile başlangıç numarası belirlenir.
- `<li>`: Liste öğesi oluşturur.

### Form

- `<form action="/submit">`: Form oluşturur, `action` parametresi ile formun gönderileceği adres belirlenir.
- `<input type="text" name="isim" placeholder="İsminizi girin" required>`: Kullanıcıdan veri almak için giriş alanı oluşturur, `type` parametresi ile giriş türü, `name` parametresi ile alan adı, `placeholder` parametresi ile örnek metin, `required` parametresi ile zorunlu alan belirlenir.
- `<button type="submit" disabled>Gönder</button>`: Buton oluşturur, `type` parametresi ile buton türü, `disabled` parametresi ile butonun devre dışı bırakılması sağlanır.

## CSS Özellikleri

### Border Özellikleri

- `border: 1px solid black;`: Kenarlık özelliklerini belirler, `1px` kalınlık, `solid` stil ve `black` renk.
- `border-radius: 10px;`: Kenarlık köşelerini yuvarlar, `10px` yarıçap.

#### Örnek:

```html
<div class="border-example">Kenarlık Örneği</div>
```

```css
.border-example {
  border: 1px solid black;
  border-radius: 10px;
  padding: 10px;
}
```

#### Çıktı:

<div class="border-example">Kenarlık Örneği</div>

### Renklendirme

- `color: #333;`: Metin rengini belirler, `#333` renk kodu.
- `background-color: #f0f0f0;`: Arka plan rengini belirler, `#f0f0f0` renk kodu.

#### Örnek:

```html
<div class="color-example">Renklendirme Örneği</div>
```

```css
.color-example {
  color: #333;
  background-color: #f0f0f0;
  padding: 10px;
}
```

#### Çıktı:

<div class="color-example">Renklendirme Örneği</div>

### Class Kullanımı

- `.className { font-size: 16px; margin: 10px; }`: CSS sınıfı tanımlar ve HTML öğelerine uygulanır, `font-size` ile yazı boyutu, `margin` ile dış boşluk belirlenir.

#### Örnek:

```html
<div class="class-example">Class Kullanımı Örneği</div>
```

```css
.class-example {
  font-size: 16px;
  margin: 10px;
}
```

#### Çıktı:

<div class="class-example">Class Kullanımı Örneği</div>

### Hover Özelliği

- `a:hover { text-decoration: underline; }`: Fare ile üzerine gelindiğinde uygulanacak stilleri belirler, `text-decoration` ile alt çizgi eklenir. Bu özellik, kullanıcıların fare ile bir bağlantının üzerine geldiğinde görsel bir geri bildirim almasını sağlar.

#### Örnek:

```html
<a href="#" class="hover-example">Hover Örneği</a>
```

```css
.hover-example:hover {
  text-decoration: underline;
}
```

#### Çıktı:

<a href="#" class="hover-example">Hover Örneği</a>

## HTML ve CSS Bağlantısı

- `<link rel="stylesheet" href="styles.css">`: Harici CSS dosyasını HTML belgesine bağlar.
- `<style> body { font-family: Arial, sans-serif; } </style>`: Dahili CSS stillerini HTML belgesine ekler.

## Örnek Kodlar

### Sıfırdan Kod

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Örnek Sayfa</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <h1>Merhaba Dünya</h1>
  </body>
</html>
```

### Listeleme Örneği

```html
<ul class="circle-list">
  <li>Öğe 1</li>
  <li>Öğe 2</li>
</ul>
<ol class="roman-list" start="3">
  <li>Öğe 1</li>
  <li>Öğe 2</li>
</ol>
```

#### Çıktı:

<ul class="circle-list">
  <li>Öğe 1</li>
  <li>Öğe 2</li>
</ul>
<ol class="roman-list" start="3">
  <li>Öğe 1</li>
  <li>Öğe 2</li>
</ol>

### Tablo ve Form Örneği

```html
<table border="1" cellpadding="10" cellspacing="0">
  <tr>
    <th>Ad</th>
    <th>Soyad</th>
  </tr>
  <tr>
    <td>Ali</td>
    <td>Veli</td>
  </tr>
  <tr>
    <td colspan="2">
      <form action="/submit">
        <label for="isim">İsim:</label>
        <input
          type="text"
          id="isim"
          name="isim"
          placeholder="İsminizi girin"
          required
        />
        <button type="submit">Gönder</button>
      </form>
    </td>
  </tr>
</table>
```

#### Çıktı:

<table border="1" cellpadding="10" cellspacing="0">
  <tr>
    <th>Ad</th>
    <th>Soyad</th>
  </tr>
  <tr>
    <td>Ali</td>
    <td>Veli</td>
  </tr>
  <tr>
    <td colspan="2">
      <form action="/submit">
        <label for="isim">İsim:</label>
        <input
          type="text"
          id="isim"
          name="isim"
          placeholder="İsminizi girin"
          required
        />
        <button type="submit">Gönder</button>
      </form>
    </td>
  </tr>
</table>

### CSS Örneği

```css
.circle-list {
  list-style-type: circle;
}

.roman-list {
  list-style-type: upper-roman;
}

.sirasiz-liste li:hover {
  color: red;
}

.sirali-liste li:hover {
  color: blue;
}
```

### Form Etiketleri ve Özellikleri

- `<input type="text" name="isim" placeholder="İsminizi girin" required>`: Kullanıcıdan metin girişi almak için kullanılır. `type` parametresi "text" olarak ayarlanmıştır.
- `<input type="password" name="sifre" placeholder="Şifrenizi girin" required>`: Kullanıcıdan şifre girişi almak için kullanılır. `type` parametresi "password" olarak ayarlanmıştır.
- `<input type="email" name="email" placeholder="Email adresinizi girin" required>`: Kullanıcıdan email girişi almak için kullanılır. `type` parametresi "email" olarak ayarlanmıştır.
- `<input type="number" name="yas" min="1" max="100" step="1">`: Kullanıcıdan sayı girişi almak için kullanılır. `type` parametresi "number" olarak ayarlanmıştır. `min`, `max` ve `step` parametreleri ile sayı aralığı ve adımı belirlenir.
- `<input type="date" name="dogum_tarihi">`: Kullanıcıdan tarih girişi almak için kullanılır. `type` parametresi "date" olarak ayarlanmıştır.
- `<input type="checkbox" name="sozlesme" required>`: Kullanıcıdan onay almak için kullanılır. `type` parametresi "checkbox" olarak ayarlanmıştır.
- `<input type="radio" name="cinsiyet" value="erkek">`: Kullanıcıdan seçenekler arasında seçim yapmak için kullanılır. `type` parametresi "radio" olarak ayarlanmıştır.
- `<input type="file" name="dosya">`: Kullanıcıdan dosya yüklemesi almak için kullanılır. `type` parametresi "file" olarak ayarlanmıştır.
- `<textarea name="mesaj" rows="4" cols="50" placeholder="Mesajınızı girin"></textarea>`: Kullanıcıdan çok satırlı metin girişi almak için kullanılır. `rows` ve `cols` parametreleri ile metin alanının boyutu belirlenir.
- `<select name="sehir">`: Kullanıcıdan açılır menü ile seçim yapmak için kullanılır.
  - `<option value="istanbul">İstanbul</option>`: Açılır menü seçeneği.
  - `<option value="ankara">Ankara</option>`: Açılır menü seçeneği.
  - `<option value="izmir">İzmir</option>`: Açılır menü seçeneği.
- `<button type="submit">Gönder</button>`: Formu göndermek için kullanılır. `type` parametresi "submit" olarak ayarlanmıştır.
- `<button type="reset">Temizle</button>`: Formu sıfırlamak için kullanılır. `type` parametresi "reset" olarak ayarlanmıştır.

### Video Ekleme

- `<video src="video.mp4" controls width="600" height="400">`: Video eklemek için kullanılır. `src` parametresi ile video kaynağı, `controls` parametresi ile oynatma kontrolleri, `width` ve `height` parametreleri ile video boyutları belirlenir.
  ```html
  <video src="video.mp4" controls width="600" height="400">
    Tarayıcınız video etiketini desteklemiyor.
  </video>
  ```

### Yatay Çizgi ve Satır Sonu

- `<hr>`: Yatay çizgi ekler.
  ```html
  <hr />
  ```
- `<br>`: Satır sonu ekler.
  ```html
  Satır sonu<br />eklemek için kullanılır.
  ```

### Yorum Satırı

- `<!-- Yorum -->`: HTML'de yorum eklemek için kullanılır.
  ```html
  <!-- Bu bir yorum satırıdır -->
  ```

### Başlık Etiketleri

- `<h1>` - `<h6>`: Başlık etiketleri, `<h1>` en büyük, `<h6>` en küçük başlık.
  ```html
  <h1>Başlık 1</h1>
  <h2>Başlık 2</h2>
  <h3>Başlık 3</h3>
  <h4>Başlık 4</h4>
  <h5>Başlık 5</h5>
  <h6>Başlık 6</h6>
  ```

### Metin Biçimlendirme Etiketleri

- `<b>`: Kalın metin.
- `<i>`: İtalik metin.
- `<u>`: Altı çizili metin.
- `<strong>`: Vurgulu kalın metin.
- `<em>`: Vurgulu italik metin.
- `<mark>`: Vurgulu arka plan rengi.
- `<small>`: Küçük metin.
- `<del>`: Üstü çizili metin.
- `<ins>`: Altı çizili metin.
- `<sub>`: Alt simge.
- `<sup>`: Üst simge.
  ```html
  <b>Kalın</b>
  <i>İtalik</i>
  <u>Altı çizili</u>
  <strong>Vurgulu kalın</strong>
  <em>Vurgulu italik</em>
  <mark>Vurgulu arka plan</mark>
  <small>Küçük</small>
  <del>Üstü çizili</del>
  <ins>Altı çizili</ins>
  <sub>Alt simge</sub>
  <sup>Üst simge</sup>
  ```

### Görsel Ekleme

- `<img src="image.jpg" alt="description" width="500" height="300">`: Görsel eklemek için kullanılır. `src` parametresi ile görsel kaynağı, `alt` parametresi ile alternatif metin, `width` ve `height` parametreleri ile görsel boyutları belirlenir.
  ```html
  <img src="image.jpg" alt="Açıklama" width="500" height="300" />
  ```

### Form Etiketleri

- `<form action="/submit">`: Form oluşturur.
- `<input type="text" name="isim" placeholder="İsminizi girin" required>`: Metin girişi.
- `<input type="password" name="sifre" placeholder="Şifrenizi girin" required>`: Şifre girişi.
- `<input type="email" name="email" placeholder="Email adresinizi girin" required>`: Email girişi.
- `<input type="number" name="yas" min="1" max="100" step="1">`: Sayı girişi.
- `<input type="date" name="dogum_tarihi">`: Tarih girişi.
- `<input type="checkbox" name="sozlesme" required>`: Onay kutusu.
- `<input type="radio" name="cinsiyet" value="erkek">`: Radyo butonu.
- `<input type="file" name="dosya">`: Dosya yükleme.
- `<textarea name="mesaj" rows="4" cols="50" placeholder="Mesajınızı girin"></textarea>`: Çok satırlı metin girişi.
- `<select name="sehir">`: Açılır menü.
  - `<option value="istanbul">İstanbul</option>`
  - `<option value="ankara">Ankara</option>`
  - `<option value="izmir">İzmir</option>`
- `<button type="submit">Gönder</button>`: Gönder butonu.
- `<button type="reset">Temizle</button>`: Temizle butonu.
  ```html
  <form action="/submit">
    <input type="text" name="isim" placeholder="İsminizi girin" required />
    <input
      type="password"
      name="sifre"
      placeholder="Şifrenizi girin"
      required
    />
    <input
      type="email"
      name="email"
      placeholder="Email adresinizi girin"
      required
    />
    <input type="number" name="yas" min="1" max="100" step="1" />
    <input type="date" name="dogum_tarihi" />
    <input type="checkbox" name="sozlesme" required /> Sözleşmeyi kabul ediyorum
    <input type="radio" name="cinsiyet" value="erkek" /> Erkek
    <input type="radio" name="cinsiyet" value="kadin" /> Kadın
    <input type="file" name="dosya" />
    <textarea
      name="mesaj"
      rows="4"
      cols="50"
      placeholder="Mesajınızı girin"
    ></textarea>
    <select name="sehir">
      <option value="istanbul">İstanbul</option>
      <option value="ankara">Ankara</option>
      <option value="izmir">İzmir</option>
    </select>
    <button type="submit">Gönder</button>
    <button type="reset">Temizle</button>
  </form>
  ```

### HTML5 Temel Özellikleri ve Yeni Gelen Özellikler

- `<article>`: Bağımsız içerik parçası.
- `<aside>`: Yan içerik.
- `<details>`: Gizlenebilir içerik.
- `<figcaption>`: Resim alt yazısı.
- `<figure>`: Resim ve alt yazı grubu.
- `<footer>`: Alt bilgi.
- `<header>`: Üst bilgi.
- `<main>`: Ana içerik.
- `<mark>`: Vurgulu metin.
- `<nav>`: Navigasyon.
- `<section>`: Bölüm.
- `<summary>`: Gizlenebilir içeriğin başlığı.
- `<time>`: Zaman.
  ```html
  <article>
    <header>
      <h1>Makale Başlığı</h1>
    </header>
    <p>Makale içeriği...</p>
    <footer>Makale alt bilgisi</footer>
  </article>
  <aside>Yan içerik</aside>
  <details>
    <summary>Detaylar</summary>
    <p>Gizlenebilir içerik</p>
  </details>
  <figure>
    <img src="image.jpg" alt="Açıklama" />
    <figcaption>Resim alt yazısı</figcaption>
  </figure>
  <footer>Sayfa alt bilgisi</footer>
  <header>Sayfa üst bilgisi</header>
  <main>Ana içerik</main>
  <mark>Vurgulu metin</mark>
  <nav>Menü</nav>
  <section>Bölüm</section>
  <time datetime="2023-10-01">1 Ekim 2023</time>
  ```

### Detaylı CSS Özellikleri

- `margin`: Dış boşluk.
- `padding`: İç boşluk.
- `border`: Kenarlık.
- `background`: Arka plan.
- `color`: Metin rengi.
- `font-size`: Yazı boyutu.
- `font-family`: Yazı tipi.
- `text-align`: Metin hizalama.
- `display`: Görüntüleme türü.
- `position`: Konumlandırma.
- `top`, `right`, `bottom`, `left`: Konum.
- `width`, `height`: Genişlik ve yükseklik.
- `max-width`, `max-height`: Maksimum genişlik ve yükseklik.
- `min-width`, `min-height`: Minimum genişlik ve yükseklik.
- `opacity`: Saydamlık.
- `transition`: Geçiş efekti.
- `transform`: Dönüşüm.

#### Örnekler:

```html
<div class="css-example">CSS Özellikleri Örneği</div>
```

```css
.css-example {
  margin: 10px;
  padding: 20px;
  border: 1px solid black;
  background: #f0f0f0;
  color: #333;
  font-size: 16px;
  font-family: Arial, sans-serif;
  text-align: center;
  display: block;
  position: relative;
  top: 10px;
  right: 20px;
  width: 100px;
  height: 50px;
  max-width: 200px;
  min-width: 50px;
  opacity: 0.8;
  transition: all 0.3s ease;
  transform: rotate(10deg);
}
```

#### Çıktı:

<div class="css-example">CSS Özellikleri Örneği</div>

### Navigasyon Menüsü

- `<nav>`: Navigasyon menüsü oluşturur.
  ```html
  <nav>
    <ul>
      <li><a href="#home">Anasayfa</a></li>
      <li><a href="#about">Hakkında</a></li>
      <li><a href="#contact">İletişim</a></li>
    </ul>
  </nav>
  ```

#### Örnek:

```html
<div id="yanMenu">
  <ul>
    <li><a href="#">AnaSayfa</a></li>
    <li><a href="#">Hakkımızda</a>
      <ul>
        <li><a href="#">Kısa Özgeçmiş</a></li>
        <li><a href="#">Misyonumuz</a></li>
        <li><a href="#">Vizyonumuz</a></li>
      </ul>
    </li>
    <li><a href="#">Ürünlerimiz</a></li>
    <li><a href="#">Kullanıcılar</a>
      <ul>
        <li><a href="#">Kullanıcı Deneyimleri</a></li>
        <li><a href="#">Kullanıcı Önerileri</a></li>
        <li><a href="#">Kullanıcılarla İletişim</a></li>
      </ul>
    </li>
    <li><a href="#">İletişim</a></li>
    <div style="clear:both"></div>
  </ul>
</div>
```

```css
#yanMenu {
  padding: 0px;
}

#yanMenu ul {
  margin: 0px;
  padding: 0px;
  list-style: none;
}

#yanMenu li {
  float: left;
  position: relative;
  width: 150px;
}

#yanMenu li ul {
  display: none;
  position: absolute;
  left: 0px;
  top: 29px;
}

#yanMenu ul li a {
  background-color: pink;
  border: 1px solid red;
  color: red;
  font-weight: bold;
  display: block;
  margin: 0px;
  padding: 2px;
  text-decoration: none;
  line-height: 24px;
  text-align: center;
}

#yanMenu ul li a:hover {
  background-color: white;
  color: gray;
}

#yanMenu li:hover ul {
  display: block;
}
```

#### Çıktı:

<div id="yanMenu">
  <ul>
    <li><a href="#">AnaSayfa</a></li>
    <li><a href="#">Hakkımızda</a>
      <ul>
        <li><a href="#">Kısa Özgeçmiş</a></li>
        <li><a href="#">Misyonumuz</a></li>
        <li><a href="#">Vizyonumuz</a></li>
      </ul>
    </li>
    <li><a href="#">Ürünlerimiz</a></li>
    <li><a href="#">Kullanıcılar</a>
      <ul>
        <li><a href="#">Kullanıcı Deneyimleri</a></li>
        <li><a href="#">Kullanıcı Önerileri</a></li>
        <li><a href="#">Kullanıcılarla İletişim</a></li>
      </ul>
    </li>
    <li><a href="#">İletişim</a></li>
    <div style="clear:both"></div>
  </ul>
</div>

