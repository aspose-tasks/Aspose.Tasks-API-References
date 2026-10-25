---
title: "Task.Predecessors"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Task. تحصل على كائن TaskCollection الذي يحتوي على جميع سابقي كائن Task هذا"
type: docs
weight: 980
url: /ar/net/aspose.tasks/task/predecessors/
---
## Task.Predecessors property

تحصل على كائن [`TaskCollection`](../../taskcollection/) الذي يحتوي على جميع سابقي كائن Task هذا.

```csharp
public TaskCollection Predecessors { get; }
```

### قيمة الإرجاع

مثيل للقراءة فقط من فئة [`TaskCollection`](../../taskcollection/).

## الأمثلة

يظهر كيفية قراءة سابقي المهمة.

```csharp
var project = new Project();
var pred = project.RootTask.Children.Add("Predecessor");
var succ = project.RootTask.Children.Add("Successor");

project.TaskLinks.Add(pred, succ);

foreach (var predecessor in succ.Predecessors)
{
    Console.WriteLine("{0} {1}", predecessor.Get(Tsk.Id), predecessor.Get(Tsk.Name));
}
```

### انظر أيضًا

* class [TaskCollection](../../taskcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


