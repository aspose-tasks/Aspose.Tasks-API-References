---
title: "Calendar.GetWorkingHours"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Calendar. تُعيد WorkUnit  بدء وانتهاء ومدة ساعات العمل للفترة الزمنية المحددة."
type: docs
weight: 220
url: /ar/net/aspose.tasks/calendar/getworkinghours/
---
## GetWorkingHours(DateTime, DateTime) {#getworkinghours}

إرجاع وحدة العمل - البداية، النهاية ومدة ساعات العمل للفترة الزمنية المحددة.

```csharp
public WorkUnit GetWorkingHours(DateTime start, DateTime finish)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| بداية | DateTime | تاريخ البدء للفترة. |
| انتهاء | DateTime | تاريخ الانتهاء للفترة. |

### قيمة الإرجاع

مثيل من فئة [`WorkUnit`](../../workunit/) يحتوي على بدء وانتهاء ومدة ساعات العمل.

## الأمثلة

يعرض كيفية الحصول على ساعات العمل لتواريخ محددة.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// احصل على ساعات العمل لتاريخ محدد
var workUnit = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0), new DateTime(2020, 4, 9, 17, 0, 0));

// سيتم طباعة 16 ساعة
Console.WriteLine(workUnit.WorkingHours);
```

### انظر أيضًا

* class [WorkUnit](../../workunit/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetWorkingHours(DateTime) {#getworkinghours_1}

يرجع مقدار ساعات العمل في التاريخ المحدد.

```csharp
public TimeSpan GetWorkingHours(DateTime dt)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| dt | DateTime | التاريخ للحصول على ساعات العمل. |

### قيمة الإرجاع

ساعات العمل في التاريخ المحدد.

## الأمثلة

يعرض كيفية الحصول على ساعات العمل لتاريخ محدد.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// احصل على ساعات العمل لتاريخ محدد
var workingHours = calendar.GetWorkingHours(new DateTime(2020, 4, 10));

// سيتم طباعة 8 ساعات
Console.WriteLine(workingHours.Hours);
```

### انظر أيضًا

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


