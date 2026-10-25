---
title: "Tsk.NotesText"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Απλό κείμενο σημειώσεων εξάγεται από δεδομένα RTF"
type: docs
weight: 830
url: /el/net/aspose.tasks/tsk/notestext/
---
## Tsk.NotesText field

Απλό κείμενο σημειώσεων εξαγόμενο από δεδομένα RTF.

```csharp
public static readonly Key<string, TaskKey> NotesText;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.NotesText.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.NotesText, "Notes");

Console.WriteLine("Notes Text: " + task.Get(Tsk.NotesText));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


