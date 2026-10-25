---
title: "Tsk.NotesText"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Note in testo semplice estratte dai dati RTF"
type: docs
weight: 830
url: /it/net/aspose.tasks/tsk/notestext/
---
## Tsk.NotesText field

Testo semplice delle note estratto dai dati RTF.

```csharp
public static readonly Key<string, TaskKey> NotesText;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.NotesText.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.NotesText, "Notes");

Console.WriteLine("Notes Text: " + task.Get(Tsk.NotesText));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


