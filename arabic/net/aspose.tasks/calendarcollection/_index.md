---
title: "الفئة CalendarCollection"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.CalendarCollection. تمثل مجموعة من كائنات Calendar."
type: docs
weight: 240
url: /ar/net/aspose.tasks/calendarcollection/
---
## CalendarCollection class

تمثل مجموعة من [`Calendar`](../calendar/) كائنات.

```csharp
public class CalendarCollection : IList<Calendar>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.tasks/calendarcollection/count/) { get; } | يحصل على عدد الكائنات الموجودة في كائن `CalendarCollection` هذا. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.tasks/calendarcollection/add/#add)(string) | يضيف تقويمًا أساسيًا جديدًا إلى كائن CalendarCollection هذا ويعيد التقويم المضاف. |
| [Add](../../aspose.tasks/calendarcollection/add/#add_1)(string, Calendar) | يضيف تقويمًا جديدًا مع تقويم أساسي محدد إلى كائن CalendarCollection هذا ويعيد التقويم المضاف. |
| [GetByName](../../aspose.tasks/calendarcollection/getbyname/)(string) | يعيد تقويمًا بالاسم المحدد. |
| [GetByUid](../../aspose.tasks/calendarcollection/getbyuid/)(int) | يعيد تقويمًا بالمعرف UID المحدد. |
| [GetEnumerator](../../aspose.tasks/calendarcollection/getenumerator/)() | يرجع عدادًا لهذه المجموعة. |
| [Remove](../../aspose.tasks/calendarcollection/remove/)(Calendar) | يزيل Calendar من مجموعة CalendarCollection الخاصة بالمشروع. |
| [ToList](../../aspose.tasks/calendarcollection/tolist/)() | تحول كائن CalendarCollection إلى قائمة من كائنات [`Calendar`](../calendar/). |

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

* class [Calendar](../calendar/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


