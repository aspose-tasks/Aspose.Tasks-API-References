---
title: "Tsk.RemainingDuration"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. De tijd die nodig is om het onafgewerkte deel van een taak te voltooien"
type: docs
weight: 960
url: /nl/net/aspose.tasks/tsk/remainingduration/
---
## Tsk.RemainingDuration field

De tijd die nodig is om het onafgewerkte deel van een taak te voltooien.

```csharp
public static readonly Key<Duration, TaskKey> RemainingDuration;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.RemainingDuration te lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingDuration, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Remaining Duration: " + task.Get(Tsk.RemainingDuration));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


