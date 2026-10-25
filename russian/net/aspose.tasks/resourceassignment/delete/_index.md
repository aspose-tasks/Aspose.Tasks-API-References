---
title: "ResourceAssignment.Delete"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "ResourceAssignment метод. Удаляет назначение ресурса из коллекции назначений проекта"
type: docs
weight: 680
url: /ru/net/aspose.tasks/resourceassignment/delete/
---
## ResourceAssignment.Delete method

Удаляет назначение ресурса из коллекции назначений проекта.

```csharp
public void Delete()
```

## Примеры

Показывает, как удалить назначение ресурса.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Assignment count (before): {0}", project.ResourceAssignments.Count);

resourceAssignment.Delete();

Console.WriteLine("Assignment count (after): {0}", project.ResourceAssignments.Count);
```

### См. также

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


