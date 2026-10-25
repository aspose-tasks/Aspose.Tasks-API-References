---
title: "WorkUnit.From"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية WorkUnit. تحصل أو تعين تاريخ From"
type: docs
weight: 20
url: /ar/net/aspose.tasks/workunit/from/
---
## WorkUnit.From property

يحصل أو يعيّن تاريخ From.

```csharp
public DateTime From { get; set; }
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


