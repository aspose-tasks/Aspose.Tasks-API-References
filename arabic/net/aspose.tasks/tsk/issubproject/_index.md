---
title: "Tsk.IsSubproject"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. يحدد ما إذا كانت المهمة مشروعًا مدرجًا"
type: docs
weight: 700
url: /ar/net/aspose.tasks/tsk/issubproject/
---
## Tsk.IsSubproject field

يحدد ما إذا كانت المهمة مشروعًا مُدرجًا.

```csharp
public static readonly Key<bool, TaskKey> IsSubproject;
```

## الأمثلة

يظهر كيفية قراءة/كتابة خاصية Tsk.IsSubproject.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsSubproject, true);

Console.WriteLine("Is Subproject: " + task.Get(Tsk.IsSubproject));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


