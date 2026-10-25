---
title: "Task.OutlineIndent"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Task. تُدرج مهمة في المخطط"
type: docs
weight: 1380
url: /ar/net/aspose.tasks/task/outlineindent/
---
## Task.OutlineIndent method

يقوم بزيادة إزاحة مهمة في المخطط.

```csharp
public void OutlineIndent()
```

## الأمثلة

يعرض كيفية إدراج مهمة.

```csharp
var project = new Project();
var task1 = project.RootTask.Children.Add("Parent");
var task2 = project.RootTask.Children.Add("Task");
Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));

// إدرج المهمة
task2.OutlineIndent();

Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));
```

### انظر أيضًا

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


