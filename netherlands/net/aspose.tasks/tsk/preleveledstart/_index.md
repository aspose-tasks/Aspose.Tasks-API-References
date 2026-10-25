---
title: "Tsk.PreleveledStart"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. De startdatum van een taak zoals die was voordat resource-leveling werd uitgevoerd"
type: docs
weight: 920
url: /nl/net/aspose.tasks/tsk/preleveledstart/
---
## Tsk.PreleveledStart field

De startdatum van een taak zoals die was voordat resource-leveling werd uitgevoerd.

```csharp
public static readonly Key<DateTime, TaskKey> PreleveledStart;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.PreleveledStart gelezen/geschreven kan worden.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PreleveledStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Preleveled Start: " + task.Get(Tsk.PreleveledStart));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


