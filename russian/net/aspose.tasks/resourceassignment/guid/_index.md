---
title: "ResourceAssignment.Guid"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство ResourceAssignment. Получает или задает уникальный идентификатор для этого назначения"
type: docs
weight: 290
url: /ru/net/aspose.tasks/resourceassignment/guid/
---
## ResourceAssignment.Guid property

Получает или задает уникальный идентификатор для этого назначения.

```csharp
public Guid? Guid { get; set; }
```

## Примеры

Показывает, как прочитать GUID назначения ресурса.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine(assignment.Guid);
```

### См. также

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


