---
title: "Task.ParentProject"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Task özelliği. Bir görevin üst projesini alır."
type: docs
weight: 930
url: /tr/net/aspose.tasks/task/parentproject/
---
## Task.ParentProject property

Bir görevin üst projesini alır.

```csharp
public Project ParentProject { get; }
```

## Açıklamalar

Bu özellikleri güncellemek için Project.UpdateReferences metodunu çağırın.

## Örnekler

Görevin üst projesinin nasıl kullanılacağını gösterir.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Parent");

// Görev için varsayılan proje zaman birimi türünü kullanarak bir süre ayarlayın.
task.Set(Tsk.Duration, task.ParentProject.GetDuration(1));

Console.WriteLine(task.Get(Tsk.Duration));
```

### Ayrıca Bakınız

* class [Project](../../project/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


