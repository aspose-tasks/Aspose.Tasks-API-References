---
title: "CalendarCollection.GetByName"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة CalendarCollection. تُرجع تقويمًا بالاسم المحدد"
type: docs
weight: 30
url: /ar/net/aspose.tasks/calendarcollection/getbyname/
---
## CalendarCollection.GetByName method

يعيد تقويمًا بالاسم المحدد.

```csharp
public Calendar GetByName(string name)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| الاسم | سلسلة | اسم تقويم. |

### قيمة الإرجاع

إذا وُجد، تُرجع التقويم بالاسم المحدد وإلا تُرجع null.

## الأمثلة

يوضح كيفية الحصول على التقويمات بالاسم أو بالمعرف.

```csharp
var project = new Project(DataDir + "Project5.mpp");

var calendarByName = project.Calendars.GetByName("TestCalendar");
var calendarByUid = project.Calendars.GetByUid(4);

Console.WriteLine("Calendar Name: " + calendarByName.Name);
Console.WriteLine("Calendar Name: " + calendarByUid.Name);
Console.WriteLine("Are calendars equals: " + calendarByName.Equals(calendarByUid));
```

### انظر أيضًا

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


