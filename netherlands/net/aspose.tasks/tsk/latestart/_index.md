---
title: "Tsk.LateStart"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. De laatste datum waarop een taak kan beginnen zonder de voltooiing van het project te vertragen"
type: docs
weight: 740
url: /nl/net/aspose.tasks/tsk/latestart/
---
## Tsk.LateStart field

De laatste datum waarop een taak kan starten zonder de voltooiing van het project te vertragen.

```csharp
public static readonly Key<DateTime, TaskKey> LateStart;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.LateStart te lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LateStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Late Start: " + task.Get(Tsk.LateStart));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


