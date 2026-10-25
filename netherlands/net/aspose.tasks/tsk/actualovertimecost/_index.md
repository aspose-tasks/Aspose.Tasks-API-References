---
title: "Tsk.ActualOvertimeCost"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. Kosten gemaakt voor overwerk die al op taken zijn uitgevoerd door toegewezen resources."
type: docs
weight: 50
url: /nl/net/aspose.tasks/tsk/actualovertimecost/
---
## Tsk.ActualOvertimeCost field

Kosten die zijn gemaakt voor overwerk dat al op taken door toegewezen resources is uitgevoerd.

```csharp
public static readonly Key<decimal, TaskKey> ActualOvertimeCost;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.ActualOvertimeCost te lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualOvertimeCost, 10m);

Console.WriteLine("Actual Overtime Cost: " + task.Get(Tsk.ActualOvertimeCost));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


