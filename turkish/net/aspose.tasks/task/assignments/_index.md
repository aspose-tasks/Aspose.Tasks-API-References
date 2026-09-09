---
title: "Task.Assignments"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Task özelliği. Bu nesne için kaynak atamalarının bir koleksiyonunu alır."
type: docs
weight: 120
url: /tr/net/aspose.tasks/task/assignments/
---
## Task.Assignments property

Bu nesne için kaynak atamalarının bir koleksiyonunu alır.

```csharp
public ResourceAssignmentCollection Assignments { get; }
```

## Örnekler

Görevin atamalarında nasıl yineleme yapılacağını gösterir.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // görevin atamalarını göster
    foreach (var assignment in task.Assignments)
    {
        Console.WriteLine(assignment.ToString());
    }
}
```

### Ayrıca Bakınız

* class [ResourceAssignmentCollection](../../resourceassignmentcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


