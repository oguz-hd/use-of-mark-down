# Markdown Rehberi

## Genel Bakış
Neredeyse tüm Markdown uygulamaları, orijinal Markdown tasarım belgesinde belirtilen temel sözdizimini destekler. Markdown işlemcileri arasında küçük farklılıklar ve uyuşmazlıklar olabilir — bunlar mümkün olduğunca satır içinde belirtilmiştir.

## Başlıklar (Headings)
Bir başlık oluşturmak için, bir kelimenin veya ifadenin önüne sayı işareti (`#`) ekleyin. Kullandığınız sayı işareti sayısı başlık seviyesine karşılık gelmelidir. Örneğin, üçüncü seviye bir başlık (`<h3>`) oluşturmak için üç sayı işareti kullanın (örneğin, `### Benim Başlığım`).

| Markdown | HTML | Görünüm |
| :--- | :--- | :--- |
| `# Başlık seviyesi 1` | `<h1>Başlık seviyesi 1</h1>` | Başlık seviyesi 1 |
| `## Başlık seviyesi 2` | `<h2>Başlık seviyesi 2</h2>` | Başlık seviyesi 2 |
| `### Başlık seviyesi 3` | `<h3>Başlık seviyesi 3</h3>` | Başlık seviyesi 3 |
| `#### Başlık seviyesi 4` | `<h4>Başlık seviyesi 4</h4>` | Başlık seviyesi 4 |
| `##### Başlık seviyesi 5` | `<h5>Başlık seviyesi 5</h5>` | Başlık seviyesi 5 |
| `###### Başlık seviyesi 6` | `<h6>Başlık seviyesi 6</h6>` | Başlık seviyesi 6 |

### Alternatif Sözdizimi
Alternatif olarak, metnin altındaki satıra başlık seviyesi 1 için istediğiniz sayıda `==` karakteri veya başlık seviyesi 2 için `--` karakteri ekleyebilirsiniz.

| Markdown | HTML | Görünüm |
| :--- | :--- | :--- |
| `Başlık seviyesi 1`<br>`===============` | `<h1>Başlık seviyesi 1</h1>` | Başlık seviyesi 1 |
| `Başlık seviyesi 2`<br>`---------------` | `<h2>Başlık seviyesi 2</h2>` | Başlık seviyesi 2 |

### Başlıklar İçin En İyi Uygulamalar
Markdown uygulamaları, sayı işaretleri (`#`) ile başlık adı arasında eksik bir boşluğun nasıl ele alınacağı konusunda hemfikir değildir. Uyumluluk için, sayı işaretleri ile başlık adı arasına her zaman bir boşluk koyun.

✅ **Bunu yapın:** `# İşte Bir Başlık`
❌ **Bunu yapmayın:** `#İşte Bir Başlık`

Uyumluluk için başlıktan önce ve sonra boş satırlar bırakmalısınız.

## Paragraflar (Paragraphs)
Paragraf oluşturmak için, bir veya daha fazla metin satırını ayırmak üzere boş bir satır kullanın.

| Markdown | HTML | Görünüm |
| :--- | :--- | :--- |
| `Markdown kullanmayı gerçekten seviyorum.`<br><br>`Sanırım bundan sonra tüm belgelerimi biçimlendirmek için kullanacağım.` | `<p>Markdown kullanmayı gerçekten seviyorum.</p>`<br>`<p>Sanırım bundan sonra tüm belgelerimi biçimlendirmek için kullanacağım.</p>` | Markdown kullanmayı gerçekten seviyorum.<br><br>Sanırım bundan sonra tüm belgelerimi biçimlendirmek için kullanacağım. |

### Paragraflar İçin En İyi Uygulamalar
Paragraf bir liste içinde değilse, paragrafları boşluk veya sekmelerle (tab) girintilemeyin.

✅ **Bunu yapın:** Satırları sola dayalı tutun.
❌ **Bunu yapmayın:** Paragrafların önüne sekme veya boşluk eklemeyin.

## Satır Sonları (Line Breaks)
Bir satır sonu veya yeni satır (`<br>`) oluşturmak için, bir satırı iki veya daha fazla boşlukla bitirin ve ardından enter'a basın.

| Markdown | HTML | Görünüm |
| :--- | :--- | :--- |
| `Bu ilk satır.  `<br>`Ve bu da ikinci satır.` | `<p>Bu ilk satır.<br>`<br>`Ve bu da ikinci satır.</p>` | Bu ilk satır.<br>Ve bu da ikinci satır. |

### Satır Sonları İçin En İyi Uygulamalar
Neredeyse her Markdown uygulamasında satır sonları için iki veya daha fazla boşluk kullanabilirsiniz, ancak bu tartışmalıdır. Bir editörde satır sonundaki boşlukları görmek zordur. Uyumluluk için satır sonunda boşluk bırakmayı veya `<br>` HTML etiketini kullanmayı tercih edebilirsiniz.

## Vurgulama (Emphasis)
Metni kalın veya italik yaparak vurgu ekleyebilirsiniz.

### Kalın (Bold)
Metni kalın yapmak için, bir kelimenin veya ifadenin önüne ve arkasına iki yıldız (`**`) veya iki alt çizgi (`__`) ekleyin.

| Markdown | HTML | Görünüm |
| :--- | :--- | :--- |
| `Sadece **kalın metni** seviyorum.` | `Sadece <strong>kalın metni</strong> seviyorum.` | Sadece **kalın metni** seviyorum. |
| `Sadece __kalın metni__ seviyorum.` | `Sadece <strong>kalın metni</strong> seviyorum.` | Sadece **kalın metni** seviyorum. |

**En İyi Uygulama:** Kelimenin ortasını kalın yapmak için yıldız işaretlerini kullanın.

### İtalik (Italic)
Metni italik yapmak için, bir kelimenin veya ifadenin önüne ve arkasına bir yıldız (`*`) veya bir alt çizgi (`_`) ekleyin.

| Markdown | HTML | Görünüm |
| :--- | :--- | :--- |
| `İtalik metin *harikadır*.` | `İtalik metin <em>harikadır</em>.` | İtalik metin *harikadır*. |
| `İtalik metin _harikadır_.` | `İtalik metin <em>harikadır</em>.` | İtalik metin *harikadır*. |

**En İyi Uygulama:** Kelimenin ortasını italik yapmak için yıldız işaretlerini kullanın.

### Kalın ve İtalik
Metni aynı anda hem kalın hem de italik yapmak için, bir kelimenin veya ifadenin önüne ve arkasına üç yıldız (`***`) veya üç alt çizgi (`___`) ekleyin.

| Markdown | HTML | Görünüm |
| :--- | :--- | :--- |
| `Bu metin ***gerçekten önemli***.` | `Bu metin <em><strong>gerçekten önemli</strong></em>.` | Bu metin ***gerçekten önemli***. |

## Alıntılar (Blockquotes)
Bir alıntı oluşturmak için, bir paragrafın önüne `>` ekleyin.

`> Dorothy, kalesindeki birçok güzel odada onu takip etti.`

### İç İçe Alıntılar
Alıntılar iç içe olabilir. İç içe geçirmek istediğiniz paragrafın önüne `>>` ekleyin.

```markdown
> Dorothy, kalesindeki birçok güzel odada onu takip etti.
>
>> Cadı ona tencere ve tavaları temizlemesini emretti.
```

## Listeler (Lists)
Öğeleri sıralı ve sırasız listeler halinde düzenleyebilirsiniz.

### Sıralı Listeler (Ordered Lists)
Sıralı bir liste oluşturmak için, satır öğelerini sayılar ve ardından noktalarla ekleyin. Sayıların sayısal sırada olması gerekmez, ancak liste bir numarasıyla başlamalıdır.

```markdown
1. İlk öğe
2. İkinci öğe
3. Üçüncü öğe
```

### Sırasız Listeler (Unordered Lists)
Sırasız bir liste oluşturmak için, satır öğelerinin önüne tire (`-`), yıldız (`*`) veya artı (`+`) işaretleri ekleyin.

```markdown
- İlk öğe
- İkinci öğe
- Üçüncü öğe
```

## Kod (Code)
Bir kelimeyi veya ifadeyi kod olarak belirtmek için, onu ters tırnaklar (backticks - `` ` ``) içine alın.

`Komut isteminde `nano` yazın.`

### Kod Blokları (Code Blocks)
Kod blokları oluşturmak için, bloğun her satırını en az dört boşluk veya bir sekme (tab) ile girintileyin. Veya "çitle çevrili" (fenced) kod blokları için üç ters tırnak (```) kullanın.

    <html>
      <head>
      </head>
    </html>

## Yatay Çizgiler (Horizontal Rules)
Bir yatay çizgi oluşturmak için, bir satırda tek başlarına üç veya daha fazla yıldız (`***`), tire (`---`) veya alt çizgi (`___`) kullanın.

```markdown
***
---
_________________
```

## Bağlantılar (Links)
Bir bağlantı oluşturmak için, bağlantı metnini köşeli parantez içine alın (örneğin, `[Duck Duck Go]`) ve hemen ardından URL'yi parantez içine alın (örneğin, `(https://duckduckgo.com)`).

`En sevdiğim arama motoru [Duck Duck Go](https://duckduckgo.com).`

### URL'ler ve E-posta Adresleri
Bir URL'yi veya e-posta adresini hızlıca bağlantıya dönüştürmek için, onu açılı parantez içine alın.

`<https://www.markdownguide.org>`
`<fake@example.com>`

## Görseller (Images)
Bir görsel eklemek için, bir ünlem işareti (`!`), ardından köşeli parantez içinde alt metin (alt text) ve parantez içinde görselin yolu veya URL'sini ekleyin.

`![San Juan Dağları çok güzel](/assets/images/san-juan-mountains.jpg "San Juan Dağları")`

### Görsellere Bağlantı Verme
Bir görsele bağlantı eklemek için, görselin Markdown kodunu köşeli parantez içine alın ve ardından bağlantıyı parantez içinde ekleyin.

`[![Çöldeki eski bir kaya](/assets/images/shiprock.jpg)](https://www.flickr.com)`

## Karakter Kaçışları (Escaping Characters)
Markdown belgesinde metni biçimlendirmek için kullanılan bir karakteri, olduğu gibi (literal) görüntülemek için, karakterin önüne bir ters eğik çizgi (`\`) ekleyin.

`\* Ters eğik çizgi olmadan, bu sırasız bir listede madde işareti olurdu.`

Aşağıdaki karakterleri kaçış (escape) karakteriyle kullanabilirsiniz:
`\`   ters eğik çizgi
`*`   yıldız
`_`   alt çizgi
`{}`  süslü parantezler
`[]`  köşeli parantezler
`()`  parantezler
`#`   diyez (kare) işareti
`+`   artı işareti
`-`   eksi işareti (tire)
`.`   nokta
`!`   ünlem işareti

## HTML
Birçok Markdown uygulaması, Markdown biçimli metin içinde HTML etiketleri kullanmanıza izin verir. Bu, Markdown sözdizimi yerine belirli HTML etiketlerini tercih ediyorsanız yararlıdır.

`Bu **kelime** kalın. Bu <em>kelime</em> italik.`
