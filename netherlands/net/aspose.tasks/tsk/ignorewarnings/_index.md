---
title: "Tsk.IgnoreWarnings"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. Geeft aan of de waarschuwing voor planningsconflict in Microsoft Project moet worden verborgen"
type: docs
weight: 540
url: /nl/net/aspose.tasks/tsk/ignorewarnings/
---
## Tsk.IgnoreWarnings field

Geeft aan of de waarschuwing voor planningsconflicten moet worden verborgen in Microsoft Project.

```csharp
public static readonly Key<bool, TaskKey> IgnoreWarnings;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.IgnoreWarnings te lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IgnoreWarnings, true);

Console.WriteLine("Ignore Warnings: " + task.Get(Tsk.IgnoreWarnings));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


