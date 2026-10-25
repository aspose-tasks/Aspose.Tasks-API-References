---
title: "Prj.LastSaved"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Bir projenin en son kaydedildiği tarih. mpp dosyalarında UTC formatında kaydedilir. DateTime türü"
type: docs
weight: 440
url: /tr/net/aspose.tasks/prj/lastsaved/
---
## Prj.LastSaved field

Bir projenin en son kaydedildiği tarih. mpp dosyalarında UTC formatında kaydedilir. DateTime türü.

```csharp
public static readonly Key<DateTime, PrjKey> LastSaved;
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


