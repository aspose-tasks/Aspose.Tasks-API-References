---
title: "Tsk.DurationVariance"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. Het verschil tussen de basisduur van een taak en de huidige totale duurschatting van een taak."
type: docs
weight: 320
url: /nl/net/aspose.tasks/tsk/durationvariance/
---
## Tsk.DurationVariance field

Het verschil tussen de basislijnduur van een taak en de totale duur (huidige schatting) van een taak.

```csharp
public static readonly Key<Duration, TaskKey> DurationVariance;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.DurationVariance te lezen/schrijven.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DurationVariance, project.GetWork(1));

Console.WriteLine("Duration Variance: " + task.Get(Tsk.DurationVariance));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


