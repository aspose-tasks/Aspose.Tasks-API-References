---
title: "Rsc.PercentWorkComplete"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Процент выполненной работы по всем задачам"
type: docs
weight: 550
url: /ru/net/aspose.tasks/rsc/percentworkcomplete/
---
## Rsc.PercentWorkComplete field

Процент выполненной работы по всем задачам.

```csharp
public static readonly Key<int, RscKey> PercentWorkComplete;
```

## Примеры

Показывает, как читать процент завершённой работы ресурса.

```csharp
var project = new Project(DataDir + "ResourcePercentWorkComplete.mpp");

// Отображать процент завершения работы для всех ресурсов
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) != null)
    {
        Console.WriteLine(res.Get(Rsc.PercentWorkComplete));
    }
}
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


