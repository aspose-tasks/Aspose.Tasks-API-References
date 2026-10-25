---
title: "Tsk.DisplayOnTimeline"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. Geeft aan of een taak moet worden weergegeven in een tijdlijnweergave"
type: docs
weight: 290
url: /nl/net/aspose.tasks/tsk/displayontimeline/
---
## Tsk.DisplayOnTimeline field

Specificeert of een taak moet worden weergegeven in een tijdlijnweergave.

```csharp
public static readonly Key<bool, TaskKey> DisplayOnTimeline;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.DisplayOnTimeline te lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DisplayOnTimeline, true);

Console.WriteLine("Display On Timeline: " + task.Get(Tsk.DisplayOnTimeline));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


