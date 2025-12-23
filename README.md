# Markdown Kullanım Rehberi

Bu belge, Markdown formatını ve `.md` dosyalarının kullanımını açıklayan kapsamlı bir rehberdir.

## Markdown ve .md Nedir?

### Markdown Nedir?
Markdown, 2004 yılında John Gruber tarafından oluşturulan hafif bir işaretleme dilidir. Temel amacı, insanların kolayca okuyup yazabileceği bir **düz metin formatı** sağlamak ve gerektiğinde bunu yapısal olarak geçerli HTML'e dönüştürebilmektir. Word gibi "Ne Görüyorsan Onu Alırsın" (WYSIWYG) editörlerinin aksine, Markdown biçimlendirme için karmaşık menüler yerine basit semboller (örneğin `#`, `*`, `-`) kullanır.

### .md Dosyası Nedir?
`.md` (veya `.markdown`), Markdown sözdizimi ile yazılmış metin dosyalarının uzantısıdır. "MD" kısaltması "Markdown Documentation" (Markdown Dokümantasyonu) anlamına gelir. Bu dosyalar Notepad, TextEdit veya VS Code gibi herhangi bir metin editörü ile açılabilir ve düzenlenebilir.

### Ne İçin Kullanılır?
*   **Dokümantasyon:** Projelerin `README.md` dosyaları, kurulum rehberleri ve wiki sayfaları.
*   **Web İçeriği:** Blog gönderileri, statik web siteleri ve forum mesajları.
*   **Not Alma:** Hızlı ve düzenli not tutma uygulamaları (Örn: Obsidian, Notion).
*   **Yazılım Geliştirme:** GitHub, GitLab gibi platformlarda proje açıklamaları ve tartışmalar.

---

## Temel Sözdizimi (Basic Syntax)

Aşağıda, orijinal Markdown tasarım belgesinde belirtilen temel Markdown öğeleri yer almaktadır.

### Başlıklar (Headings)
Bir başlık oluşturmak için, kelime veya ifadenin önüne sayı işareti (`#`) ekleyin. Kullandığınız sayı işareti adedi, başlık seviyesine karşılık gelmelidir. Örneğin, seviye 3 başlık (`<h3>`) için üç adet sayı işareti kullanın.

| Markdown | HTML |
| :--- | :--- |
| `# Başlık seviyesi 1` | `<h1>Başlık seviyesi 1</h1>` |
| `## Başlık seviyesi 2` | `<h2>Başlık seviyesi 2</h2>` |
| `### Başlık seviyesi 3` | `<h3>Başlık seviyesi 3</h3>` |
| `#### Başlık seviyesi 4` | `<h4>Başlık seviyesi 4</h4>` |
| `##### Başlık seviyesi 5` | `<h5>Başlık seviyesi 5</h5>` |
| `###### Başlık seviyesi 6` | `<h6>Başlık seviyesi 6</h6>` |

**Alternatif Sözdizimi:**
Metnin altına `==` ekleyerek Seviye 1 başlık, `--` ekleyerek Seviye 2 başlık oluşturabilirsiniz.

```markdown
Başlık Seviyesi 1
===============

Başlık Seviyesi 2
---------------
```

> **En İyi Uygulama:** Sayı işaretleri (`#`) ile başlık metni arasında her zaman bir boşluk bırakın (Örn: `# Başlık`). Ayrıca, uyumluluk için başlıktan önce ve sonra birer boş satır bırakmanız önerilir.

---

### Paragraflar (Paragraphs)
Paragraf oluşturmak için, bir veya daha fazla metin satırını ayırmak üzere boş bir satır kullanın.

**Markdown:**
```markdown
Markdown kullanmayı gerçekten seviyorum.

Sanırım bundan sonra tüm belgelerimi biçimlendirmek için onu kullanacağım.
```

**HTML Karşılığı:** `<p>Markdown kullanmayı gerçekten seviyorum.</p>`

> **Not:** Paragrafları boşluk veya sekmelerle (tab) girintilemeyin.

---

### Satır Sonları (Line Breaks)
Bir satır sonu veya yeni satır (`<br>`) oluşturmak için, satırı **iki veya daha fazla boşluk** ile bitirin ve ardından Enter'a basın.

**Markdown:**
```markdown
Bu ilk satır.  
Ve bu da ikinci satır.
```

**Alternatif:** HTML ` <br> ` etiketini de kullanabilirsiniz.

```markdown
İlk satır.<br>
İkinci satır.
```

---

### Vurgulama (Emphasis)

#### Kalın (Bold)
Metni kalın yapmak için kelime veya ifadenin önüne ve arkasına iki yıldız (`**`) veya iki alt çizgi (`__`) ekleyin.

| Markdown | HTML | Çıktı |
| :--- | :--- | :--- |
| `**kalın metin**` | `<strong>kalın metin</strong>` | **kalın metin** |
| `__kalın metin__` | `<strong>kalın metin</strong>` | __kalın metin__ |

> **En İyi Uygulama:** Kelime ortasında vurgulama yapacaksanız yıldız (`**`) kullanın.

#### İtalik (Italic)
Metni italik yapmak için kelime veya ifadenin önüne ve arkasına bir yıldız (`*`) veya bir alt çizgi (`_`) ekleyin.

| Markdown | HTML | Çıktı |
| :--- | :--- | :--- |
| `*italik metin*` | `<em>italik metin</em>` | *italik metin* |
| `_italik metin_` | `<em>italik metin</em>` | _italik metin_ |

#### Kalın ve İtalik
Aynı anda hem kalın hem italik yapmak için üç yıldız (`***`) veya alt çizgi (`___`) kullanın.

`***Bu metin gerçekten çok önemli***` -> ***Bu metin gerçekten çok önemli***

---

### Alıntılar (Blockquotes)
Bir alıntı oluşturmak için paragrafın önüne `>` ekleyin.

```markdown
> Dorothy kalesindeki birçok güzel odada onu takip etti.
```

**Çıktı:**
> Dorothy kalesindeki birçok güzel odada onu takip etti.

**İç İçe Alıntılar:**
```markdown
> Ana alıntı.
>
>> İç içe geçmiş alıntı.
```

---

### Listeler (Lists)

#### Sıralı Listeler (Ordered Lists)
Sayılar ve ardından nokta ekleyerek sıralı liste oluşturabilirsiniz. Sayıların sırayla gitmesi zorunlu değildir, ancak 1 ile başlaması önerilir.

```markdown
1. İlk öğe
2. İkinci öğe
3. Üçüncü öğe
```

**Çıktı:**
1. İlk öğe
2. İkinci öğe
3. Üçüncü öğe

#### Sırasız Listeler (Unordered Lists)
Tire (`-`), yıldız (`*`) veya artı (`+`) işaretlerini kullanarak sırasız liste oluşturabilirsiniz.

```markdown
- İlk öğe
- İkinci öğe
- Üçüncü öğe
```

**Çıktı:**
- İlk öğe
- İkinci öğe
- Üçüncü öğe

#### Liste İçinde Öğe Ekleme
Listenin devamlılığını bozmadan paragraf veya başka öğeler eklemek için, öğeyi **dört boşluk** veya **bir tab** kadar girintileyin.

```markdown
* Birinci liste maddesi.
* İkinci liste maddesi.

    İkinci maddenin altına bir paragraf eklemek istiyorum.

* Üçüncü liste maddesi.
```

---

### Kod (Code)

#### Satır İçi Kod
Bir kelimeyi kod olarak belirtmek için ters tırnak (backticks `` ` ``) içine alın.

`Komut satırına ``nano`` yazın.` -> Komut satırına `nano` yazın.

#### Kod Blokları
Kod blokları oluşturmak için her satırı en az dört boşluk veya bir tab ile girintileyin. Alternatif ve yaygın yöntem olarak "fenced code blocks" (çitli kod blokları) kullanabilirsiniz (üç ters tırnak ```).

    <html>
      <head>
      </head>
    </html>

---

### Yatay Çizgiler (Horizontal Rules)
Bir yatay çizgi oluşturmak için, tek bir satırda üç veya daha fazla yıldız (`***`), tire (`---`) veya alt çizgi (`___`) kullanın.

```markdown
***
---
___
```

**Çıktı:**

---

### Bağlantılar (Links)
Bağlantı metnini köşeli parantez `[ ]` içine, URL'yi ise hemen ardından parantez `( )` içine alın.

```markdown
Favori arama motorum [Duck Duck Go](https://duckduckgo.com).
```

**Çıktı:**
Favori arama motorum [Duck Duck Go](https://duckduckgo.com).

**Başlık Ekleme:**
URL'den sonra tırnak işareti içinde başlık ekleyebilirsiniz (imleç üzerine gelince görünür).
`[Duck Duck Go](https://duckduckgo.com "En iyi arama motoru")`

**Otomatik URL:**
URL'yi açılı parantez içine alarak tıklanabilir yapabilirsiniz: `<https://www.markdownguide.org>`

---

### Görseller (Images)
Resim eklemek için bağlantı formatına benzer bir yapı kullanılır, ancak en başa ünlem işareti (`!`) eklenir.

`![Alt Metin](resim-yolu-veya-url.jpg "Opsiyonel Başlık")`

**Örnek:**
```markdown
![Linux Maskotu](/assets/images/tux.png)
```

**Resme Bağlantı Verme:**
Resim kodunu köşeli parantez içine alıp, ardından bağlantı URL'sini parantez içinde ekleyin.
`[![Resim Açıklaması](resim.jpg)](http://baglanti-adresi.com)`

---

### Karakter Kaçışları (Escaping Characters)
Markdown formatlamasında kullanılan özel karakterleri (örneğin `*` veya `#`) normal metin olarak göstermek isterseniz, önüne ters eğik çizgi (`\`) koyun.

`\* Bu bir madde işareti değildir.` -> * Bu bir madde işareti değildir.

Kaçış yapılabilen karakterler: `\`, `` ` ``, `*`, `_`, `{}`, `[]`, `()`, `#`, `+`, `-`, `.`, `!`, `|`

---

### HTML Kullanımı
Markdown içerisinde HTML etiketleri de kullanabilirsiniz.

```markdown
Bu **kalın** kelime. Bu <em>italik</em> kelime.
```

---

