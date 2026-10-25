---
title: "Tsk.IsExpanded"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. Bepaalt of een samenvattingstaak is uitgeklapt of niet in de GanttChart-weergave"
type: docs
weight: 590
url: /nl/net/aspose.tasks/tsk/isexpanded/
---
## Tsk.IsExpanded field

Bepaalt of een samenvattingstaak is uitgeklapt of niet in de GanttChart-weergave.

```csharp
public static readonly Key<NullableBool, TaskKey> IsExpanded;
```

## Voorbeelden

Toont hoe de Tsk.IsExpanded eigenschap gelezen/geschreven kan worden.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsExpanded, true);

Console.WriteLine("Is Expanded: " + task.Get(Tsk.IsExpanded));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


