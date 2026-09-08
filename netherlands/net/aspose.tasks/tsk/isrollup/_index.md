---
title: "Tsk.IsRollup"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. Bepaalt of informatie over de subtaak-Gantt-balken wordt samengevoegd tot de samenvattingstaakbalk."
type: docs
weight: 690
url: /nl/net/aspose.tasks/tsk/isrollup/
---
## Tsk.IsRollup field

Bepaalt of informatie over de subtaak‑Gantt-balken wordt samengevoegd naar de samenvattingstaak‑balk.

```csharp
public static readonly Key<NullableBool, TaskKey> IsRollup;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.IsRollup te lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsRollup, true);

Console.WriteLine("Is Rollup: " + task.Get(Tsk.IsRollup));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


