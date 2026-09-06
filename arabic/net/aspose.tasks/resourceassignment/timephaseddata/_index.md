---
title: "ResourceAssignment.TimephasedData"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ResourceAssignment. تحصل أو تعيين مثيل فئة TimephasedDataCollection التي تحتوي على عناصر فئة TimephasedData"
type: docs
weight: 600
url: /ar/net/aspose.tasks/resourceassignment/timephaseddata/
---
## ResourceAssignment.TimephasedData property

تحصل أو تعيين مثيل فئة [`TimephasedDataCollection`](../../timephaseddatacollection/) التي تحتوي على عناصر فئة `TimephasedData`.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## الأمثلة

يظهر كيفية قراءة بيانات timephased لتعيين مورد.

```csharp
var project = new Project(DataDir + "ReadWriteTimephasedData.mpp");
project.Set(Prj.StartDate, new DateTime(2013, 10, 30, 9, 0, 0));
project.Set(Prj.NewTasksAreManual, false);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Duration, project.GetDuration(6));

var rsc = project.Resources.Add("Rsc");
rsc.Set(Rsc.StandardRate, 10);
rsc.Set(Rsc.OvertimeRate, 15);

// إنشاء تعيين مورد
var assn = project.ResourceAssignments.Add(task, rsc);
assn.Set(Asn.Stop, DateTime.MinValue);
assn.Set(Asn.Resume, DateTime.MinValue);
assn.Set(Asn.WorkContour, WorkContourType.BackLoaded);

// الحصول على بيانات زمنية
foreach (var td in assn.TimephasedData)
{
    Console.WriteLine(td.Value);
}
```

### انظر أيضًا

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


