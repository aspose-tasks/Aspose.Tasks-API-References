---
title: "Tsk.CommitmentType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. Bepaalt of een taak een gekoppelde levering heeft of een afhankelijkheid van een gekoppelde levering. Lezen wordt alleen ondersteund voor XML-indeling."
type: docs
weight: 190
url: /nl/net/aspose.tasks/tsk/commitmenttype/
---
## Tsk.CommitmentType field

Bepaalt of een taak een gekoppelde levering heeft of een afhankelijkheid van een gekoppelde levering. Lezen wordt alleen ondersteund voor XML-indeling.

```csharp
public static readonly Key<int, TaskKey> CommitmentType;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.CommitmentType te lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.CommitmentType, 2);

Console.WriteLine("Commitment Type: " + task.Get(Tsk.CommitmentType));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


