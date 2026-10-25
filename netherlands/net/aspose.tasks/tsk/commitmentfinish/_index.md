---
title: "Tsk.CommitmentFinish"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk field. De einddatum van een levering.  Alleen lezen ondersteund voor XML-formaat"
type: docs
weight: 170
url: /nl/net/aspose.tasks/tsk/commitmentfinish/
---
## Tsk.CommitmentFinish field

De einddatum van een levering. Lezen wordt alleen ondersteund voor XML-indeling.

```csharp
public static readonly Key<DateTime, TaskKey> CommitmentFinish;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.CommitmentFinish te lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.CommitmentFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Commitment Finish: " + task.Get(Tsk.CommitmentFinish));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


