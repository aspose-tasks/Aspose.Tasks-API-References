---
title: "PrimaveraReadOptions.ProjectUid"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "PrimaveraReadOptions özelliği. Birden fazla proje içeren dosyadan okunacak projenin UID'sini alır veya ayarlar."
type: docs
weight: 30
url: /tr/net/aspose.tasks/primaverareadoptions/projectuid/
---
## PrimaveraReadOptions.ProjectUid property

Birden fazla proje içeren dosyadan okunacak projenin UID'sini alır veya ayarlar.

```csharp
public int ProjectUid { get; set; }
```

## Örnekler

Birden fazla proje içeren Primavera XML veya Primavera XER dosyasından bir projenin nasıl okunacağını gösterir.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 3881;

// Özel UID'ye sahip projeyi döndürür
var project = new Project(DataDir + "PrimaveraProject.xml", options);
Console.WriteLine(project.Get(Prj.Name));
```

### Ayrıca Bakınız

* class [PrimaveraReadOptions](../)
* namespace [Aspose.Tasks](../../primaverareadoptions/)
* assembly [Aspose.Tasks](../../../)


