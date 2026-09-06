---
title: "CalendarCollection.GetEnumerator"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة CalendarCollection. تُرجع عدادًا لهذه المجموعة."
type: docs
weight: 50
url: /ar/net/aspose.tasks/calendarcollection/getenumerator/
---
## CalendarCollection.GetEnumerator method

يرجع عدادًا لهذه المجموعة.

```csharp
public IEnumerator<Calendar> GetEnumerator()
```

### قيمة الإرجاع

عداد لهذه المجموعة.

## الأمثلة

يوضح كيفية إضافة تقويمات جديدة.

```csharp
var project = new Project();

// يمكن إضافة تقويمات جديدة إلى مجموعة تقويمات المشروع باستخدام التحميلات الزائدة للدالة Add في المجموعة.
project.Calendars.Add("Calendar");
var newCalendar = project.Calendars.Add("Parent");
project.Calendars.Add("Child", newCalendar);

foreach (var calendar in project.Calendars)
{
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### انظر أيضًا

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


