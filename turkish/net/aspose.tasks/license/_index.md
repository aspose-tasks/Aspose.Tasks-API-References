---
title: Class License
second_title: Aspose.Tasks for .NET API Referansı
description: Aspose.Tasks.License sınıf. Bileşeni lisanslamak için yöntemler sağlar.
type: docs
weight: 860
url: /tr/net/aspose.tasks/license/
---
## License class

Bileşeni lisanslamak için yöntemler sağlar.

```csharp
public class License
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [License](license/)() | Yeni bir örneğini başlatır.`License` sınıf. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [SetLicense](../../aspose.tasks/license/setlicense/#setlicense)(Stream) | Bileşeni lisanslar. |
| [SetLicense](../../aspose.tasks/license/setlicense/#setlicense_1)(string) | Bileşeni lisanslar. |

### Örnekler

Bu örnekte, içeren klasörde MyLicense.lic adlı bir lisans dosyası bulunmaya çalışılacaktır. bileşen, çağıran derlemeyi içeren klasörde, giriş derlemesinin klasöründe ve ardından çağıran derlemenin katıştırılmış kaynaklarında.

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

### Ayrıca bakınız

* ad alanı [Aspose.Tasks](../../aspose.tasks/)
* toplantı [Aspose.Tasks](../../)


