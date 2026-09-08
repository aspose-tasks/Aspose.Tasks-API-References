---
title: "Project.RemoveInvalidResourceAssignments"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Project. Удаляет недействительные назначения ресурсов из списка назначений ресурсов проекта."
type: docs
weight: 1170
url: /ru/net/aspose.tasks/project/removeinvalidresourceassignments/
---
## Project.RemoveInvalidResourceAssignments method

Удаляет недействительные назначения ресурсов из списка назначений ресурсов проекта.

```csharp
public void RemoveInvalidResourceAssignments()
```

## Примечания

MS Project создает пустое назначение ресурса для каждой задачи. Вызовите метод, чтобы удалить их.

## Примеры

Показывает, как удалить недействительные назначения.

```csharp
var project = new Project(DataDir + "InvalidResourceAssignments.mpp");
var invalid = 0;

// ReSharper disable once LoopCanBeConvertedToQuery //ExSkip
foreach (var ra in project.ResourceAssignments)
{
    if (ra.Get(Asn.Resource) == null)
    {
        invalid++;
    }
}

Console.WriteLine("Count of invalid assignments (before): " + invalid);

// удалить недействительные назначения
project.RemoveInvalidResourceAssignments();

Console.WriteLine("Count of invalid assignments (after): " + invalid);
```

### См. также

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


