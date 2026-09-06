---
title: "CalendarException.Delete"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة CalendarException. تحذف كائن Exception من كائن CalendarExceptionCollection التابع للتقويم الأصلي"
type: docs
weight: 180
url: /ar/net/aspose.tasks/calendarexception/delete/
---
## CalendarException.Delete method

يحذف مثيل Exception من كائن التقويم الأب CalendarExceptionCollection.

```csharp
public void Delete()
```

## الأمثلة

يوضح كيفية حذف استثناء تقويم.

```csharp
var project = new Project(DataDir + "CalendarExceptions.mpp");

var calendar = project.Calendars.ToList()[0];

Console.WriteLine("Calendar Name: " + calendar.Name);
Console.WriteLine("Calendar Exception Count: " + calendar.Exceptions.Count);

// إزالة الاستثناء
calendar.Exceptions[0].Delete();

Console.WriteLine("Calendar Exception Count: " + calendar.Exceptions.Count);
```

### انظر أيضًا

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


