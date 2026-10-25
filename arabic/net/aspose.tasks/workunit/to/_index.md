---
title: "WorkUnit.To"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية WorkUnit. تحصل أو تعين تاريخ To"
type: docs
weight: 30
url: /ar/net/aspose.tasks/workunit/to/
---
## WorkUnit.To property

يحصل أو يعيّن تاريخ To.

```csharp
public DateTime To { get; set; }
```

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


