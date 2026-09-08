---
title: "Rsc.RegularWork"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Общее количество работы без сверхурочных, запланированной для выполнения ресурсом"
type: docs
weight: 570
url: /ru/net/aspose.tasks/rsc/regularwork/
---
## Rsc.RegularWork field

Общее количество запланированной работы без сверхурочных, которую должен выполнить ресурс.

```csharp
public static readonly Key<Duration, RscKey> RegularWork;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.RegularWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RegularWork, project.GetWork(1));

Console.WriteLine("Regular Work: " + resource.Get(Rsc.RegularWork));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


