---
title: "Tsk.IsResumeValid"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. يحدد ما إذا كان يمكن استئناف المهمة"
type: docs
weight: 680
url: /ar/net/aspose.tasks/tsk/isresumevalid/
---
## Tsk.IsResumeValid field

يحدد ما إذا كان يمكن استئناف المهمة.

```csharp
public static readonly Key<NullableBool, TaskKey> IsResumeValid;
```

## الأمثلة

يظهر كيفية قراءة/كتابة خاصية Tsk.IsResumeValid.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsResumeValid, true);

Console.WriteLine("Is Resume Valid: " + task.Get(Tsk.IsResumeValid));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


