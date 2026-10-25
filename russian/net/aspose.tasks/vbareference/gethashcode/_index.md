---
title: "VbaReference.GetHashCode"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод VbaReference. Возвращает значение хеш‑кода для этого VbaReference."
type: docs
weight: 50
url: /ru/net/aspose.tasks/vbareference/gethashcode/
---
## VbaReference.GetHashCode method

Возвращает значение хеш‑кода для этого [`VbaReference`](../).

```csharp
public override int GetHashCode()
```

### Возвращаемое значение

Возвращает значение хэш‑кода для этого объекта.

## Примеры

Показывает, как получить хеш‑код VBA‑ссылки.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

var reference1 = project.VbaProject.References.ToList()[0];
var reference2 = project.VbaProject.References.ToList()[1];

// Хеш‑код ссылки является хеш‑кодом внутреннего GUID ссылки.
Console.WriteLine("VBA reference Hash Code: {0}", reference1.GetHashCode());
Console.WriteLine("VBA reference Hash Code: {0}", reference2.GetHashCode());
```

### См. также

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)


