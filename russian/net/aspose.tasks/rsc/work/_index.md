---
title: "Rsc.Work"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Общее количество времени, запланированного для ресурса в задаче"
type: docs
weight: 690
url: /ru/net/aspose.tasks/rsc/work/
---
## Rsc.Work field

Общее количество запланированного времени для ресурса в задаче.

```csharp
public static readonly Key<Duration, RscKey> Work;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.Work.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Work, project.GetWork(1));

Console.WriteLine("Work: " + resource.Get(Rsc.Work));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


