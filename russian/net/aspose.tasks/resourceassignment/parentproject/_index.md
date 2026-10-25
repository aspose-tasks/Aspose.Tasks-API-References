---
title: "ResourceAssignment.ParentProject"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство ResourceAssignment. Получает родительский проект для этого назначения"
type: docs
weight: 420
url: /ru/net/aspose.tasks/resourceassignment/parentproject/
---
## ResourceAssignment.ParentProject property

Получает родительский проект для этого назначения.

```csharp
public Project ParentProject { get; }
```

## Примеры

Показывает, как использовать родительский проект назначения ресурса.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);

// установить длительность назначения, используя тип единицы времени проекта по умолчанию.
resourceAssignment.Set(Asn.Work, resource.ParentProject.GetWork(1));

Console.WriteLine(resourceAssignment.Get(Asn.Work));
```

### См. также

* class [Project](../../project/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


