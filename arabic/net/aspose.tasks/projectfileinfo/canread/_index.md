---
title: "ProjectFileInfo.CanRead"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ProjectFileInfo. يحصل على قيمة تشير إلى ما إذا كان يمكن لـ Aspose.Tasks معالجة ملف المشروع"
type: docs
weight: 10
url: /ar/net/aspose.tasks/projectfileinfo/canread/
---
## ProjectFileInfo.CanRead property

يحصل على قيمة تشير إلى ما إذا كان Aspose.Tasks يمكنه معالجة ملف المشروع.

```csharp
public bool CanRead { get; }
```

## الأمثلة

يوضح كيفية قراءة معلومات ملف المشروع.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### انظر أيضًا

* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


