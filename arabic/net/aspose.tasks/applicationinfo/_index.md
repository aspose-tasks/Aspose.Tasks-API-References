---
title: "تعداد ApplicationInfo"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.ApplicationInfo. يحدد نسخة المشروع التي تم إنشاء الملف فيها"
type: docs
weight: 10
url: /ar/net/aspose.tasks/applicationinfo/
---
## ApplicationInfo enumeration

يحدد نسخة المشروع التي تم إنشاء الملف فيها.

```csharp
public enum ApplicationInfo
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Undefined | `0` | لا يمكن تعريفه. |
| MSP2000 | `1` | تم إنشاء الملف في Microsoft Project 2000/2002. |
| MSP2003 | `2` | تم إنشاء الملف في Microsoft Project 2003. |
| MSP2007 | `3` | تم إنشاء الملف في Microsoft Project 2007. |
| MSP2010 | `4` | تم إنشاء الملف في Microsoft Project 2010. |
| MSP2013 | `5` | تم إنشاء الملف في Microsoft Project 2013. |
| MSP2016 | `6` | تم إنشاء الملف في Microsoft Project 2016. |

## الأمثلة

يعرض كيفية التحقق من معلومات تطبيق المشروع.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


