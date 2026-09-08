---
title: "Tsk.CommitmentStart"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. De startdatum van een levering. Lezen wordt alleen ondersteund voor XML-indeling."
type: docs
weight: 180
url: /nl/net/aspose.tasks/tsk/commitmentstart/
---
## Tsk.CommitmentStart field

De startdatum van een levering. Lezen wordt alleen ondersteund voor XML-indeling.

```csharp
public static readonly Key<DateTime, TaskKey> CommitmentStart;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.CommitmentStart te lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.CommitmentStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Commitment Start: " + task.Get(Tsk.CommitmentStart));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


