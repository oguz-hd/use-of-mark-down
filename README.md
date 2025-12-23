Harika. Senin için tüm bu metni, GitHub'ın `README.md` dosyasında kusursuz görünecek şekilde, tüm kod bloklarını, tabloları ve vurgulamaları düzelterek **tek parça** haline getirdim.

Bunu kopyalayıp `README.md` dosyanın içine yapıştırdığında, tam bir "Markdown Kullanım Kılavuzu" gibi görünecek.

Aşağıdaki kod bloğunu **en üstten en alta kadar (Footer dahil)** kopyala ve yapıştır:

```markdown
# Temel Markdown Sözdizimi (Basic Syntax)

Bu belge, orijinal Markdown tasarım belgesinde belirtilen temel Markdown öğelerini açıklar ve örneklendirir.

## Genel Bakış
Neredeyse tüm Markdown uygulamaları, orijinal tasarım belgesinde belirtilen temel sözdizimini destekler. Markdown işlemcileri arasında küçük farklılıklar olabilir; bunlar mümkün olduğunca satır aralarında belirtilmiştir.

---

## Başlıklar (Headings)
Bir başlık oluşturmak için, bir kelimenin veya ifadenin önüne sayı işareti (`#`) ekleyin. Kullandığınız sayı işareti sayısı, başlık seviyesine karşılık gelmelidir. Örneğin, üçüncü seviye bir başlık (`<h3>`) oluşturmak için üç sayı işareti kullanın (örn: `### Başlığım`).

### Markdown Kodu ve Görünümü

```markdown
# Başlık Seviyesi 1
## Başlık Seviyesi 2
### Başlık Seviyesi 3
#### Başlık Seviyesi 4
##### Başlık Seviyesi 5
###### Başlık Seviyesi 6

```

### Alternatif Sözdizimi

Alternatif olarak, metnin altındaki satıra 1. seviye başlık için istediğiniz sayıda eşittir işareti (`==`) veya 2. seviye başlık için tire işareti (`--`) ekleyebilirsiniz.

```markdown
Başlık Seviyesi 1
===============

Başlık Seviyesi 2
---------------

```

### Başlıklar İçin En İyi Uygulamalar

Markdown uygulamaları, sayı işaretleri (`#`) ile başlık adı arasında boşluk olup olmayacağı konusunda hemfikir değildir. Uyumluluk için, sayı işaretleri ile başlık adı arasına **her zaman bir boşluk koyun**.

| ✅ Bunu Yapın | ❌ Bunu Yapmayın |
| --- | --- |
| `# İşte Bir Başlık` | `#İşte Bir Başlık` |

Ayrıca uyumluluk için başlıktan önce ve sonra boş satırlar bırakmalısınız.

| ✅ Bunu Yapın | ❌ Bunu Yapmayın |
| --- | --- |
| Öncesinde boş bir satır bırakın...<br>

<br>

<br>`# Başlık`<br>

<br>

<br>...ve sonrasında da. | Boş satırlar olmadan bu düzgün görünmeyebilir.<br>

<br>`# Başlık`<br>

<br>Bunu yapmayın! |

---

## Paragraflar (Paragraphs)

Paragraf oluşturmak için, bir veya daha fazla metin satırını ayırmak üzere boş bir satır kullanın.

**Markdown Kodu:**

```text
Markdown kullanmayı gerçekten seviyorum.

Sanırım bundan sonra tüm belgelerimi biçimlendirmek için onu kullanacağım.

```

**Görünüm:**
Markdown kullanmayı gerçekten seviyorum.

Sanırım bundan sonra tüm belgelerimi biçimlendirmek için onu kullanacağım.

### Paragraflar İçin En İyi Uygulamalar

Paragraf bir listenin içinde değilse, paragrafları boşluk veya sekmelerle (tab) girintilemeyin.

| ✅ Bunu Yapın | ❌ Bunu Yapmayın |
| --- | --- |
| Paragraflarınızın önüne sekme veya boşluk koymayın.<br>

<br>

<br>Satırları bu şekilde sola hizalı tutun. |     Bu, beklenmedik biçimlendirme sorunlarına neden olabilir.<br>

<br>

<br>  Paragrafların önüne sekme veya boşluk eklemeyin. |

---

## Satır Sonları (Line Breaks)

Bir satır sonu veya yeni satır (`<br>`) oluşturmak için, bir satırı **iki veya daha fazla boşlukla** bitirin ve ardından enter tuşuna basın.

**Markdown Kodu:**

```text
Bu ilk satır.  
Ve bu da ikinci satır.

```

**Görünüm:**
Bu ilk satır.

Ve bu da ikinci satır.

### Satır Sonları İçin En İyi Uygulamalar

Hemen hemen her Markdown uygulamasında satır sonları için iki veya daha fazla boşluk (genellikle "sondaki boşluk" olarak adlandırılır) kullanabilirsiniz, ancak bu tartışmalı bir konudur. Bir editörde sondaki boşluğu görmek zordur ve birçok kişi yanlışlıkla veya bilerek her cümleden sonra iki boşluk bırakır. Bu nedenle, satır sonları için sondaki boşluktan başka bir şey kullanmak isteyebilirsiniz. Markdown uygulamanız HTML'yi destekliyorsa, `<br>` HTML etiketini kullanabilirsiniz.

Uyumluluk için, satırın sonunda sondaki boşluğu veya `<br>` HTML etiketini kullanın.

| ✅ Bunu Yapın | ❌ Bunu Yapmayın |
| --- | --- |
| İki boşlukla biten ilk satır.  <br>

<br>Ve sonraki satır.<br>

<br>

<br>HTML etiketiyle biten ilk satır.<br>

<br>

<br>Ve sonraki satır. | Ters eğik çizgiyle biten ilk satır.<br>Ve sonraki satır.<br>

<br>

<br>Sonunda hiçbir şey olmayan ilk satır.<br>

<br>Ve sonraki satır. |

---

## Vurgu (Emphasis)

Metni kalın veya italik yaparak vurgu ekleyebilirsiniz.

### Kalın (Bold)

Metni kalın yapmak için, bir kelime veya ifadenin önüne ve arkasına iki yıldız (`**`) veya alt çizgi (`__`) ekleyin. Vurgu için bir kelimenin ortasını kalınlaştırmak isterseniz, harflerin etrafına boşluk bırakmadan iki yıldız ekleyin.

**Örnekler:**

* `Ben **kalın metni** seviyorum.` -> Ben **kalın metni** seviyorum.
* `Ben __kalın metni__ seviyorum.` -> Ben **kalın metni** seviyorum.
* `Aşk**tır**kalın` -> Aşk**tır**kalın

#### Kalın İçin En İyi Uygulamalar

Markdown uygulamaları, bir kelimenin ortasındaki alt çizgileri nasıl ele alacakları konusunda hemfikir değildir. Uyumluluk için, bir kelimenin ortasını kalınlaştırmak istediğinizde **yıldız işaretleri** kullanın.

| ✅ Bunu Yapın | ❌ Bunu Yapmayın |
| --- | --- |
| `Aşk**tır**kalın` | `Aşk__tır__kalın` |

### İtalik (Italic)

Metni italik yapmak için, bir kelime veya ifadenin önüne ve arkasına bir yıldız (`*`) veya alt çizgi (`_`) ekleyin.

**Örnekler:**

* `İtalik metin *harikadır*.` -> İtalik metin *harikadır*.
* `İtalik metin _harikadır_.` -> İtalik metin *harikadır*.
* `Bir*kedi*miyav` -> Bir*kedi*miyav

#### İtalik İçin En İyi Uygulamalar

Kelime ortası için yine **yıldız işaretleri** kullanın.

| ✅ Bunu Yapın | ❌ Bunu Yapmayın |
| --- | --- |
| `Bir*kedi*miyav` | `Bir_kedi_miyav` |

### Kalın ve İtalik

Aynı anda hem kalın hem de italik yapmak için üç yıldız (`***`) veya alt çizgi (`___`) kullanın.

**Örnekler:**

* `Bu metin ***gerçekten önemli***.` -> Bu metin ***gerçekten önemli***.
* `Bu metin ___gerçekten önemli___.` -> Bu metin ***gerçekten önemli***.
* `Bu metin __*gerçekten önemli*__.` -> Bu metin ***gerçekten önemli***.
* `Bu metin **_gerçekten önemli_**.` -> Bu metin ***gerçekten önemli***.

#### Kalın ve İtalik İçin En İyi Uygulamalar

Kelime ortası vurgusu için yıldız kullanın.

| ✅ Bunu Yapın | ❌ Bunu Yapmayın |
| --- | --- |
| `Bu gerçekten***çok***önemli bir metin.` | `Bu gerçekten___çok___önemli bir metin.` |

---

## Alıntılar (Blockquotes)

Bir alıntı oluşturmak için paragrafın önüne `>` ekleyin.

> Dorothy, kalesindeki birçok güzel odada onu takip etti.

### Çok Paragraflı Alıntılar

Paragraflar arasındaki boş satırlara `>` ekleyin.

> Dorothy, kalesindeki birçok güzel odada onu takip etti.
> Cadı ona tencere ve tavaları temizlemesini, yeri süpürmesini ve ateşi odunla beslemesini emretti.

### İç İçe Alıntılar (Nested Blockquotes)

İç içe yerleştirmek istediğiniz paragrafın önüne `>>` ekleyin.

> Dorothy, kalesindeki birçok güzel odada onu takip etti.
> > Cadı ona tencere ve tavaları temizlemesini, yeri süpürmesini ve ateşi odunla beslemesini emretti.
> 
> 

### Diğer Öğelerle Alıntılar

Alıntılar diğer Markdown öğelerini içerebilir.

> #### Çeyrek sonuçları harika görünüyor!
> 
> 
> * Gelir tablonun dışına çıktı.
> * Karlar hiç olmadığı kadar yüksek.
> 
> 
> *Her şey* **plana** göre gidiyor.

### Alıntılar İçin En İyi Uygulamalar

Uyumluluk için, alıntılardan önce ve sonra boş satırlar bırakın.

---

## Listeler (Lists)

### Sıralı Listeler (Ordered Lists)

Sıralı liste oluşturmak için, sayıların ardından nokta gelen satır öğeleri ekleyin. Sayıların sayısal sırada olması gerekmez, ancak liste **bir (1)** sayısı ile başlamalıdır.

**Markdown:**

```markdown
1. İlk öğe
2. İkinci öğe
3. Üçüncü öğe
4. Dördüncü öğe

```

**Görünüm:**

1. İlk öğe
2. İkinci öğe
3. Üçüncü öğe
4. Dördüncü öğe

**Sıralı Olmayan Sayılarla da Çalışır:**

```markdown
1. İlk öğe
1. İkinci öğe
1. Üçüncü öğe

```

**Görünüm:**

1. İlk öğe
2. İkinci öğe
3. Üçüncü öğe

#### Sıralı Listeler İçin En İyi Uygulamalar

Uyumluluk için sadece **nokta** kullanın. Parantez `)` kullanmayın.

| ✅ Bunu Yapın | ❌ Bunu Yapmayın |
| --- | --- |
| `1. İlk öğe` | `1) İlk öğe` |

### Sırasız Listeler (Unordered Lists)

Sırasız liste oluşturmak için satır öğelerinin önüne tire (`-`), yıldız (`*`) veya artı (`+`) işaretleri ekleyin.

**Örnek:**

```markdown
- İlk öğe
- İkinci öğe
- Üçüncü öğe

```

**Görünüm:**

* İlk öğe
* İkinci öğe
* Üçüncü öğe

#### Sırasız Listeler İçin En İyi Uygulamalar

Aynı listede farklı işaretleyicileri karıştırmayın.

| ✅ Bunu Yapın | ❌ Bunu Yapmayın |
| --- | --- |
| `- İlk öğe`<br>

<br>`- İkinci öğe` | `+ İlk öğe`<br>

<br>`* İkinci öğe` |

### Listelere Öğe Ekleme

Listenin sürekliliğini koruyarak başka bir öğe eklemek için, öğeyi **dört boşluk veya bir sekme** kadar girintileyin.

**Paragraf Ekleme:**

* Bu ilk liste öğesidir.
* İşte ikinci liste öğesi.
İkinci liste öğesinin altına başka bir paragraf eklemem gerekiyor.
* Ve işte üçüncü liste öğesi.

**Alıntı Ekleme:**

* Bu ilk liste öğesidir.
* İşte ikinci liste öğesi.
> İkinci liste öğesinin altında bir alıntı harika görünürdü.


* Ve işte üçüncü liste öğesi.

**Kod Bloğu Ekleme (8 boşluk girintilenir):**

1. Dosyayı açın.
2. 21. satırda aşağıdaki kod bloğunu bulun:
<html>
<head>
<title>Test</title>
</head>


3. Başlığı web sitenizin adıyla eşleşecek şekilde güncelleyin.

---

## Kod (Code)

Bir kelimeyi veya ifadeyi kod olarak belirtmek için, onu ters tırnak (backtick) içine alın (```).

**Örnek:**
Komut isteminde `nano` yazın.

### Ters Tırnakları Kaçırmak (Escaping Backticks)

Göstermek istediğiniz kodun içinde ters tırnak varsa, kelimeyi çift ters tırnak içine alın (`     ` ` `     `).

**Örnek:**
`Markdown dosyanızda `code` kullanın.`

### Kod Blokları

Kod blokları oluşturmak için, bloğun her satırını en az **dört boşluk veya bir sekme** kadar girintileyin.

```
<html>
  <head>
  </head>
</html>

```

---

## Yatay Çizgiler (Horizontal Rules)

Yatay çizgi oluşturmak için, tek başına bir satırda üç veya daha fazla yıldız (`***`), tire (`---`) veya alt çizgi (`___`) kullanın.

---

---

---

### Yatay Çizgiler İçin En İyi Uygulamalar

Uyumluluk için, yatay çizgilerden önce ve sonra boş satırlar bırakın.

---

## Bağlantılar (Links)

Bir bağlantı oluşturmak için, bağlantı metnini köşeli parantez içine alın (örn: `[Duck Duck Go]`) ve ardından URL'yi parantez içinde hemen yanına ekleyin (örn: `(https://duckduckgo.com)`).

**Örnek:**
En sevdiğim arama motoru [Duck Duck Go](https://duckduckgo.com).

### Başlık Ekleme (Titles)

İsteğe bağlı olarak bir bağlantı için başlık ekleyebilirsiniz. Bu, kullanıcı bağlantının üzerine geldiğinde bir ipucu olarak görünür. URL'den sonra tırnak işaretleri içinde ekleyin.

**Kod:**
`[Duck Duck Go](https://duckduckgo.com "Gizlilik için en iyi arama motoru")`

### URL ve E-posta Adresleri

Bir URL'yi veya e-posta adresini hızlıca bağlantıya dönüştürmek için açılı parantez içine alın.

* [https://www.markdownguide.org](https://www.markdownguide.org)
* [fake@example.com](mailto:fake@example.com)

### Bağlantıları Biçimlendirme

Bağlantıları **vurgulamak** için köşeli parantez ve normal parantezlerin önüne ve arkasına yıldız ekleyin.

* **[EFF](https://eff.org)**'yi desteklemeyi seviyorum.
* Bu *[Markdown Rehberi](https://www.markdownguide.org)*.

### Referans Tarzı Bağlantılar (Reference-style Links)

URL'lerin okunmasını kolaylaştıran özel bir bağlantı türüdür. İki parçadan oluşur.

**Birinci Kısım (Metin İçi):**
`[hobbit-kovuğu][1]`

**İkinci Kısım (Belgenin Herhangi Bir Yeri):**
`[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit yaşam tarzları"`

**Örnek Kullanım:**
Topraktaki bir oyukta bir hobbit yaşardı. Solucan uçlarıyla dolu ve yosun kokan iğrenç, kirli, ıslak bir oyuk değil, ne de oturacak veya yiyecek bir şeyi olmayan kuru, çıplak, kumlu bir oyuk: bu bir [hobbit-kovuğu](https://en.wikipedia.org/wiki/Hobbit#Lifestyle) idi ve bu da konfor demektir.

### Bağlantılar İçin En İyi Uygulamalar

URL'nin ortasındaki boşlukları `%20` ile kodlayın.

| ✅ Bunu Yapın | ❌ Bunu Yapmayın |
| --- | --- |
| `[bağlantı](https://www.example.com/my%20great%20page)` | `[bağlantı](https://www.example.com/my great page)` |

---

## Resimler (Images)

Resim eklemek için, bir ünlem işareti (`!`), ardından köşeli parantez içinde alt metin (alt text) ve parantez içinde resmin yolu veya URL'si gelir.

**Kod:**
`![Linux maskotu Tux](https://github.com/oguz-hd/bmyo-projects/assets/placeholder_tux.png "Tux")`

*(Not: Yukarıdaki sadece bir örnektir, geçerli bir resim URL'si kullanmalısınız)*

### Resimleri Bağlantılandırma

Bir resme bağlantı eklemek için, resim için olan Markdown kodunu köşeli parantez içine alın ve ardından bağlantıyı parantez içinde ekleyin.

`[![Çöldeki eski bir kaya](https://via.placeholder.com/150 "Örnek Resim")](https://www.flickr.com)`

---

## Karakterleri Kaçırma (Escaping Characters)

Markdown belgesinde biçimlendirme için kullanılan bir karakteri, kelime anlamıyla (literal) göstermek için karakterin önüne ters eğik çizgi (`\`) ekleyin.

* Ters eğik çizgi olmadan, bu sırasız bir listede madde işareti olurdu.

### Kaçırılabilen Karakterler

Aşağıdaki karakterleri kaçırmak için ters eğik çizgi kullanabilirsiniz:

* Ters eğik çizgi: `\`
* Ters tırnak: ```
* Yıldız: `*`
* Alt çizgi: `_`
* Süslü parantez: `{ }`
* Köşeli parantez: `[ ]`
* Açılı parantez: `< >`
* Parantez: `( )`
* Sayı işareti: `#`
* Artı işareti: `+`
* Eksi işareti (tire): `-`
* Nokta: `.`
* Ünlem işareti: `!`
* Dikey çizgi: `|`

---

## HTML

Birçok Markdown uygulaması, Markdown formatlı metin içinde HTML etiketlerini kullanmanıza izin verir. Bu, rengi değiştirmek veya resim genişliğini ayarlamak gibi durumlarda faydalıdır.

**Kod:**
`Bu **kelime** kalın. Bu <em>kelime</em> italik.`

**Görünüm:**
Bu **kelime** kalın. Bu <em>kelime</em> italik.

### HTML İçin En İyi Uygulamalar

Güvenlik nedenleriyle, tüm Markdown uygulamaları HTML'yi desteklemez. Şüpheye düştüğünüzde uygulamanızın belgelerine bakın.

`<div>`, `<table>`, `<pre>`, ve `<p>` gibi blok düzeyindeki HTML öğelerini çevreleyen içerikten ayırmak için boş satırlar kullanın. Etiketleri sekme veya boşluklarla girintilememeye çalışın.

---

*Hazırlayanlar: Oğuz & Kerem | Ege Üniversitesi Bergama MYO*

```

```