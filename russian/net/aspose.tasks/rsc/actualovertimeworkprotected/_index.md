---
title: "Rsc.ActualOvertimeWorkProtected"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Количество работы, через которое защищена фактическая сверхурочная работа"
type: docs
weight: 60
url: /ru/net/aspose.tasks/rsc/actualovertimeworkprotected/
---
## Rsc.ActualOvertimeWorkProtected field

Объём работы, через который защищена фактическая сверхурочная работа.

```csharp
public static readonly Key<Duration, RscKey> ActualOvertimeWorkProtected;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.ActualOvertimeWorkProtected.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualOvertimeWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Overtime Work Protected: " + resource.Get(Rsc.ActualOvertimeWorkProtected));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


