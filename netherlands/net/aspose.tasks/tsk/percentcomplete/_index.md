---
title: "Tsk.PercentComplete"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. De huidige status van een taak uitgedrukt als het percentage van de duur van de taak dat is voltooid"
type: docs
weight: 880
url: /nl/net/aspose.tasks/tsk/percentcomplete/
---
## Tsk.PercentComplete field

De huidige status van een taak, uitgedrukt als het percentage van de duur van de taak dat is voltooid.

```csharp
public static readonly Key<int, TaskKey> PercentComplete;
```

## Voorbeelden

Toont hoe de voortgang van een taak gewijzigd kan worden door het bijwerken van het percentage voltooid.

```csharp
var project = new Project();
Console.WriteLine("Project Calculation mode is Automatic: {0}", project.CalculationMode.Equals(CalculationMode.Automatic));

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Duration, project.GetDuration(2));
task.Set(Tsk.PercentComplete, 50);

// Toegang tot taken en weergave van voltooiingspercentage
foreach (var tsk in project.RootTask.Children)
{
    Console.WriteLine(tsk.Get(Tsk.PercentComplete));
    Console.WriteLine(tsk.Get(Tsk.PercentWorkComplete));
    Console.WriteLine(tsk.Get(Tsk.PhysicalPercentComplete));
}
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


