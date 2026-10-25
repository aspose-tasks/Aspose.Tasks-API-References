---
title: "LoadOptions.Encoding"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "LoadOptions özelliği. HTML, MPX, XER ve Primavera XML formatlarından bir projeyi okumak için kullanılan kodlamayı alır veya ayarlar. Varsayılan kodlama UTF8'dir."
type: docs
weight: 30
url: /tr/net/aspose.tasks/loadoptions/encoding/
---
## LoadOptions.Encoding property

HTML, MPX, XER ve Primavera XML formatlarından bir proje okurken kullanılan kodlamayı alır veya ayarlar. Varsayılan kodlama UTF8'dir.

```csharp
public Encoding Encoding { get; set; }
```

## Örnekler

Primavera XER dosyasından bir proje açarken kodlamanın nasıl belirtileceğini gösterir.

```csharp
LoadOptions lo = new LoadOptions();
lo.Encoding = Encoding.GetEncoding(1251);
lo.PrimaveraReadOptions = new PrimaveraReadOptions();
var project = new Project("encoding1251.xer", lo);
```

### Ayrıca Bakınız

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


