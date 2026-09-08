---
title: "Tsk.RemainingOvertimeCost"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. De resterende geplande overurenkosten voor een taak."
type: docs
weight: 970
url: /nl/net/aspose.tasks/tsk/remainingovertimecost/
---
## Tsk.RemainingOvertimeCost field

De resterende geplande overurenkosten voor een taak.

```csharp
public static readonly Key<decimal, TaskKey> RemainingOvertimeCost;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.RemainingOvertimeCost te lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingOvertimeCost, 2m);

Console.WriteLine("Remaining Overtime Cost: " + task.Get(Tsk.RemainingOvertimeCost));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


