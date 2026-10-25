---
title: "ProjectFileInfo.ProjectApplicationInfo"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ProjectFileInfo. تُعيد معلومات تطبيق ملف المشروع"
type: docs
weight: 30
url: /ar/net/aspose.tasks/projectfileinfo/projectapplicationinfo/
---
## ProjectFileInfo.ProjectApplicationInfo property

يحصل على معلومات تطبيق ملف المشروع.

```csharp
public ApplicationInfo ProjectApplicationInfo { get; }
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

* enum [ApplicationInfo](../../applicationinfo/)
* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


