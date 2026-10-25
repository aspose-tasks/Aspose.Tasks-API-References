---
title: "Tsk.PhysicalPercentComplete"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. Voltooiingspercentage dat kan worden gebruikt als alternatief voor het berekenen van de begrote kostprijs van het uitgevoerde werk (BCWP)"
type: docs
weight: 900
url: /nl/net/aspose.tasks/tsk/physicalpercentcomplete/
---
## Tsk.PhysicalPercentComplete field

Voltooiingspercentage dat kan worden gebruikt als alternatief voor het berekenen van de begrote kostprijs van uitgevoerd werk (BCWP).

```csharp
public static readonly Key<int, TaskKey> PhysicalPercentComplete;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.PhysicalPercentComplete te lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PhysicalPercentComplete, 10);

Console.WriteLine("Physical Percent Complete: " + task.Get(Tsk.PhysicalPercentComplete));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


