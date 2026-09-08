---
title: "Resource.Delete"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Resource. Удаляет ресурс и его назначения из проекта"
type: docs
weight: 810
url: /ru/net/aspose.tasks/resource/delete/
---
## Resource.Delete method

Удаляет ресурс и его назначения из проекта.

```csharp
public void Delete()
```

## Примеры

Показывает, как удалить ресурс.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

var resource = project.Resources.GetById(1);

Console.WriteLine("Number of resources (before): " + project.Resources.Count);

// удалить ресурс
resource.Delete();

Console.WriteLine("Number of resources (after): " + project.Resources.Count);
```

### См. также

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


