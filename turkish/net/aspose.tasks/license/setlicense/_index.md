---
title: "License.SetLicense"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "License yöntemi. Bileşeni lisanslar"
type: docs
weight: 20
url: /tr/net/aspose.tasks/license/setlicense/
---
## SetLicense(string) {#setlicense_1}

Bileşeni lisanslar.

```csharp
public void SetLicense(string licenseName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| licenseName | Dize | Tam veya kısa dosya adı ya da gömülü bir kaynağın adı olabilir. Değerlendirme moduna geçmek için boş bir dize kullanın. |

## Açıklamalar

Lisansı aşağıdaki konumlarda bulmaya çalışır:

1. Açık yol.

2. Aspose bileşen derlemesini içeren klasör.

3. İstemcinin çağıran derlemesini içeren klasör.

4. Giriş (başlangıç) derlemesini içeren klasör.

5. İstemcinin çağıran derlemesindeki gömülü kaynak.

**Note:**On the .NET Compact Framework, tries to find the license only in these locations:

1. Açık yol.

2. İstemcinin çağıran derlemesindeki gömülü kaynak.

2. Aspose bileşen JAR dosyasını içeren klasör.

3. İstemcinin çağıran JAR dosyasını içeren klasör.

## Örnekler

Bu örnekte, bileşeni içeren klasörde, çağıran derlemenin bulunduğu klasörde, giriş derlemesinin klasöründe ve ardından çağıran derlemenin gömülü kaynaklarında MyLicense.lic adlı bir lisans dosyası bulunmaya çalışılacaktır.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");
```

bileşen jar dosyası:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

Aspose.Tasks lisansının nasıl uygulanacağını gösterir.

```csharp
var license = new License();
license.SetLicense("Aspose.Tasks.lic");
```

### Ayrıca Bakınız

* class [License](../)
* namespace [Aspose.Tasks](../../license/)
* assembly [Aspose.Tasks](../../../)

---

## SetLicense(Stream) {#setlicense}

Bileşeni lisanslar.

```csharp
public void SetLicense(Stream stream)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Akış | Lisansı içeren bir akış. |

## Açıklamalar

Bu yöntemi bir akıştan lisans yüklemek için kullanın.

## Örnekler

```csharp
[C#]

License license = new License();
license.SetLicense(myStream);


[Visual Basic]

Dim license as License = new License
license.SetLicense(myStream)

License license = new License();
license.setLicense(myStream);
```

Aspose.Tasks lisansının &lt;see cref=\"System.IO.FileStream\" /&gt; üzerinden okunarak nasıl uygulanacağını gösterir.

```csharp
var license = new License();
using (var stream = new FileStream("Aspose.Tasks.lic", FileMode.Open))
{
    license.SetLicense(stream);
}
```

### Ayrıca Bakınız

* class [License](../)
* namespace [Aspose.Tasks](../../license/)
* assembly [Aspose.Tasks](../../../)


