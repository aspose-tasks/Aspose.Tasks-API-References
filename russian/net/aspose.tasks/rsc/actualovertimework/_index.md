---
title: "Rsc.ActualOvertimeWork"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Фактическое количество сверхурочной работы, уже выполненной ресурсом, назначенным на задачи"
type: docs
weight: 50
url: /ru/net/aspose.tasks/rsc/actualovertimework/
---
## Rsc.ActualOvertimeWork field

Фактическое количество сверхурочной работы, уже выполненной ресурсом, назначенным на задачи.

```csharp
public static readonly Key<Duration, RscKey> ActualOvertimeWork;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.ActualOvertimeWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualOvertimeWork, project.GetWork(1));

Console.WriteLine("Actual Overtime Work: " + resource.Get(Rsc.ActualOvertimeWork));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


