---
title: "Tsk.NotesRTF"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. ملاحظات النص بتنسيق RTF. مدعومة فقط لتنسيقات MPP"
type: docs
weight: 820
url: /ar/net/aspose.tasks/tsk/notesrtf/
---
## Tsk.NotesRTF field

ملاحظات النص بتنسيق RTF. مدعومة فقط لتنسيقات MPP.

```csharp
public static readonly Key<string, TaskKey> NotesRTF;
```

## الأمثلة

يظهر كيفية قراءة/كتابة خاصية Tsk.NotesRTF.

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

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


