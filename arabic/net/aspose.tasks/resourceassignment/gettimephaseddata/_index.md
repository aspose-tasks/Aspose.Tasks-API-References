---
title: "ResourceAssignment.GetTimephasedData"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ResourceAssignment. تُرجع فئة TimephasedDataCollection التي تحتوي على مثيلات فئة TimephasedData ضمن تواريخ البدء والنهاية المحددة لنوع TimephasedDataType المحدد"
type: docs
weight: 720
url: /ar/net/aspose.tasks/resourceassignment/gettimephaseddata/
---
## GetTimephasedData(DateTime, DateTime, TimephasedDataType) {#gettimephaseddata_1}

تُرجع فئة [`TimephasedDataCollection`](../../timephaseddatacollection/) التي تحتوي على مثيلات فئة [`TimephasedData`](../timephaseddata/) ضمن تواريخ البدء والنهاية المحددة لنوع [`TimephasedDataType`](../../timephaseddatatype/).

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end, 
    TimephasedDataType timephasedType)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| بداية | DateTime | تاريخ البدء للبيانات المرحلية. |
| نهاية | DateTime | تاريخ النهاية للبيانات المرحلية. |
| timephasedType | TimephasedDataType | نوع البيانات المرحلية ([`TimephasedDataType`](../../timephaseddatatype/)). |

### قيمة الإرجاع

تُرجع قائمة تحتوي على مثيلات فئة [`TimephasedData`](../../timephaseddata/).

## الأمثلة

يظهر كيفية إنشاء بيانات زمنية لتعيين مورد ضمن نطاق تاريخ.

```csharp
var project = new Project(DataDir + "ReadWriteTimephasedData.mpp");

// تعيين خصائص المشروع
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

// تعيين مخطط Backloaded، يزيد من مدة المهمة من 6 إلى 10 أيام
assn.Set(Asn.WorkContour, WorkContourType.BackLoaded);

project.SetBaseline(BaselineType.Baseline);
task.Set(Tsk.PercentComplete, 50);

// الحصول على بيانات زمنية
List<TimephasedData> td = assn.GetTimephasedData(assn.Get(Asn.Start), assn.Get(Asn.Finish), TimephasedDataType.AssignmentRemainingWork).ToList();
Console.WriteLine(td.Count);
foreach (var timePhasedValue in td)
{
    Console.WriteLine(timePhasedValue.Value);
}
```

### انظر أيضًا

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedData(DateTime, DateTime) {#gettimephaseddata}

تُرجع كائن [`TimephasedDataCollection`](../../timephaseddatacollection/) مع مثيلات فئة [`TimephasedData`](../timephaseddata/) ضمن تواريخ البدء والنهاية المحددة لعمل AssignmentWork.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| بداية | DateTime | تاريخ البدء للبيانات المرحلية. |
| نهاية | DateTime | تاريخ النهاية للبيانات المرحلية. |

### قيمة الإرجاع

تُرجع قائمة تحتوي على مثيلات فئة [`TimephasedData`](../../timephaseddata/).

## الأمثلة

يظهر كيفية إنشاء بيانات زمنية لتعيين مورد ضمن نطاق تاريخ.

```csharp
var project = new Project(DataDir + "ReadWriteTimephasedData.mpp");

// تعيين خصائص المشروع
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

// تعيين مخطط Backloaded، يزيد من مدة المهمة من 6 إلى 10 أيام
assn.Set(Asn.WorkContour, WorkContourType.BackLoaded);

project.SetBaseline(BaselineType.Baseline);
task.Set(Tsk.PercentComplete, 50);

// الحصول على بيانات زمنية
List<TimephasedData> td = assn.GetTimephasedData(assn.Get(Asn.Start), assn.Get(Asn.Finish), TimephasedDataType.AssignmentRemainingWork).ToList();
Console.WriteLine(td.Count);
foreach (var timePhasedValue in td)
{
    Console.WriteLine(timePhasedValue.Value);
}
```

### انظر أيضًا

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


