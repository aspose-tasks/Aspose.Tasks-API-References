---
title: "Tsk.IsSummary"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. Bepaalt of een taak een samenvattingstaak is"
type: docs
weight: 720
url: /nl/net/aspose.tasks/tsk/issummary/
---
## Tsk.IsSummary field

Bepaalt of een taak een samenvattingstaak is.

```csharp
public static readonly Key<bool, TaskKey> IsSummary;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.IsSummary gelezen/geschreven kan worden.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsSummary, true);

Console.WriteLine("Is Summary: " + task.Get(Tsk.IsSummary));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


