---
title: "Tsk.IsSubproject"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. Bepaalt of een taak een ingevoegd project is"
type: docs
weight: 700
url: /nl/net/aspose.tasks/tsk/issubproject/
---
## Tsk.IsSubproject field

Bepaalt of een taak een ingevoegd project is.

```csharp
public static readonly Key<bool, TaskKey> IsSubproject;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.IsSubproject gelezen/geschreven kan worden.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsSubproject, true);

Console.WriteLine("Is Subproject: " + task.Get(Tsk.IsSubproject));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


