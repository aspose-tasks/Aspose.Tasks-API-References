---
title: "Tsk.StartText"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. Geeft de starttekst van de taak terug"
type: docs
weight: 1030
url: /nl/net/aspose.tasks/tsk/starttext/
---
## Tsk.StartText field

Retourneert de starttekst van de taak.

```csharp
public static readonly Key<string, TaskKey> StartText;
```

## Voorbeelden

Toont hoe de Tsk.StartText-eigenschap gelezen/schreven kan worden.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.StartText, "Start Task Text");

Console.WriteLine("Start Text: " + task.Get(Tsk.StartText));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


