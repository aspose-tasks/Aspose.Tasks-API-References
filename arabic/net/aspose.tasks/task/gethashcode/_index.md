---
title: "Task.GetHashCode"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Task. تُرجع قيمة رمز تجزئة لهذه المهمة"
type: docs
weight: 1350
url: /ar/net/aspose.tasks/task/gethashcode/
---
## Task.GetHashCode method

يرجع قيمة رمز تجزئة لهذا Task.

```csharp
public override int GetHashCode()
```

### قيمة الإرجاع

تُرجع قيمة رمز تجزئة لهذا الكائن.

## الأمثلة

يُظهر كيفية الحصول على رمز تجزئة لمهمة.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

// رمز التجزئة لمهمة يعتمد على UID واسم المهمة
Console.WriteLine("Hash code of the task: " + task.GetHashCode());

task.Set(Tsk.Name, "Task 1");

Console.WriteLine("Hash code of the task: " + task.GetHashCode());
```

### انظر أيضًا

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


