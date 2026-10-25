---
title: "Prj.WorkFormat"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Görevin süresini göstermek için kullanılan format"
type: docs
weight: 790
url: /tr/net/aspose.tasks/prj/workformat/
---
## Prj.WorkFormat field

Görevin süresini göstermek için kullanılan format.

```csharp
public static readonly Key<TimeUnitType, PrjKey> WorkFormat;
```

## Örnekler

Varsayılan iş formatı ile bir sürenin nasıl alınacağını gösterir.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

Console.WriteLine("Project's work format: " + project.Get(Prj.WorkFormat));

// Projenin varsayılan iş formatı ile bir iş değeri oluştur
var work = project.GetWork(2);
Console.WriteLine("Work: " + work.TimeSpan);
Console.WriteLine("Time unit: " + work.TimeUnit);
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TimeUnitType](../../timeunittype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


