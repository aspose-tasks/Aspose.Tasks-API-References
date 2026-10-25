---
title: "Tsk.NotesText"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. ملاحظات نصية عادية مستخرجة من بيانات RTF"
type: docs
weight: 830
url: /ar/net/aspose.tasks/tsk/notestext/
---
## Tsk.NotesText field

النص العادي للملاحظات المستخرج من بيانات RTF.

```csharp
public static readonly Key<string, TaskKey> NotesText;
```

## الأمثلة

يعرض كيفية قراءة/كتابة الخاصية Tsk.NotesText.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.NotesText, "Notes");

Console.WriteLine("Notes Text: " + task.Get(Tsk.NotesText));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


