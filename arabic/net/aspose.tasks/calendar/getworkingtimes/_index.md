---
title: "Calendar.GetWorkingTimes"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Calendar. تُرجع WorkingTimeCollection لأوقات العمل للتاريخ المحدد"
type: docs
weight: 240
url: /ar/net/aspose.tasks/calendar/getworkingtimes/
---
## Calendar.GetWorkingTimes method

تُرجع [`WorkingTimeCollection`](../../workingtimecollection/) لأوقات العمل للتاريخ المحدد.

```csharp
public WorkingTimeCollection GetWorkingTimes(DateTime dt)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| dt | DateTime | التاريخ للحصول على أوقات العمل. |

### قيمة الإرجاع

مجموعة من مثيلات [`WorkingTime`](../../workingtime/).

## الأمثلة

يظهر كيفية الحصول على أوقات العمل لتاريخ محدد.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// احصل على أوقات العمل لتاريخ محدد
var workingTimes = calendar.GetWorkingTimes(new DateTime(2020, 4, 8, 8, 0, 0));

// سيتم طباعة 16 ساعة
foreach (var workingTime in workingTimes)
{
    Console.WriteLine("From: " + workingTime.From);
    Console.WriteLine("To: " + workingTime.To);
}
```

### انظر أيضًا

* class [WorkingTimeCollection](../../workingtimecollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


