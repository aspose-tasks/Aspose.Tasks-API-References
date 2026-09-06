---
title: "Task.SelectAllChildTasks"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Task method. يجمع بشكل متكرر جميع مهام الأطفال لهذه المهمة"
type: docs
weight: 1400
url: /ar/net/aspose.tasks/task/selectallchildtasks/
---
## Task.SelectAllChildTasks method

يجمع بشكل متكرر جميع المهام الفرعية لهذه المهمة.

```csharp
public IEnumerable<Task> SelectAllChildTasks()
```

### قيمة الإرجاع

قائمة بمهام الأطفال لهذه المهمة.

## الأمثلة

يظهر كيفية التكرار على مهام الأطفال.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task 1");
task.Children.Add("Task 2");

foreach (var tsk in project.RootTask.SelectAllChildTasks())
{
    Console.WriteLine("{0} {1}", tsk.Get(Tsk.Id), tsk.Get(Tsk.Name));
}
```

### انظر أيضًا

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


