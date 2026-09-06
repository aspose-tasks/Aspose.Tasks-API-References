---
title: "Tsk.IsNull"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. يحدد ما إذا كانت المهمة مهمة فارغة."
type: docs
weight: 640
url: /ar/net/aspose.tasks/tsk/isnull/
---
## Tsk.IsNull field

يحدد ما إذا كانت المهمة مهمة فارغة.

```csharp
public static readonly Key<NullableBool, TaskKey> IsNull;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Tsk.IsNull.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsNull, true);

Console.WriteLine("Is Null: " + task.Get(Tsk.IsNull));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


