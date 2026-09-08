---
title: "Tsk.RemainingOvertimeWork"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. De hoeveelheid resterende geplande overuren."
type: docs
weight: 980
url: /nl/net/aspose.tasks/tsk/remainingovertimework/
---
## Tsk.RemainingOvertimeWork field

De hoeveelheid resterende geplande overuren.

```csharp
public static readonly Key<Duration, TaskKey> RemainingOvertimeWork;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.RemainingOvertimeWork te lezen/schrijven.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingOvertimeWork, project.GetWork(1));

Console.WriteLine("Remaining Overtime Work: " + task.Get(Tsk.RemainingOvertimeWork));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


