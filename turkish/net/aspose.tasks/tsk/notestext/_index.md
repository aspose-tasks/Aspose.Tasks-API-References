---
title: "Tsk.NotesText"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. RTF verisinden çıkarılan notların düz metni"
type: docs
weight: 830
url: /tr/net/aspose.tasks/tsk/notestext/
---
## Tsk.NotesText field

RTF verilerinden çıkarılan notların düz metni.

```csharp
public static readonly Key<string, TaskKey> NotesText;
```

## Örnekler

Tsk.NotesText özelliğini okuma/yazma nasıl yapılacağını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.NotesText, "Notes");

Console.WriteLine("Notes Text: " + task.Get(Tsk.NotesText));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


