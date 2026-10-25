---
title: "الفئة ProjectFileInfo"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.ProjectFileInfo. تحتوي نسخة الفئة على معلومات حول تنسيق ملف المشروع وإصدار Microsoft Project الذي تم إنشاء الملف فيه."
type: docs
weight: 1460
url: /ar/net/aspose.tasks/projectfileinfo/
---
## ProjectFileInfo class

تحتوي نسخة الفئة على معلومات حول تنسيق ملف المشروع وإصدار Microsoft Project الذي تم إنشاء الملف به.

```csharp
public sealed class ProjectFileInfo : IEquatable<ProjectFileInfo>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CanRead](../../aspose.tasks/projectfileinfo/canread/) { get; } | يحصل على قيمة تشير إلى ما إذا كان Aspose.Tasks يمكنه معالجة ملف المشروع. |
| [IsPasswordProtected](../../aspose.tasks/projectfileinfo/ispasswordprotected/) { get; } | يحصل على قيمة تشير إلى ما إذا كان المشروع محميًا بكلمة مرور. |
| [ProjectApplicationInfo](../../aspose.tasks/projectfileinfo/projectapplicationinfo/) { get; } | يحصل على معلومات تطبيق ملف المشروع. |
| [ProjectFileFormat](../../aspose.tasks/projectfileinfo/projectfileformat/) { get; } | يحصل على تنسيق ملف المشروع. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| override [Equals](../../aspose.tasks/projectfileinfo/equals/#equals_1)(object) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد. |
| [Equals](../../aspose.tasks/projectfileinfo/equals/#equals)(ProjectFileInfo) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد. |
| override [GetHashCode](../../aspose.tasks/projectfileinfo/gethashcode/)() | يعيد قيمة رمز تجزئة (hash code) لنسخة الفئة `ProjectFileInfo`. |

## ملاحظات

استخدم خاصية CanRead لتحديد أن المكتبة يمكنها معالجة ملف المشروع.

## الأمثلة

يوضح كيفية قراءة معلومات ملف المشروع.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


