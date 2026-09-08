---
title: "Tsk.IsNull"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. Bepaalt of een taak een null-taak is"
type: docs
weight: 640
url: /nl/net/aspose.tasks/tsk/isnull/
---
## Tsk.IsNull field

Bepaalt of een taak een nul‑taak is.

```csharp
public static readonly Key<NullableBool, TaskKey> IsNull;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.IsNull te lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsNull, true);

Console.WriteLine("Is Null: " + task.Get(Tsk.IsNull));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


