---
title: "Tsk.NotesRTF"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Текстовые заметки в формате RTF. Поддерживается только для форматов MPP"
type: docs
weight: 820
url: /ru/net/aspose.tasks/tsk/notesrtf/
---
## Tsk.NotesRTF field

Текстовые заметки в формате RTF. Поддерживается только для форматов MPP.

```csharp
public static readonly Key<string, TaskKey> NotesRTF;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.NotesRTF.

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

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


