---
title: "Task.Status"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Task. تحصّل على حالة المهمة"
type: docs
weight: 1160
url: /ar/net/aspose.tasks/task/status/
---
## Task.Status property

يحصل على حالة المهمة.

```csharp
public TaskStatus Status { get; }
```

## الأمثلة

يوضح كيفية الحصول على حالة المهمة.

```csharp
var project = new Project(DataDir + "TaskPercentageCompletion.mpp");

// يجب تعيين تاريخ حالة المشروع لأن حساب الحالة يستخدم تاريخ الحالة.
project.StatusDate = new DateTime(2010, 7, 9, 15, 0, 0);
foreach (var task in project.EnumerateAllChildTasks())
{
    Console.WriteLine("{0} - {1}", task.Name, task.Status);
}
```

### انظر أيضًا

* enum [TaskStatus](../../taskstatus/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


