---
title: "CalendarCollection.Add"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة CalendarCollection. تُضيف تقويمًا أساسيًا جديدًا إلى كائن CalendarCollection هذا وتُرجع التقويم المُضاف"
type: docs
weight: 20
url: /ar/net/aspose.tasks/calendarcollection/add/
---
## Add(string) {#add}

يضيف تقويمًا أساسيًا جديدًا إلى كائن CalendarCollection هذا ويعيد التقويم المضاف.

```csharp
public Calendar Add(string name)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| الاسم | سلسلة | اسم التقويم. |

### قيمة الإرجاع

تم إضافة كائن [`Calendar`](../../calendar/).

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentException | يُرمى عندما يكون اسم التقويم null. |

## الأمثلة

يوضح كيفية إنشاء تقويم قياسي.

```csharp
var project = new Project();

// عرّف تقويمًا واجعله قياسيًا
var calendar = project.Calendars.Add("New Standard Calendar");
Calendar.MakeStandardCalendar(calendar);

project.Save(OutDir + "MakeAStandardCalendar_out.xml", SaveFileFormat.Xml);
```

### انظر أيضًا

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string, Calendar) {#add_1}

يضيف تقويمًا جديدًا مع تقويم أساسي محدد إلى كائن CalendarCollection هذا ويعيد التقويم المضاف.

```csharp
public Calendar Add(string name, Calendar baseCalendar)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| الاسم | سلسلة | الاسم المحدد. |
| baseCalendar | Calendar | التقويم الأساسي المحدد. |

### قيمة الإرجاع

تم إضافة كائن [`Calendar`](../../calendar/).

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


