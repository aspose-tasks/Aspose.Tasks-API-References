---
title: "Calendar.Delete"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Calendar. تزيل Calendar من المشروع"
type: docs
weight: 140
url: /ar/net/aspose.tasks/calendar/delete/
---
## Calendar.Delete method

يزيل التقويم من المشروع.

```csharp
public void Delete()
```

## الأمثلة

يظهر كيفية حذف تقويم من مشروع.

```csharp
var project = new Project(DataDir + "BrokenCalendar.mpp");

// احصل على التقويم بالاسم
var calendar = project.Calendars.GetByName("Broken Calendar");

// حذف التقويم
calendar.Delete();
```

### انظر أيضًا

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


