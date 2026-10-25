---
title: "Tsk.IsMarked"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. يوضح ما إذا كانت المهمة مُعلَّمة لإجراء إضافي أو لتحديد من نوع ما"
type: docs
weight: 620
url: /ar/net/aspose.tasks/tsk/ismarked/
---
## Tsk.IsMarked field

يعرض ما إذا كانت المهمة مُعلّمة لإجراء إضافي أو لتحديد من نوع ما.

```csharp
public static readonly Key<bool, TaskKey> IsMarked;
```

## ملاحظات

ينطبق على تنسيق ملف mpp فقط.

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Tsk.IsMarked.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsMarked, true);

Console.WriteLine("Is Marked: " + task.Get(Tsk.IsMarked));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


