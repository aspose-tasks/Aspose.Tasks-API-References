---
title: "Tsk.IsRollup"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. يحدد ما إذا كانت المعلومات حول أشرطة جانت للمهام الفرعية سيتم تجميعها إلى شريط المهمة الملخصة"
type: docs
weight: 690
url: /ar/net/aspose.tasks/tsk/isrollup/
---
## Tsk.IsRollup field

يحدد ما إذا كانت معلومات أشرطة جانت للمهام الفرعية ستُدمج في شريط مهمة الملخص.

```csharp
public static readonly Key<NullableBool, TaskKey> IsRollup;
```

## الأمثلة

يعرض كيفية قراءة/كتابة خاصية Tsk.IsRollup.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsRollup, true);

Console.WriteLine("Is Rollup: " + task.Get(Tsk.IsRollup));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


