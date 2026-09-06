---
title: "TaskLink.LinkLag"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية TaskLink. تحصل أو تعين التأخير بوحدات من عشر دقيقة أو كنسبة مئوية"
type: docs
weight: 40
url: /ar/net/aspose.tasks/tasklink/linklag/
---
## TaskLink.LinkLag property

يحصل أو يعيّن التأخير بوحدات من عشرة دقيقة أو كنسبة مئوية.

```csharp
public int LinkLag { get; set; }
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

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


