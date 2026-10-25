---
title: "Tsk.DurationText"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. Retourneert de duurtekst van de taak"
type: docs
weight: 310
url: /nl/net/aspose.tasks/tsk/durationtext/
---
## Tsk.DurationText field

Geeft de duurtekst van de taak terug.

```csharp
public static readonly Key<string, TaskKey> DurationText;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.DurationText te lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DurationText, "Not A Duration");

Console.WriteLine("Duration Text: " + task.Get(Tsk.DurationText));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


