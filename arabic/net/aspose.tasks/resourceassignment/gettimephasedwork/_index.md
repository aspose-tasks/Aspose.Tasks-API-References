---
title: "ResourceAssignment.GetTimephasedWork"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ResourceAssignment. تحصل على مقدار العمل المتدرج زمنياً للفترة الزمنية المحددة"
type: docs
weight: 730
url: /ar/net/aspose.tasks/resourceassignment/gettimephasedwork/
---
## GetTimephasedWork(DateTime, DateTime, TimephasedDataType) {#gettimephasedwork_1}

يحصل على مقدار العمل المتدرج زمنياً للفترة الزمنية المحددة.

```csharp
public TimeSpan GetTimephasedWork(DateTime start, DateTime end, 
    TimephasedDataType timephasedDataType)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| بداية | DateTime | بداية الفترة الزمنية. |
| نهاية | DateTime | نهاية الفترة الزمنية. |
| timephasedDataType | TimephasedDataType | نوع البيانات المتدرجة زمنياً للاستخدام. |

## الأمثلة

يظهر كيفية حساب عمل التعيين لفترة زمنية عشوائية.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var assignment = project.ResourceAssignments.GetByUid(2);

// اطبع عمل التعيين لكل ساعة.
for (DateTime hour = assignment.Start; hour <= assignment.Finish; hour = hour.AddHours(1))
{
    var work = assignment.GetTimephasedWork(hour, hour.AddHours(1), TimephasedDataType.AssignmentWork);
    Console.WriteLine("{0} : {1:N2}", hour, work.TotalHours);
}
```

### انظر أيضًا

* enum [TimephasedDataType](../../timephaseddatatype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedWork(DateTime, DateTime) {#gettimephasedwork}

يحصل على مقدار العمل المتدرج زمنياً للفترة الزمنية المحددة.

```csharp
public TimeSpan GetTimephasedWork(DateTime start, DateTime end)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| بداية | DateTime | بداية الفترة الزمنية. |
| نهاية | DateTime | نهاية الفترة الزمنية. |

### انظر أيضًا

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


