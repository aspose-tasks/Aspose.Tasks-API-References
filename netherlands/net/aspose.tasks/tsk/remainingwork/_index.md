---
title: "Tsk.RemainingWork"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. De tijd die nog nodig is om een taak of een reeks taken te voltooien"
type: docs
weight: 990
url: /nl/net/aspose.tasks/tsk/remainingwork/
---
## Tsk.RemainingWork field

De tijd die nog nodig is om een taak of een reeks taken te voltooien.

```csharp
public static readonly Key<Duration, TaskKey> RemainingWork;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.RemainingWork te lezen/schrijven.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingWork, project.GetWork(1));

Console.WriteLine("Remaining Work: " + task.Get(Tsk.RemainingWork));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


