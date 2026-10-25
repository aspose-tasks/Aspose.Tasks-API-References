---
title: "Prj.LastPrinted"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Projelerin son yazdırma zamanı. mpp dosyalarında UTC formatında kaydedilir. DateTime türü"
type: docs
weight: 430
url: /tr/net/aspose.tasks/prj/lastprinted/
---
## Prj.LastPrinted field

Projenin son yazdırma zamanı. mpp dosyalarında UTC formatında kaydedilir. DateTime türü.

```csharp
public static readonly Key<DateTime, PrjKey> LastPrinted;
```

## Örnekler

Prj.LastPrinted özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

project.Set(Prj.LastPrinted, new DateTime(2020, 4, 10, 13, 0, 0));

Console.WriteLine("Last Printed: " + project.Get(Prj.LastPrinted));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


