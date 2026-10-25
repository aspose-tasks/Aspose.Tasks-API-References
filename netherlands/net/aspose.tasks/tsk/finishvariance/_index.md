---
title: "Tsk.FinishVariance"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. De tijd die het verschil weergeeft tussen de baseline-einddatum van een taak of toewijzing en de huidige einddatum"
type: docs
weight: 420
url: /nl/net/aspose.tasks/tsk/finishvariance/
---
## Tsk.FinishVariance field

De tijd die het verschil weergeeft tussen de basislijn einddatum van een taak of toewijzing en de huidige einddatum.

```csharp
public static readonly Key<Duration, TaskKey> FinishVariance;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.FinishVariance gelezen/geschreven kan worden.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.FinishVariance, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Finish Variance: " + task.Get(Tsk.FinishVariance));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


