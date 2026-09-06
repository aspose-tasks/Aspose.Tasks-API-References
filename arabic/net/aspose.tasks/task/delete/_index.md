---
title: "Task.Delete"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Task. تحذف مهمة من مجموعة مهام المشروع الأصل وجميع تعييناتها"
type: docs
weight: 1320
url: /ar/net/aspose.tasks/task/delete/
---
## Task.Delete method

يحذف مهمة من مجموعة مهام المشروع الأصل وجميع تعييناتها.

```csharp
public void Delete()
```

## الأمثلة

يعرض كيفية حذف مهمة.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Number of tasks: " + project.RootTask.Children.Count);

// حذف مهمة
task.Delete();

Console.WriteLine("Number of tasks: " + project.RootTask.Children.Count);
```

### انظر أيضًا

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


