---
title: "Project.DisplayOptions"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Project. تحصل على نسخة من الفئة ProjectDisplayOptions"
type: docs
weight: 380
url: /ar/net/aspose.tasks/project/displayoptions/
---
## Project.DisplayOptions property

تحصل على نسخة من الفئة [`ProjectDisplayOptions`](../../projectdisplayoptions/)

```csharp
public ProjectDisplayOptions DisplayOptions { get; }
```

## الأمثلة

يوضح كيفية ضبط خيارات عرض المشروع.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// عيّن قيمة تشير إلى ما إذا كان يجب عرض التحذيرات عندما يحدد Project تعارضًا محتملًا في الجدولة مع مهمة مجدولة يدويًا.
// هذا الخيار متاح لإصدار Project 2010 وما بعده.
project.DisplayOptions.ShowTaskScheduleWarnings = false;
```

### انظر أيضًا

* class [ProjectDisplayOptions](../../projectdisplayoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


