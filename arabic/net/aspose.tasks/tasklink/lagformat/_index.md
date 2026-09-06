---
title: "TaskLink.LagFormat"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية TaskLink. تحصل أو تعين الصيغة لتعبير التأخير"
type: docs
weight: 30
url: /ar/net/aspose.tasks/tasklink/lagformat/
---
## TaskLink.LagFormat property

يحصل أو يعيّن التنسيق لتعبير عن تنسيق التأخير.

```csharp
public TimeUnitType LagFormat { get; set; }
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

* enum [TimeUnitType](../../timeunittype/)
* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


