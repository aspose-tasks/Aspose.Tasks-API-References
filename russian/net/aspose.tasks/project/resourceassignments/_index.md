---
title: "Project.ResourceAssignments"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Project. Получает объект ResourceAssignmentCollection"
type: docs
weight: 750
url: /ru/net/aspose.tasks/project/resourceassignments/
---
## Project.ResourceAssignments property

Получает объект ResourceAssignmentCollection.

```csharp
public ResourceAssignmentCollection ResourceAssignments { get; }
```

## Примеры

Показывает, как работать с назначениями ресурсов.

```csharp
var project = new Project();

// Добавить новую задачу и ресурс
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Rsc");

// Назначьте ресурс нужной задаче
project.ResourceAssignments.Add(task, resource);
```

### См. также

* class [ResourceAssignmentCollection](../../resourceassignmentcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


