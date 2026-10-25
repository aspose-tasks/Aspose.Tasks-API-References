---
title: "Tsk.DisplayAsSummary"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. يحدد ما إذا كان يجب عرض المهمة كمهمة ملخص. القراءة مدعومة لتنسيق XML فقط"
type: docs
weight: 280
url: /ar/net/aspose.tasks/tsk/displayassummary/
---
## Tsk.DisplayAsSummary field

يحدد ما إذا كان يجب عرض المهمة كمهمة ملخص. القراءة مدعومة فقط لتنسيق XML.

```csharp
public static readonly Key<NullableBool, TaskKey> DisplayAsSummary;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Tsk.DisplayAsSummary.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DisplayAsSummary, true);

Console.WriteLine("Display As Summary: " + task.Get(Tsk.DisplayAsSummary));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


