---
title: "Calendar.PrimaveraProperties"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Calendar. يحصل على كائن يحتوي على خصائص Primaveraspecific لتقويم تم قراءته من صيغ Primavera"
type: docs
weight: 100
url: /ar/net/aspose.tasks/calendar/primaveraproperties/
---
## Calendar.PrimaveraProperties property

يحصل على كائن يحتوي على خصائص خاصة بـ Primavera لتقويم تم قراءته من صيغ Primavera.

```csharp
public PrimaveraCalendarProperties PrimaveraProperties { get; }
```

## الأمثلة

يوضح كيفية قراءة مشروع من ملف Primavera وفحص خصائص Primavera-specific للتقويم.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 4861;

// يعيد مشروعًا بمعرف UID خاص.
var project = new Project(DataDir + "ScheduleOptions.xer", options);

var calendar = project.Calendars.GetByUid(178);

Console.WriteLine("Hours per day in '{0}' : {1}", calendar.Name, calendar.PrimaveraProperties.HoursPerDay);
```

### انظر أيضًا

* class [PrimaveraCalendarProperties](../../primaveracalendarproperties/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


