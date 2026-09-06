---
title: "Task.ParentProject"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Task. تحصّل على المشروع الأب للمهمة"
type: docs
weight: 930
url: /ar/net/aspose.tasks/task/parentproject/
---
## Task.ParentProject property

يحصل على المشروع الأب للمهمة.

```csharp
public Project ParentProject { get; }
```

## ملاحظات

استدعِ Project.UpdateReferences لتحديث هذه الخصائص.

## الأمثلة

يوضح كيفية استخدام المشروع الأب للمهمة.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Parent");

// حدد مدة للمهمة باستخدام نوع وحدة الوقت الافتراضية للمشروع.
task.Set(Tsk.Duration, task.ParentProject.GetDuration(1));

Console.WriteLine(task.Get(Tsk.Duration));
```

### انظر أيضًا

* class [Project](../../project/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


