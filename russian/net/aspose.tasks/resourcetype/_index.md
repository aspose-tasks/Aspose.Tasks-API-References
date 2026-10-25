---
title: "Перечисление ResourceType"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Aspose.Tasks.ResourceType enum. Указывает тип ресурса"
type: docs
weight: 1800
url: /ru/net/aspose.tasks/resourcetype/
---
## ResourceType enumeration

Указывает тип ресурса.

```csharp
public enum ResourceType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Material | `0` | Указывает тип ресурса Material. |
| Work | `1` | Указывает тип ресурса Work. |
| Cost | `2` | Указывает тип ресурса Cost. |

## Примеры

Показывает, как работать с типами ресурсов.

```csharp
var project = new Project();

// добавить рабочий ресурс
var work = project.Resources.Add("Work resource");
work.Set(Rsc.Type, ResourceType.Work);

// добавить материалный ресурс
var material = project.Resources.Add("Material resource");
material.Set(Rsc.Type, ResourceType.Material);
material.Set(Rsc.MaterialLabel, "kg");

// добавить материалный ресурс
var cost = project.Resources.Add("Cost resource");
cost.Set(Rsc.Type, ResourceType.Cost);
cost.Set(Rsc.Cost, 59.99m);

// работа с ресурсами: создавать задачи, назначать ресурсы и т.д.
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


