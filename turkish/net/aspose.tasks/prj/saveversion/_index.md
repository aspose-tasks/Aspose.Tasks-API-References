---
title: "Prj.SaveVersion"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Bir proje dosyasının kaydedildiği Microsoft Office Project sürümü"
type: docs
weight: 620
url: /tr/net/aspose.tasks/prj/saveversion/
---
## Prj.SaveVersion field

Bir proje dosyasının kaydedildiği Microsoft Office Project sürümü.

```csharp
public static readonly Key<int, PrjKey> SaveVersion;
```

## Örnekler

Projenin kaydetme sürümünü ve kaydetme tarihini nasıl kontrol edeceğinizi gösterir.

```csharp
var project = new Project(DataDir + "DetermineProjectVersion.mpp");

// Proje sürümünü göster
Console.WriteLine("Project Version : " + project.Get(Prj.SaveVersion));
Console.WriteLine("Last Saved : " + project.Get(Prj.LastSaved).ToShortDateString());
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


