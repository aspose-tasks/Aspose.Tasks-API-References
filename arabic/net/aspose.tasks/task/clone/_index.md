---
title: "Task.Clone"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Task method. ينشئ نسخة كاملة من مهمة دون المهام الفرعية"
type: docs
weight: 1310
url: /ar/net/aspose.tasks/task/clone/
---
## Task.Clone method

ينشئ نسخة كاملة من مهمة دون المهام الفرعية.

```csharp
public object Clone()
```

### قيمة الإرجاع

تم إنشاء نسخة من مهمة.

## الأمثلة

يعرض كيفية استنساخ مهمة.

```csharp
var project = new Project();

var originalTask = project.RootTask.Children.Add("Task");
var cloneTask = (Task)originalTask.Clone();

Console.WriteLine("Are tasks equal: " + cloneTask.Equals(originalTask));
```

### انظر أيضًا

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


