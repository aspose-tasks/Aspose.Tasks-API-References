---
title: "ProjectFileInfo.GetHashCode"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ProjectFileInfo. تُرجع قيمة رمز تجزئة للمثيلة من فئة ProjectFileInfo"
type: docs
weight: 60
url: /ar/net/aspose.tasks/projectfileinfo/gethashcode/
---
## ProjectFileInfo.GetHashCode method

تُرجع قيمة رمز تجزئة للمثيلة من فئة [`ProjectFileInfo`](../).

```csharp
public override int GetHashCode()
```

### قيمة الإرجاع

تُرجع قيمة رمز تجزئة لهذا الكائن.

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


