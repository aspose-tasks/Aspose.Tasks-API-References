---
title: "الفئة TaskLink"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.TaskLink. تمثل رابط سلف"
type: docs
weight: 2410
url: /ar/net/aspose.tasks/tasklink/
---
## TaskLink class

يمثّل ارتباطًا سلفيًا.

```csharp
public sealed class TaskLink : IEquatable<TaskLink>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CrossProjectName](../../aspose.tasks/tasklink/crossprojectname/) { get; set; } | يحصل أو يعيّن المشروع السلف الخارجي. |
| [IsCrossProject](../../aspose.tasks/tasklink/iscrossproject/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان السلف جزءًا من مشروع آخر. |
| [LagFormat](../../aspose.tasks/tasklink/lagformat/) { get; set; } | يحصل أو يعيّن التنسيق لتعبير عن تنسيق التأخير. |
| [LinkLag](../../aspose.tasks/tasklink/linklag/) { get; set; } | يحصل أو يعيّن التأخير بوحدات من عشرة دقيقة أو كنسبة مئوية. |
| [LinkLagTimeSpan](../../aspose.tasks/tasklink/linklagtimespan/) { get; set; } | يحصل أو يعيّن مدة التأخير، اعتمادًا على LagFormat. |
| [LinkType](../../aspose.tasks/tasklink/linktype/) { get; set; } | يحصل أو يعيّن نوع الرابط. |
| [PredTask](../../aspose.tasks/tasklink/predtask/) { get; set; } | يحصل أو يعيّن مهمة السلف. |
| [SuccTask](../../aspose.tasks/tasklink/succtask/) { get; set; } | يحصل أو يعيّن مهمة المتابع. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| override [Equals](../../aspose.tasks/tasklink/equals/#equals_1)(object) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد. |
| [Equals](../../aspose.tasks/tasklink/equals/#equals)(TaskLink) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد. |
| override [GetHashCode](../../aspose.tasks/tasklink/gethashcode/)() | يرجع قيمة تجزئة (hash code) للنسخة من الفئة `TaskLink`. |
| override [ToString](../../aspose.tasks/tasklink/tostring/)() | يرجع تمثيلًا نصيًا لـ TaskLink. التفاصيل الدقيقة للتمثيل غير محددة وقد تتغير. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


