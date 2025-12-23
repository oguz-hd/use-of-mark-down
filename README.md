Çok haklısın, şimdi tam olarak anladım. Sen **"Markdown'ı anlatan Markdown dosyasının kaynak kodunu"** istiyorsun. Yani sen bunu kopyalayıp yapıştırdığında, GitHub'da "Başlık nasıl yapılır", "Kalın yazı nasıl yazılır" gibi kuralları hem **kod** hem de **görüntü** olarak sunan bir rehber oluşacak.

Aşağıdaki **koyu gri kutunun içindeki her şeyi** (en üstten en alta kadar) kopyala. GitHub'daki `README.md` dosyanın içini tamamen sil ve bunu yapıştır. Kaydettiğinde (Commit), tam istediğin gibi "Markdown Kullanım Rehberi" sayfası oluşacak.

```markdown
# Temel Markdown Sözdizimi (Basic Syntax)

Bu belge, orijinal Markdown tasarım belgesinde belirtilen temel Markdown öğelerini açıklar ve örneklendirir.

## Genel Bakış
Neredeyse tüm Markdown uygulamaları, orijinal tasarım belgesinde belirtilen temel sözdizimini destekler. Markdown işlemcileri arasında küçük farklılıklar olabilir; bunlar mümkün olduğunca satır aralarında belirtilmiştir.

---

## 1. Başlıklar (Headings)
Bir başlık oluşturmak için, bir kelimenin veya ifadenin önüne sayı işareti (`#`) ekleyin. Kullandığınız sayı işareti sayısı, başlık seviyesine karşılık gelmelidir.

### Markdown Kodu
```markdown
# Başlık Seviyesi 1
## Başlık Seviyesi 2
### Başlık Seviyesi 3
#### Başlık Seviyesi 4
##### Başlık Seviyesi 5
###### Başlık Seviyesi 6

```

### Önizleme (Rendered Output)

# Başlık Seviyesi 1

## Başlık Seviyesi 2

### Başlık Seviyesi 3

#### Başlık Seviyesi 4

##### Başlık Seviyesi 5

###### Başlık Seviyesi 6

### Alternatif Sözdizimi

Alternatif olarak, metnin altındaki satıra eşittir (`==`) veya tire (`--`) işareti ekleyebilirsiniz.

```markdown
Başlık Seviyesi 1
===============

Başlık Seviyesi 2
---------------

```

### Başlıklar İçin En İyi Uygulamalar (Best Practices)

Uyumluluk için `#` işareti ile metin arasında **her zaman boşluk bırakın**.

| ✅ Bunu Yapın | ❌ Bunu Yapmayın |
| --- | --- |
| `# Başlık` | `#Başlık` |

---

## 2. Paragraflar (Paragraphs)

Paragraf oluşturmak için, satırları ayırmak üzere boş bir satır kullanın.

### Markdown Kodu

```markdown
Markdown kullanmayı gerçekten seviyorum.

Sanırım bundan sonra tüm belgelerimi biçimlendirmek için onu kullanacağım.

```

### Önizleme

Markdown kullanmayı gerçekten seviyorum.

Sanırım bundan sonra tüm belgelerimi biçimlendirmek için onu kullanacağım.

### Paragraf En İyi Uygulamalar

Paragrafları boşluk veya tab ile girintilemeyin.

| ✅ Bunu Yapın | ❌ Bunu Yapmayın |
| --- | --- |
| Sola hizalı yazın. |     Girintili yazmayın. |

---

## 3. Satır Sonları (Line Breaks)

Bir alt satıra geçmek için (`<br>`), satırın sonuna **iki boşluk** koyun ve Enter'a basın.

### Markdown Kodu

```markdown
Bu ilk satır.  
Ve bu da ikinci satır.

```

### Önizleme

Bu ilk satır.

Ve bu da ikinci satır.

---

## 4. Vurgu (Emphasis)

### Kalın (Bold)

Metni kalın yapmak için `**` veya `__` kullanın.

### Markdown Kodu

```markdown
Ben **kalın metni** seviyorum.

```

### Önizleme

Ben **kalın metni** seviyorum.

### İtalik (Italic)

Metni italik yapmak için `*` veya `_` kullanın.

### Markdown Kodu

```markdown
İtalik metin *harikadır*.

```

### Önizleme

İtalik metin *harikadır*.

### Kalın ve İtalik

İkisini aynı anda kullanmak için `***` kullanın.

### Markdown Kodu

```markdown
Bu metin ***gerçekten önemli***.

```

### Önizleme

Bu metin ***gerçekten önemli***.

---

## 5. Alıntılar (Blockquotes)

Bir alıntı oluşturmak için `>` işaretini kullanın.

### Markdown Kodu

```markdown
> Dorothy, kalesindeki birçok güzel odada onu takip etti.

```

### Önizleme

> Dorothy, kalesindeki birçok güzel odada onu takip etti.

### İç İçe Alıntılar

```markdown
> Ana alıntı.
>> İçteki alıntı.

```

### Önizleme

> Ana alıntı.
> > İçteki alıntı.
> 
> 

---

## 6. Listeler (Lists)

### Sıralı Listeler (Ordered Lists)

Sayı ve nokta kullanarak oluşturulur.

### Markdown Kodu

```markdown
1. İlk öğe
2. İkinci öğe
3. Üçüncü öğe

```

### Önizleme

1. İlk öğe
2. İkinci öğe
3. Üçüncü öğe

### Sırasız Listeler (Unordered Lists)

Tire (`-`), yıldız (`*`) veya artı (`+`) işareti kullanılır.

### Markdown Kodu

```markdown
- Süt
- Yumurta
- Ekmek

```

### Önizleme

* Süt
* Yumurta
* Ekmek

---

## 7. Kod (Code)

### Satır İçi Kod

Metin içinde kod belirtmek için ters tırnak (backtick) kullanın: ```

### Markdown Kodu

```markdown
Komut satırına `nano` yazın.

```

### Önizleme

Komut satırına `nano` yazın.

### Kod Blokları

Çok satırlı kodlar için üç ters tırnak kullanın: `````

### Markdown Kodu

```
```
<html>
  <head>
  </head>
</html>
```

```

### Önizleme

```html
<html>
  <head>
  </head>
</html>

```

---

## 8. Yatay Çizgiler (Horizontal Rules)

Sayfayı bölmek için üç adet tire veya yıldız kullanın.

### Markdown Kodu

```markdown
---
***

```

### Önizleme

---

---

## 9. Bağlantılar (Links)

Metni köşeli parantez `[]`, linki normal parantez `()` içine yazın.

### Markdown Kodu

```markdown
En sevdiğim site [Google](https://google.com).

```

### Önizleme

En sevdiğim site [Google](https://google.com).

### Referans Tarzı Bağlantılar

Kodun temiz görünmesi için linkleri aşağıda tanımlayabilirsiniz.

### Markdown Kodu

```markdown
Bu bir [referans][1] örneğidir.

[1]: https://en.wikipedia.org "Wiki"

```

### Önizleme

Bu bir [referans](https://www.google.com/search?q=%5Bhttps://en.wikipedia.org%5D(https://en.wikipedia.org)) örneğidir.

---

## 10. Resimler (Images)

Link yapısının başına ünlem `!` işareti konur.

### Markdown Kodu

```markdown
![Alternatif Metin](https://github.com/fluidicon.png)

```

### Önizleme

---

## 11. Karakterleri Kaçırma (Escaping)

Markdown karakterlerini yazı olarak kullanmak için ters eğik çizgi `\` kullanın.

### Markdown Kodu

```markdown
\* Bu bir liste maddesi değildir.

```

### Önizleme

* Bu bir liste maddesi değildir.

---

## 12. HTML Kullanımı

Markdown içinde HTML etiketleri de kullanılabilir.

### Markdown Kodu

```markdown
Bu kelime <b>kalın</b> yazıldı.

```

### Önizleme

Bu kelime <b>kalın</b> yazıldı.

---

# Referanslar

Bu çalışma aşağıdaki kaynaklardan derlenmiştir:

* [Markdown Guide - Basic Syntax](https://www.markdownguide.org/basic-syntax/)
* [DataCamp - What is YAML?](https://www.datacamp.com/blog/what-is-yaml)
* [Spacelift - YAML Guide](https://spacelift.io/blog/yaml)

```

```