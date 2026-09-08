---
title: "Tsk.PercentWorkComplete"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. De huidige status van een taak uitgedrukt als het percentage van het werk dat is voltooid"
type: docs
weight: 890
url: /nl/net/aspose.tasks/tsk/percentworkcomplete/
---
## Tsk.PercentWorkComplete field

De huidige status van een taak, uitgedrukt als het percentage van het werk dat is voltooid.

```csharp
public static readonly Key<int, TaskKey> PercentWorkComplete;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.PercentWorkComplete te lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PercentWorkComplete, 10);

Console.WriteLine("Percent Work Complete: " + task.Get(Tsk.PercentWorkComplete));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


