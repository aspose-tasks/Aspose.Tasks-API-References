---
title: "CalendarCollection.Count"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية CalendarCollection. تحصل على عدد الكائنات الموجودة في كائن CalendarCollection هذا"
type: docs
weight: 10
url: /ar/net/aspose.tasks/calendarcollection/count/
---
## CalendarCollection.Count property

تحصل على عدد الكائنات الموجودة في كائن [`CalendarCollection`](../) هذا.

```csharp
public int Count { get; }
```

## الأمثلة

يوضح كيفية التكرار على مجموعة التقويم.

```csharp
var project = new Project(DataDir + "Project5.mpp");

Console.WriteLine("Number of calendars in the project: " + project.Calendars.Count);
List<Calendar> calendars = project.Calendars.ToList();
foreach (var calendar in calendars)
{
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### انظر أيضًا

* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


