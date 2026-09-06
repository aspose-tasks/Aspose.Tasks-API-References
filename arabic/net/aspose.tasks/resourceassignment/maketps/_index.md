---
title: "ResourceAssignment.MakeTPs"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ResourceAssignment. تُنشئ قائمة من بيانات الوقت المرحلية"
type: docs
weight: 740
url: /ar/net/aspose.tasks/resourceassignment/maketps/
---
## ResourceAssignment.MakeTPs method

ينشئ قائمة بالبيانات المتدرجة زمنياً.

```csharp
public DateTime MakeTPs(DateTime start, TimeSpan time, Calendar calendar, 
    List<TimephasedData> list, bool isWorking, int type)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| بداية | DateTime | تاريخ البدء المحدد. |
| الوقت | TimeSpan | وقت العمل المحدد. |
| تقويم | Calendar | تقويم العمل المحدد. |
| قائمة | List`1 | قائمة بيانات الوقت المرحلية. |
| isWorking | Boolean | العلم المحدد الذي يحدد ما إذا كانت بيانات الوقت المرحلية عاملة أم لا. |
| نوع | Int32 | نوع بيانات الوقت المرحلية المحدد. |

### قيمة الإرجاع

تاريخ أقصى من القائمة أو تاريخ البدء إذا كانت القائمة فارغة.

## الأمثلة

يوضح كيفية إنشاء TPs باستخدام المعلمات.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 3, 30, 8, 0, 0));
var resource = project.Resources.Add("Resource");
var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Start, new DateTime(2020, 4, 1, 8, 0, 0));

var tps = new List<TimephasedData>();
var lastDate = assignment.MakeTPs(
    assignment.Get(Asn.Start),
    TimeSpan.FromHours(32),
    project.Calendars.GetByName("Standard"),
    tps,
    true,
    (int)TimephasedDataType.AssignmentRemainingWork);

foreach (var data in tps)
{
    Console.WriteLine("Start: " + data.Start);
    Console.WriteLine("Finish: " + data.Finish);
    Console.WriteLine("TimephasedDataType: " + data.TimephasedDataType);
    Console.WriteLine();
}
```

### انظر أيضًا

* class [Calendar](../../calendar/)
* class [TimephasedData](../../timephaseddata/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


