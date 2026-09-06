---
title: "ProjectFileInfo.ProjectFileFormat"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ProjectFileInfo. يحصل على تنسيق ملف المشروع"
type: docs
weight: 40
url: /ar/net/aspose.tasks/projectfileinfo/projectfileformat/
---
## ProjectFileInfo.ProjectFileFormat property

يحصل على تنسيق ملف المشروع.

```csharp
public FileFormat ProjectFileFormat { get; }
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

* enum [FileFormat](../../fileformat/)
* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


