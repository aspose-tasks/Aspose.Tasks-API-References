---
title: "Tsk.IsPublished"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. Bepaalt of de huidige taak moet worden gepubliceerd naar Project Server samen met de rest van het project"
type: docs
weight: 660
url: /nl/net/aspose.tasks/tsk/ispublished/
---
## Tsk.IsPublished field

Bepaalt of de huidige taak moet worden gepubliceerd naar Project Server samen met de rest van het project.

```csharp
public static readonly Key<NullableBool, TaskKey> IsPublished;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.IsPublished te lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsPublished, true);

Console.WriteLine("Is Published: " + task.Get(Tsk.IsPublished));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


