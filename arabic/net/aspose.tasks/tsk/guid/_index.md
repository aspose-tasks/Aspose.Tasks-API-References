---
title: "Tsk.Guid"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. الرموز التعريفية الفريدة التي تم إنشاؤها للمهمة"
type: docs
weight: 460
url: /ar/net/aspose.tasks/tsk/guid/
---
## Tsk.Guid field

الرموز التعريفية الفريدة التي تم إنشاؤها للمهمة.

```csharp
public static readonly Key<string, TaskKey> Guid;
```

## الأمثلة

يوضح كيفية قراءة/كتابة الخاصية Tsk.Guid.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Guid, "60648d59-9c2b-4dc6-bfdb-bfd38f331d61");

Console.WriteLine("Guid: " + task.Get(Tsk.Guid));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


