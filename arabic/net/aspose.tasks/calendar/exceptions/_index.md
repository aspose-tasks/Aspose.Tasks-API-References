---
title: "Calendar.Exceptions"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Calendar. يحصل على كائن CalendarExceptionCollection. مجموعة الاستثناءات المرتبطة بالتقويم."
type: docs
weight: 50
url: /ar/net/aspose.tasks/calendar/exceptions/
---
## Calendar.Exceptions property

يحصل على كائن CalendarExceptionCollection. مجموعة الاستثناءات المرتبطة بالتقويم.

```csharp
public CalendarExceptionCollection Exceptions { get; }
```

## الأمثلة

يعرض كيفية استرجاع معلومات حول استثناءات التقويم.

```csharp
var project = new Project(DataDir + "project_RetrieveExceptions_test.mpp");

// التكرار عبر التقويمات
foreach (var calendar in project.Calendars)
{
    // الوصول إلى استثناءات التقويم
    foreach (var exception in calendar.Exceptions)
    {
        Console.WriteLine("From: " + exception.FromDate.ToShortDateString());
        Console.WriteLine("To: " + exception.ToDate.ToShortDateString());
    }
}
```

### انظر أيضًا

* class [CalendarExceptionCollection](../../calendarexceptioncollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


