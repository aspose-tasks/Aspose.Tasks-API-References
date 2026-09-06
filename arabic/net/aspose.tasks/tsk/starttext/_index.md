---
title: "Tsk.StartText"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. يُرجع نص بداية المهمة."
type: docs
weight: 1030
url: /ar/net/aspose.tasks/tsk/starttext/
---
## Tsk.StartText field

يعيد نص بدء المهمة.

```csharp
public static readonly Key<string, TaskKey> StartText;
```

## الأمثلة

يعرض كيفية قراءة/كتابة الخاصية Tsk.StartText.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.StartText, "Start Task Text");

Console.WriteLine("Start Text: " + task.Get(Tsk.StartText));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


