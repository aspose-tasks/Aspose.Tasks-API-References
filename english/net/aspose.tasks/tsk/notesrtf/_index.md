---
title: Tsk.NotesRTF
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The text notes in RTF format. Supported for MPP formats only
type: docs
weight: 820
url: /net/aspose.tasks/tsk/notesrtf/
---
## Tsk.NotesRTF field

The text notes in RTF format. Supported for MPP formats only.

```csharp
public static readonly Key<string, TaskKey> NotesRTF;
```

## Examples

Shows how to read/write Tsk.NotesRTF property.

```csharp
var project = new Project();

            var task = project.RootTask.Children.Add("Task");

            const string rtf = @"{\rtf1\ansi\ansicpg1252\deff0\deflang1033{\fonttbl{\f0\fnil\fcharset134 SimSun;}{\f1\fnil\fcharset0 Calibri;}}
{\*\generator Msftedit 5.41.21.2510;}\viewkind4\uc1\pard\sa200\sl276\slmult1\lang9\f0\fs22\'d4\'e7\'c9\'cf\'ba\'c3\f1\par
}
 "; // 早上好

            task.Set(Tsk.NotesRTF, rtf);

            Console.WriteLine("Notes RTF: " + task.Get(Tsk.NotesRTF));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


