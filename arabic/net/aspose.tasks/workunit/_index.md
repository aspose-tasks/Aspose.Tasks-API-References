---
title: "الفئة WorkUnit"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.WorkUnit. تمثّل ساعات العمل"
type: docs
weight: 3630
url: /ar/net/aspose.tasks/workunit/
---
## WorkUnit class

يمثل ساعات العمل.

```csharp
public class WorkUnit
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [WorkUnit](workunit/)(DateTime, DateTime) | يُهيئ نسخة جديدة من الفئة `WorkUnit`. ينشئ كائن WorkUnit جديد بالتواريخ المحددة From و To. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [From](../../aspose.tasks/workunit/from/) { get; set; } | يحصل أو يعيّن تاريخ From. |
| [To](../../aspose.tasks/workunit/to/) { get; set; } | يحصل أو يعيّن تاريخ To. |
| [WorkingHours](../../aspose.tasks/workunit/workinghours/) { get; set; } | يحصل أو يعيّن مدة ساعات العمل. |

## الأمثلة

يظهر كيفية العمل مع معلومات وحدة العمل.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// احصل على ساعات العمل لتاريخ محدد
var workUnit = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0), new DateTime(2020, 4, 9, 17, 0, 0));

Console.WriteLine("From: " + workUnit.From);
Console.WriteLine("To: " + workUnit.To);
Console.WriteLine("Working hours: " + workUnit.WorkingHours);
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


