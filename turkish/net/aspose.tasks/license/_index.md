---
title: "Sınıf Lisans"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.License sınıfı. Bileşeni lisanslamak için yöntemler sağlar."
type: docs
weight: 980
url: /tr/net/aspose.tasks/license/
---
## License class

Bileşeni lisanslamak için yöntemler sağlar.

```csharp
public sealed class License
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [License](license/)() | `License` sınıfının yeni bir örneğini başlatır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [SetLicense](../../aspose.tasks/license/setlicense/#setlicense)(Stream) | Bileşeni lisanslar. |
| [SetLicense](../../aspose.tasks/license/setlicense/#setlicense_1)(string) | Bileşeni lisanslar. |

## Örnekler

Bu örnekte, bileşeni içeren klasörde, çağıran derlemenin bulunduğu klasörde, giriş derlemesinin klasöründe ve ardından çağıran derlemenin gömülü kaynaklarında MyLicense.lic adlı bir lisans dosyası bulunmaya çalışılacaktır.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As license = New license
License.SetLicense("MyLicense.lic")
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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


