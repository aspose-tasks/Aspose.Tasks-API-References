---
title: "Tsk.NotesText"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk field. Notities platte tekst geëxtraheerd uit RTF-gegevens"
type: docs
weight: 830
url: /nl/net/aspose.tasks/tsk/notestext/
---
## Tsk.NotesText field

Platte tekst van notities geëxtraheerd uit RTF‑gegevens.

```csharp
public static readonly Key<string, TaskKey> NotesText;
```

## Voorbeelden

Toont hoe de Tsk.NotesText-eigenschap gelezen/schreven kan worden.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.NotesText, "Notes");

Console.WriteLine("Notes Text: " + task.Get(Tsk.NotesText));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


