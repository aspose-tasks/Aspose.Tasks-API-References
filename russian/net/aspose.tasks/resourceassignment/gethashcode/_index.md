---
title: "ResourceAssignment.GetHashCode"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ResourceAssignment. Возвращает значение хеш‑кода для экземпляра класса ResourceAssignment"
type: docs
weight: 710
url: /ru/net/aspose.tasks/resourceassignment/gethashcode/
---
## ResourceAssignment.GetHashCode method

Возвращает значение хеш‑кода для экземпляра класса [`ResourceAssignment`](../).

```csharp
public override int GetHashCode()
```

### Возвращаемое значение

возвращает значение хеш‑кода для этого объекта.

## Примеры

Показывает, как получить хеш‑код назначения ресурса.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var resourceAssignment1 = project.ResourceAssignments.GetByUid(2);
var resourceAssignment2 = project.ResourceAssignments.GetByUid(3);

// вывести хеш‑коды назначения
Console.WriteLine("Resource Assignment 1 Hash Code: {0}", resourceAssignment1.GetHashCode());
Console.WriteLine("Resource Assignment 2 Hash Code: {0}", resourceAssignment2.GetHashCode());
```

### См. также

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


