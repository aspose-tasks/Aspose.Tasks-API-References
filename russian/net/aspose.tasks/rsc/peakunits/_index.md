---
title: "Rsc.PeakUnits"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Максимальная единица назначения для ресурса в любой момент времени для всех задач, к которым ресурс назначен"
type: docs
weight: 540
url: /ru/net/aspose.tasks/rsc/peakunits/
---
## Rsc.PeakUnits field

Максимальная единица назначения ресурса в любой момент времени для всех задач, к которым ресурс назначен.

```csharp
public static readonly Key<double, RscKey> PeakUnits;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.PeakUnits.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.PeakUnits, 2);

Console.WriteLine("Peak Units: " + resource.Get(Rsc.PeakUnits));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


