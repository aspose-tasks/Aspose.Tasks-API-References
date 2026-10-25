---
title: "Tsk.IgnoreWarnings"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. يشير إلى ما إذا كان يجب إخفاء مؤشر تحذير تعارض الجدول في Microsoft Project"
type: docs
weight: 540
url: /ar/net/aspose.tasks/tsk/ignorewarnings/
---
## Tsk.IgnoreWarnings field

يحدد ما إذا كان يجب إخفاء مؤشر تحذير تعارض الجدول في Microsoft Project.

```csharp
public static readonly Key<bool, TaskKey> IgnoreWarnings;
```

## الأمثلة

يعرض كيفية قراءة/كتابة خاصية Tsk.IgnoreWarnings.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IgnoreWarnings, true);

Console.WriteLine("Ignore Warnings: " + task.Get(Tsk.IgnoreWarnings));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


