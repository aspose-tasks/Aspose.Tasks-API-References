---
title: "Rsc.RemainingOvertimeWork"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Количество оставшегося запланированного сверхурочного времени"
type: docs
weight: 600
url: /ru/net/aspose.tasks/rsc/remainingovertimework/
---
## Rsc.RemainingOvertimeWork field

Количество оставшихся запланированных сверхурочных.

```csharp
public static readonly Key<Duration, RscKey> RemainingOvertimeWork;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.RemainingOvertimeWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingOvertimeWork, project.GetWork(1));

Console.WriteLine("Remaining Overtime Work: " + resource.Get(Rsc.RemainingOvertimeWork));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


