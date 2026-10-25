---
title: "Task.ParentTask"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Task özelliği. Bir görevin üst görevini alır"
type: docs
weight: 940
url: /tr/net/aspose.tasks/task/parenttask/
---
## Task.ParentTask property

Bir görevin üst görevini alır.

```csharp
public Task ParentTask { get; }
```

## Örnekler

Bir görevin üst görevinin nasıl kullanılacağını gösterir.

```csharp
var project = new Project();
var parent = project.RootTask.Children.Add("Parent");
var child1 = parent.Children.Add("Child1");
var child2 = child1.ParentTask.Children.Add("Child2");

Console.WriteLine("Is parent is equal to the root task: " + child2.ParentTask.Equals(parent));
```

### Ayrıca Bakınız

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


