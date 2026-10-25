---
title: "Task.OutlineOutdent"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Task. يرفع مهمة في المخطط"
type: docs
weight: 1390
url: /ar/net/aspose.tasks/task/outlineoutdent/
---
## Task.OutlineOutdent method

يرفع مهمة في المخطط.

```csharp
public void OutlineOutdent()
```

## الأمثلة

يعرض كيفية إلغاء إزاحة مهمة.

```csharp
var project = new Project();
var task1 = project.RootTask.Children.Add("Parent");
var task2 = task1.Children.Add("Task");
Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));

// إلغاء إزاحة المهمة
task2.OutlineOutdent();

Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));
```

### انظر أيضًا

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


