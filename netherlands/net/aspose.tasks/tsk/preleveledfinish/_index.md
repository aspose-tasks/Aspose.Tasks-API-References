---
title: "Tsk.PreleveledFinish"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. De einddatum van een taak zoals die was voordat resource-leveling werd uitgevoerd"
type: docs
weight: 910
url: /nl/net/aspose.tasks/tsk/preleveledfinish/
---
## Tsk.PreleveledFinish field

De einddatum van een taak zoals die was voordat resource-leveling werd uitgevoerd.

```csharp
public static readonly Key<DateTime, TaskKey> PreleveledFinish;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.PreleveledFinish te lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PreleveledFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Preleveled Finish: " + task.Get(Tsk.PreleveledFinish));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


