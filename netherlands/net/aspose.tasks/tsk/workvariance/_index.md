---
title: "Tsk.WorkVariance"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. Het verschil tussen de basislijnwerk van een taak en het momenteel geplande werk"
type: docs
weight: 1160
url: /nl/net/aspose.tasks/tsk/workvariance/
---
## Tsk.WorkVariance field

Het verschil tussen de baseline-werk van een taak en het momenteel geplande werk.

```csharp
public static readonly Key<Duration, TaskKey> WorkVariance;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.WorkVariance te lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.WorkVariance, project.GetDuration(1));

Console.WriteLine("Work Variance: " + task.Get(Tsk.WorkVariance));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


