---
title: "License.License"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "License yapıcı. License sınıfının yeni bir örneğini başlatır"
type: docs
weight: 10
url: /tr/net/aspose.tasks/license/license/
---
## License constructor

[`License`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public License()
```

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

* class [License](../)
* namespace [Aspose.Tasks](../../license/)
* assembly [Aspose.Tasks](../../../)


