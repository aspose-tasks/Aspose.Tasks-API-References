---
title: "Tsk.IsResumeValid"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. Bepaalt of een taak hervat kan worden"
type: docs
weight: 680
url: /nl/net/aspose.tasks/tsk/isresumevalid/
---
## Tsk.IsResumeValid field

Bepaalt of een taak kan worden hervat.

```csharp
public static readonly Key<NullableBool, TaskKey> IsResumeValid;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.IsResumeValid gelezen/geschreven kan worden.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsResumeValid, true);

Console.WriteLine("Is Resume Valid: " + task.Get(Tsk.IsResumeValid));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


