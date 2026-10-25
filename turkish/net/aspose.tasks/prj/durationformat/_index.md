---
title: "Prj.DurationFormat"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Toplu sürenin ifade edilme biçimi"
type: docs
weight: 300
url: /tr/net/aspose.tasks/prj/durationformat/
---
## Prj.DurationFormat field

Toplu sürenin ifade edilme biçimi.

```csharp
public static readonly Key<TimeUnitType, PrjKey> DurationFormat;
```

## Örnekler

Prj.DurationFormat özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

project.Set(Prj.DurationFormat, TimeUnitType.Day);

Console.WriteLine("Duration Format: " + project.Get(Prj.DurationFormat));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TimeUnitType](../../timeunittype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


