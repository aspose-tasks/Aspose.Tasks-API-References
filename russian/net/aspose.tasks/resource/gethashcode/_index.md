---
title: "Resource.GetHashCode"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Resource. Возвращает значение хеш‑кода для экземпляра класса Resource"
type: docs
weight: 840
url: /ru/net/aspose.tasks/resource/gethashcode/
---
## Resource.GetHashCode method

Возвращает значение хеш‑кода для экземпляра класса [`Resource`](../).

```csharp
public override int GetHashCode()
```

### Возвращаемое значение

возвращает значение хеш‑кода для этого объекта.

## Примеры

Показывает, как получить хеш‑код ресурса.

```csharp
var project = new Project(DataDir + "Project.mpp");

var resource1 = project.Resources.GetById(1);
var resource2 = project.Resources.GetById(2);

// хеш‑код ресурса равен UID ресурса
Console.WriteLine("Resource UID: {0} Hash Code: {1}", resource1.Get(Rsc.Uid), resource1.GetHashCode());
Console.WriteLine("Resource UID: {0} Hash Code: {1}", resource2.Get(Rsc.Uid), resource2.GetHashCode());
```

### См. также

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


