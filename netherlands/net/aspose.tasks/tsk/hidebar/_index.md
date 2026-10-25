---
title: "Tsk.HideBar"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. Bepaalt of de Gantt-balk van een taak verborgen is wanneer deze wordt weergegeven in Microsoft Project"
type: docs
weight: 480
url: /nl/net/aspose.tasks/tsk/hidebar/
---
## Tsk.HideBar field

Bepaalt of de Gantt-balk van een taak verborgen is wanneer deze wordt weergegeven in Microsoft Project.

```csharp
public static readonly Key<NullableBool, TaskKey> HideBar;
```

## Voorbeelden

Toont hoe de Tsk.HideBar-eigenschap gelezen/schreven kan worden.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.HideBar, true);

Console.WriteLine("Hide Bar: " + task.Get(Tsk.HideBar));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


