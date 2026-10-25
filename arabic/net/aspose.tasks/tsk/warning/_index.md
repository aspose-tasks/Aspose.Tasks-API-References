---
title: "Tsk.Warning"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. يمثل العلامة التي تشير إلى أن المهمة لديها اختلافات في الجدول الزمني"
type: docs
weight: 1120
url: /ar/net/aspose.tasks/tsk/warning/
---
## Tsk.Warning field

يمثل العلامة التي تشير إلى أن المهمة لديها تناقضات في الجدول.

```csharp
public static readonly Key<bool, TaskKey> Warning;
```

## الأمثلة

يوضح كيفية قراءة تحذير المهمة.

```csharp
var project = new Project(DataDir + "schedule-conflict.mpp");
var task = project.RootTask.Children.GetById(1);
Console.WriteLine(task.Get(Tsk.Warning));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


