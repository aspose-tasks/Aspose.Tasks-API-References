---
title: "Rsc.RemainingWork"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Время, необходимое для завершения задачи или набора задач"
type: docs
weight: 610
url: /ru/net/aspose.tasks/rsc/remainingwork/
---
## Rsc.RemainingWork field

Время, необходимое для завершения задачи или набора задач.

```csharp
public static readonly Key<Duration, RscKey> RemainingWork;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.RemainingWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingWork, project.GetWork(1));

Console.WriteLine("Remaining Work: " + resource.Get(Rsc.RemainingWork));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


