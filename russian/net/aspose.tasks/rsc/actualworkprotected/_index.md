---
title: "Rsc.ActualWorkProtected"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Объём работы, через который защищена фактическая работа"
type: docs
weight: 80
url: /ru/net/aspose.tasks/rsc/actualworkprotected/
---
## Rsc.ActualWorkProtected field

Объём работы, через который защищена фактическая работа.

```csharp
public static readonly Key<Duration, RscKey> ActualWorkProtected;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.ActualWorkProtected.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Work Protected: " + resource.Get(Rsc.ActualWorkProtected));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


