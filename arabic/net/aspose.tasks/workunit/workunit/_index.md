---
title: "WorkUnit.WorkUnit"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ WorkUnit. يهيئ نسخة جديدة من فئة WorkUnit. ينشئ كائن WorkUnit جديد بالتواريخ From و To المحددة."
type: docs
weight: 10
url: /ar/net/aspose.tasks/workunit/workunit/
---
## WorkUnit constructor

يهيئ نسخة جديدة من فئة [`WorkUnit`](../). ينشئ كائن WorkUnit جديد بالتواريخ From و To المحددة.

```csharp
public WorkUnit(DateTime from, DateTime to)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| من | DateTime | تاريخ بدء ساعات العمل. |
| إلى | DateTime | تاريخ انتهاء ساعات العمل. |

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

* class [WorkUnit](../)
* namespace [Aspose.Tasks](../../workunit/)
* assembly [Aspose.Tasks](../../../)


