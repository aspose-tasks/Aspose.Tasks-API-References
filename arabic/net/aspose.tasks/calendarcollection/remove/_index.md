---
title: "CalendarCollection.Remove"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة CalendarCollection. تُزيل التقويم من مجموعة تقويم المشروع CalendarCollection"
type: docs
weight: 60
url: /ar/net/aspose.tasks/calendarcollection/remove/
---
## CalendarCollection.Remove method

يزيل Calendar من مجموعة CalendarCollection الخاصة بالمشروع.

```csharp
public bool Remove(Calendar item)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| العنصر | Calendar | التقويم المراد إزالته. |

### قيمة الإرجاع

إذا تم الإزالة تُعيد true، وإلا تُعيد false.

### استثناءات

| استثناء | شرط |
| --- | --- |
| InvalidOperationException | يُرمى عندما لا يمكن إزالة التقويم. |

## الأمثلة

يوضح كيفية استبدال تقويم في مجموعة التقويم.

```csharp
var project = new Project(DataDir + "Project5.mpp");

var calendar = project.Calendars.GetByName("TestCalendar");
if (calendar != null)
{
    project.Calendars.Remove(calendar);
}

// إضافة تقويم جديد
project.Calendars.Add("New Calendar");
project.Save(OutDir + "ReplaceCalendarWithNewCalendar_out.mpp", SaveFileFormat.Mpp);
```

### انظر أيضًا

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


