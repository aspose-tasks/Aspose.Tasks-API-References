---
title: "TaskLink.SuccTask"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية TaskLink. تحصل أو تعين المهمة اللاحقة"
type: docs
weight: 80
url: /ar/net/aspose.tasks/tasklink/succtask/
---
## TaskLink.SuccTask property

يحصل أو يعيّن مهمة المتابع.

```csharp
public Task SuccTask { get; set; }
```

## الأمثلة

يوضح كيفية قراءة روابط مهام المشروع.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

// عرض أسماء مهام السلف والمتابع
foreach (var taskLink in project.TaskLinks)
{
    Console.WriteLine("Predecessor: " + taskLink.PredTask.Get(Tsk.Name));
    Console.WriteLine("Successor: " + taskLink.SuccTask.Get(Tsk.Name));
    Console.WriteLine("Lag Format: " + taskLink.LagFormat);
    Console.WriteLine("Link Lag: " + taskLink.LinkLag);
    Console.WriteLine();
}
```

### انظر أيضًا

* class [Task](../../task/)
* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


