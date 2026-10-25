---
title: "TimephasedData.CreateCostTimephased"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة TimephasedData. تنشئ وتُهيئ نسخة جديدة من فئة TimephasedData للبيانات ذات الطور الزمني القائم على التكلفة"
type: docs
weight: 20
url: /ar/net/aspose.tasks/timephaseddata/createcosttimephased/
---
## CreateCostTimephased(int, DateTime, DateTime, double, TimeUnitType, TimephasedDataType) {#createcosttimephased_1}

تنشئ وتُهيئ نسخة جديدة من فئة [`TimephasedData`](../) للبيانات ذات الطور الزمني القائم على التكلفة.

```csharp
public static TimephasedData CreateCostTimephased(int uid, DateTime start, DateTime finish, 
    double value, TimeUnitType timeUnit, TimephasedDataType type)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| uid | Int32 | معرف فريد (UID) للمهمة. |
| بداية | DateTime | تاريخ ووقت البدء. |
| انتهاء | DateTime | تاريخ ووقت الانتهاء. |
| value | Double | قيمة التكلفة. |
| timeUnit | TimeUnitType | نوع وحدة الوقت. |
| نوع | TimephasedDataType | نوع البيانات ذات الطور الزمني. |

### قيمة الإرجاع

نسخة من فئة [`TimephasedData`](../) للبيانات ذات الطور الزمني القائم على التكلفة.

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentException | إذا تم تحديد قيمة تكلفة سلبية. |

## الأمثلة

يوضح كيفية العمل مع بيانات زمنية مخصصة.

```csharp
var project = new Project(DataDir + "Project1.mpp") { CalculationMode = CalculationMode.None };

var workResource = project.Resources.Add("Work Resource");
workResource.Set(Rsc.Type, ResourceType.Work);
var costResource = project.Resources.Add("Cost Resource");
costResource.Set(Rsc.Type, ResourceType.Cost);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2018, 1, 1, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

var workAssignment = project.ResourceAssignments.Add(task, workResource);
workAssignment.Set(Asn.WorkContour, WorkContourType.Contoured);
var costAssignment = project.ResourceAssignments.Add(task, costResource);
costAssignment.Set(Asn.WorkContour, WorkContourType.Contoured);

// دعنا نضيف بيانات زمنية مخصصة tds
workAssignment.TimephasedData.Clear();

// أضف أيام العمل
var td1 = TimephasedData.CreateWorkTimephased(
    workAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 2, 8, 0, 0),
    new DateTime(2018, 1, 5, 17, 0, 0),
    TimeSpan.FromHours(40),
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentRemainingWork);

// أضف عطلة نهاية الأسبوع
var td2 = TimephasedData.CreateWorkTimephased(
    workAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 6, 8, 0, 0),
    new DateTime(2018, 1, 8, 8, 0, 0),
    TimeSpan.Zero,
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentRemainingWork);

workAssignment.TimephasedData.Add(td1);
workAssignment.TimephasedData.Add(td2);

costAssignment.TimephasedData.Clear();

// أضف أيام العمل
var td11 = TimephasedData.CreateCostTimephased(
    costAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 2, 8, 0, 0),
    new DateTime(2018, 1, 5, 17, 0, 0),
    1,
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentCost);

// أضف عطلة نهاية الأسبوع
var td22 = TimephasedData.CreateCostTimephased(
    costAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 6, 8, 0, 0),
    new DateTime(2018, 1, 8, 8, 0, 0),
    0,
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentCost);

costAssignment.TimephasedData.Add(td11);
costAssignment.TimephasedData.Add(td22);

Console.WriteLine("Print assignment timephased data:");
foreach (var assignment in project.ResourceAssignments)
{
    Console.WriteLine("Assignment UID: " + assignment.Get(Asn.Uid));
    foreach (var tds in assignment.TimephasedData)
    {
        Console.WriteLine("  Uid: " + tds.Uid);
        Console.WriteLine("  Start: " + tds.Start);
        Console.WriteLine("  Finish: " + tds.Finish);
        Console.WriteLine("  Type: " + tds.TimephasedDataType);
        Console.WriteLine("  Unit: " + tds.Unit);
        Console.WriteLine("  Value: " + tds.Value);
        Console.WriteLine("  ValueToCost: " + tds.ValueToCost);
        Console.WriteLine("  ValueToDuration: " + tds.ValueToDuration);
        Console.WriteLine("  ValueToUnits: " + tds.ValueToUnits);
        Console.WriteLine();
    }
}

project.Recalculate();
```

### انظر أيضًا

* enum [TimeUnitType](../../timeunittype/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [TimephasedData](../)
* namespace [Aspose.Tasks](../../timephaseddata/)
* assembly [Aspose.Tasks](../../../)

---

## CreateCostTimephased(int, DateTime, DateTime, double, TimephasedDataType) {#createcosttimephased}

تنشئ وتُهيئ نسخة جديدة من فئة [`TimephasedData`](../) للبيانات ذات الطور الزمني القائم على التكلفة.

```csharp
public static TimephasedData CreateCostTimephased(int uid, DateTime start, DateTime finish, 
    double value, TimephasedDataType type)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| uid | Int32 | معرف فريد (UID) للمهمة. |
| بداية | DateTime | تاريخ ووقت البدء. |
| انتهاء | DateTime | تاريخ ووقت الانتهاء. |
| value | Double | قيمة التكلفة. |
| نوع | TimephasedDataType | نوع البيانات ذات الطور الزمني. |

### قيمة الإرجاع

نسخة من فئة [`TimephasedData`](../) للبيانات ذات الطور الزمني القائم على التكلفة.

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentException | إذا تم تحديد قيمة تكلفة سلبية. |

### انظر أيضًا

* enum [TimephasedDataType](../../timephaseddatatype/)
* class [TimephasedData](../)
* namespace [Aspose.Tasks](../../timephaseddata/)
* assembly [Aspose.Tasks](../../../)


