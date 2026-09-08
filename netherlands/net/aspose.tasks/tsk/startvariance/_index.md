---
title: "Tsk.StartVariance"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. De tijd die het verschil weergeeft tussen een basis‑startdatum van een taak of toewijzing en de momenteel geplande startdatum."
type: docs
weight: 1040
url: /nl/net/aspose.tasks/tsk/startvariance/
---
## Tsk.StartVariance field

De tijd die het verschil weergeeft tussen een baseline-startdatum van een taak of toewijzing en de momenteel geplande startdatum.

```csharp
public static readonly Key<Duration, TaskKey> StartVariance;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.StartVariance te lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.StartVariance, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Start Variance: " + task.Get(Tsk.StartVariance));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


