---
title: Tsk.NotesText
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. Notes plain text extracted from RTF data
type: docs
weight: 830
url: /net/aspose.tasks/tsk/notestext/
---
## Tsk.NotesText field

Notes' plain text extracted from RTF data.

```csharp
public static readonly Key<string, TaskKey> NotesText;
```

## Examples

Shows how to read/write Tsk.NotesText property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.NotesText, "Notes");

Console.WriteLine("Notes Text: " + task.Get(Tsk.NotesText));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


