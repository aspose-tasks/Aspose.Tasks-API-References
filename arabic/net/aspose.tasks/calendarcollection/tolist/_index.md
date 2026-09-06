---
title: "CalendarCollection.ToList"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة CalendarCollection. تحوّل كائن CalendarCollection إلى قائمة من كائنات Calendar."
type: docs
weight: 70
url: /ar/net/aspose.tasks/calendarcollection/tolist/
---
## CalendarCollection.ToList method

تحوّل كائن CalendarCollection إلى قائمة من كائنات [`Calendar`](../../calendar/)

```csharp
public List<Calendar> ToList()
```

### قيمة الإرجاع

قائمة من كائنات [`Calendar`](../../calendar/)

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

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


