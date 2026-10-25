---
title: "Tsk.FinishText"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. يُرجع نص انتهاء المهمة"
type: docs
weight: 410
url: /ar/net/aspose.tasks/tsk/finishtext/
---
## Tsk.FinishText field

يعيد نص انتهاء المهمة.

```csharp
public static readonly Key<string, TaskKey> FinishText;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Tsk.FinishText.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.FinishText, "Not A Finish");

Console.WriteLine("Finish Text: " + task.Get(Tsk.FinishText));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


