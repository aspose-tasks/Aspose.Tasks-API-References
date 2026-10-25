---
title: "Calendar.IsBaselineCalendar"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Calendar. تحصل أو تعين قيمة تشير إلى ما إذا كان التقويم تقويمًا أساسيًا للخط الأساسي"
type: docs
weight: 80
url: /ar/net/aspose.tasks/calendar/isbaselinecalendar/
---
## Calendar.IsBaselineCalendar property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان التقويم تقويمًا خط أساس.

```csharp
public bool IsBaselineCalendar { get; set; }
```

## الأمثلة

يظهر كيفية التحقق مما إذا كان التقويم تقويمًا أساسيًا للخط الأساسي أم لا.

```csharp
var project = new Project(DataDir + "IsBaselineCalendar.mpp");

var calendar = project.Calendars.GetByUid(3);

Console.WriteLine("Is baseline calendar: " + calendar.IsBaselineCalendar);
```

### انظر أيضًا

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


