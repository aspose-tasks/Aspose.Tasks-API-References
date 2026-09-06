---
title: "TaskUtils.TaskChildrenCount"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة TaskUtils. تحسب بشكل متكرر عدد مهام الأطفال عبر جميع المستويات."
type: docs
weight: 40
url: /ar/net/aspose.tasks.util/taskutils/taskchildrencount/
---
## TaskUtils.TaskChildrenCount method

يحسب بشكل متكرر عدد مهام الأطفال لمهمة عبر جميع المستويات.

```csharp
public static int TaskChildrenCount(Task task)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| مهمة | مهمة | المهمة التي يتم حساب أطفالها. |

### قيمة الإرجاع

عدد الأطفال.

## الأمثلة

يظهر كيفية استخدام طريقة &lt;see cref=\"Aspose.Tasks.Util.TaskUtils.TaskChildrenCount\" /&gt;.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// تحسب بشكل متكرر عدد مهام الأطفال للمهمة عبر جميع المستويات.
var count = TaskUtils.TaskChildrenCount(project.RootTask);

Console.WriteLine("Number of tasks: " + count);
```

### انظر أيضًا

* class [Task](../../../aspose.tasks/task/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


