---
title: "Task.Successors"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Task. يحصل على كائن TaskCollection الذي يحتوي على جميع الخلفاء لهذا الكائن Task"
type: docs
weight: 1200
url: /ar/net/aspose.tasks/task/successors/
---
## Task.Successors property

يحصل على كائن [`TaskCollection`](../../taskcollection/) الذي يحتوي على جميع الخلفاء لهذا الكائن Task.

```csharp
public TaskCollection Successors { get; }
```

### قيمة الإرجاع

مثيل للقراءة فقط من فئة [`TaskCollection`](../../taskcollection/).

## الأمثلة

يظهر كيفية قراءة خلفاء المهمة.

```csharp
var project = new Project();
var pred = project.RootTask.Children.Add("Predecessor");
var succ = project.RootTask.Children.Add("Successor");

project.TaskLinks.Add(pred, succ);

foreach (var successor in pred.Successors)
{
    Console.WriteLine("{0} {1}", successor.Get(Tsk.Id), successor.Get(Tsk.Name));
}
```

### انظر أيضًا

* class [TaskCollection](../../taskcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


