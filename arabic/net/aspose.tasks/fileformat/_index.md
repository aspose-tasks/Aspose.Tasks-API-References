---
title: "تعداد FileFormat"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Aspose.Tasks.FileFormat enum. يحدد تنسيق ملف المشروع"
type: docs
weight: 590
url: /ar/net/aspose.tasks/fileformat/
---
## FileFormat enumeration

يحدد تنسيق ملف المشروع.

```csharp
public enum FileFormat
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Undefined | `0` | لا يمكن تعريفه. |
| P6XML | `1` | يمثل تنسيق Primavera P6 XML. |
| XML | `2` | تنسيق Microsoft Project XML. |
| MPP8 | `3` | تنسيق Microsoft Project 2000. |
| MPP9 | `4` | تنسيق Microsoft Project 2003. |
| MPP12 | `5` | تنسيق Microsoft Project 2007. |
| MPP14 | `6` | تنسيق Microsoft Project 2010. |
| MPT9 | `7` | تنسيق قالب Microsoft Project 2003. |
| MPT12 | `8` | تنسيق قالب Microsoft Project 2007. |
| MPT14 | `9` | تنسيق قالب Microsoft Project 2010 (2013). |
| MPX | `10` | تنسيق ملف Mpx. |
| XER | `11` | يمثل تنسيق Primavera XER. |
| HTML | `12` | يمثل تنسيق HTML. |
| ProjectServer | `13` | تم قراءة المشروع من Project Server أو Project Online. |

## الأمثلة

يعرض كيفية قراءة تنسيق ملف المشروع.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


