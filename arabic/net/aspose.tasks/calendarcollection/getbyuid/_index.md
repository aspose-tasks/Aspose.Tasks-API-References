---
title: "CalendarCollection.GetByUid"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة CalendarCollection. تُرجع تقويمًا بالمعرف UID المحدد"
type: docs
weight: 40
url: /ar/net/aspose.tasks/calendarcollection/getbyuid/
---
## CalendarCollection.GetByUid method

يعيد تقويمًا بالمعرف UID المحدد.

```csharp
public Calendar GetByUid(int uid)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| uid | Int32 | معرف UID لتقويم. |

### قيمة الإرجاع

تقويم بمعرف UID محدد.

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


