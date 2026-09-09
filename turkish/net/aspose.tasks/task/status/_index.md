---
title: "Task.Status"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Task özelliği. Görev durumunu alır."
type: docs
weight: 1160
url: /tr/net/aspose.tasks/task/status/
---
## Task.Status property

Görev durumunu alır.

```csharp
public TaskStatus Status { get; }
```

## Örnekler

Görevin durumunu nasıl alacağınızı gösterir.

```csharp
var project = new Project(DataDir + "TaskPercentageCompletion.mpp");

// Projenin durum tarihi, durum hesaplaması durum tarihini kullandığı için ayarlanmalıdır.
project.StatusDate = new DateTime(2010, 7, 9, 15, 0, 0);
foreach (var task in project.EnumerateAllChildTasks())
{
    Console.WriteLine("{0} - {1}", task.Name, task.Status);
}
```

### Ayrıca Bakınız

* enum [TaskStatus](../../taskstatus/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


