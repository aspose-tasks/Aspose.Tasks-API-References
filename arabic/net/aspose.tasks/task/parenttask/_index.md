---
title: "Task.ParentTask"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Task. يحصل على مهمة الأصل لمهمة"
type: docs
weight: 940
url: /ar/net/aspose.tasks/task/parenttask/
---
## Task.ParentTask property

يحصل على المهمة الأب للمهمة.

```csharp
public Task ParentTask { get; }
```

## الأمثلة

يوضح كيفية استخدام مهمة الأصل لمهمة.

```csharp
var project = new Project();
var parent = project.RootTask.Children.Add("Parent");
var child1 = parent.Children.Add("Child1");
var child2 = child1.ParentTask.Children.Add("Child2");

Console.WriteLine("Is parent is equal to the root task: " + child2.ParentTask.Equals(parent));
```

### انظر أيضًا

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


