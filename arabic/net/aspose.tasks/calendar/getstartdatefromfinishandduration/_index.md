---
title: "Calendar.GetStartDateFromFinishAndDuration"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Calendar. تُرجع تاريخ البدء بناءً على تاريخ الانتهاء المحدد والمدة"
type: docs
weight: 200
url: /ar/net/aspose.tasks/calendar/getstartdatefromfinishandduration/
---
## GetStartDateFromFinishAndDuration(DateTime, Duration) {#getstartdatefromfinishandduration}

يرجع تاريخ البدء بناءً على تاريخ الانتهاء المحدد والمدة.

```csharp
public DateTime GetStartDateFromFinishAndDuration(DateTime finish, Duration duration)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| انتهاء | DateTime | تاريخ الانتهاء المحدد. |
| المدة | المدة | المدة المحددة. |

### قيمة الإرجاع

تاريخ البدء المحسوب.

## الأمثلة

يعرض كيفية الحصول على تاريخ البدء بواسطة تاريخ الانتهاء والمدة.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// احصل على تاريخ البدء بواسطة تاريخ الانتهاء ومدة
var startDate = calendar.GetStartDateFromFinishAndDuration(new DateTime(2020, 4, 10, 9, 0, 0), project.GetDuration(16, TimeUnitType.Hour));

// سيتم طباعة 8 أبريل 2020 9:00 ص
Console.WriteLine(startDate);
```

### انظر أيضًا

* struct [Duration](../../duration/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetStartDateFromFinishAndDuration(DateTime, TimeSpan) {#getstartdatefromfinishandduration_1}

يرجع تاريخ البدء بناءً على تاريخ الانتهاء المحدد والمدة.

```csharp
public DateTime GetStartDateFromFinishAndDuration(DateTime finish, TimeSpan duration)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| انتهاء | DateTime | تاريخ الانتهاء المحدد. |
| المدة | TimeSpan | المدة المحددة. |

### قيمة الإرجاع

تاريخ البدء المحسوب.

## الأمثلة

يعرض كيفية الحصول على تاريخ البدء بواسطة تاريخ الانتهاء والمدة (كفترة زمنية).

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// احصل على تاريخ البدء بواسطة تاريخ الانتهاء ومدة
var startDate = calendar.GetStartDateFromFinishAndDuration(new DateTime(2020, 4, 10, 9, 0, 0), TimeSpan.FromHours(16));

// سيتم طباعة 8 أبريل 2020 9:00 ص
Console.WriteLine(startDate);
```

### انظر أيضًا

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


