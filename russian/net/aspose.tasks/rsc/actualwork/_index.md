---
title: "Rsc.ActualWork"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Объём работы, уже выполненной ресурсом, назначенным на задачи"
type: docs
weight: 70
url: /ru/net/aspose.tasks/rsc/actualwork/
---
## Rsc.ActualWork field

Объём работы, уже выполненной ресурсом, назначенным на задачи.

```csharp
public static readonly Key<Duration, RscKey> ActualWork;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.ActualWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualWork, project.GetWork(1));

Console.WriteLine("Actual Work: " + resource.Get(Rsc.ActualWork));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


