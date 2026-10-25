---
title: "Tsk.NotesText"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Текст заметок в простом виде, извлечённый из данных RTF"
type: docs
weight: 830
url: /ru/net/aspose.tasks/tsk/notestext/
---
## Tsk.NotesText field

Обычный текст заметок, извлечённый из данных RTF.

```csharp
public static readonly Key<string, TaskKey> NotesText;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.NotesText.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.NotesText, "Notes");

Console.WriteLine("Notes Text: " + task.Get(Tsk.NotesText));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


