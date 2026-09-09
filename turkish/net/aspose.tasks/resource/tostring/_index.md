---
title: "Resource.ToString"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Resource yöntemi. Resource sınıfının örneğinin kısa string temsilini döndürür. Temsilin kesin detayları belirtilmemiştir ve değişebilir."
type: docs
weight: 870
url: /tr/net/aspose.tasks/resource/tostring/
---
## Resource.ToString method

[`Resource`](../) sınıfının örneğinin kısa string temsilini döndürür. Temsilin kesin detayları belirtilmemiştir ve değişebilir.

```csharp
public override string ToString()
```

### Dönüş Değeri

kaynak nesnesini temsil eden kısa string.

## Örnekler

resource ToString yönteminin nasıl kullanılacağını gösterir.

```csharp
var project = new Project();
var resource = project.Resources.Add("Resource");

// kaynak ortak bilgilerini yazdır
Console.WriteLine(resource.ToString());
```

### Ayrıca Bakınız

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


