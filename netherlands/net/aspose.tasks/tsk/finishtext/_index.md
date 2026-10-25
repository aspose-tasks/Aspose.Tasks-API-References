---
title: "Tsk.FinishText"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. Retourneert de eindtekst van de taak"
type: docs
weight: 410
url: /nl/net/aspose.tasks/tsk/finishtext/
---
## Tsk.FinishText field

Geeft de eindtekst van de taak terug.

```csharp
public static readonly Key<string, TaskKey> FinishText;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.FinishText te lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.FinishText, "Not A Finish");

Console.WriteLine("Finish Text: " + task.Get(Tsk.FinishText));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


