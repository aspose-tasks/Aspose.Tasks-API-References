---
title: "Tsk.WBS"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. Werkverdelingsstructuur WBS-codes"
type: docs
weight: 1130
url: /nl/net/aspose.tasks/tsk/wbs/
---
## Tsk.WBS field

Work breakdown structure (WBS)-codes.

```csharp
public static readonly Key<string, TaskKey> WBS;
```

## Voorbeelden

Toont hoe de WBS-codes van een taak te lezen.

```csharp
var project = new Project(DataDir + "TaskWBS.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Alle verzamelde taken doorlopen
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.WBS));
    Console.WriteLine(task.Get(Tsk.WBSLevel));
}
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


