---
title: "الفئة BuildVersionInfo"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.BuildVersionInfo. تحتوي على نسخة البناء ومعلومات المنتج"
type: docs
weight: 160
url: /ar/net/aspose.tasks/buildversioninfo/
---
## BuildVersionInfo class

يحتوي على إصدار البناء ومعلومات المنتج.

```csharp
public static class BuildVersionInfo
```

## الحقول

| الاسم | الوصف |
| --- | --- |
| static readonly [AssemblyInformationalVersion](../../aspose.tasks/buildversioninfo/assemblyinformationalversion/) | رقم النسخة الإعلامية للتجميع. |
| static readonly [AssemblyVersion](../../aspose.tasks/buildversioninfo/assemblyversion/) | نسخة التجميع. |
| static readonly [FileVersion](../../aspose.tasks/buildversioninfo/fileversion/) | نسخة الملف. |
| static readonly [Product](../../aspose.tasks/buildversioninfo/product/) | اسم المنتج. |

## الأمثلة

يعرض كيفية قراءة معلومات نسخة البناء لـ Aspose.Tasks.

```csharp
// قراءة المعلومات العامة حول نسخة Aspose.Tasks الحالية
Console.WriteLine("Product: " + BuildVersionInfo.Product);
Console.WriteLine("File Version: " + BuildVersionInfo.FileVersion);
Console.WriteLine("Assembly Version: " + BuildVersionInfo.AssemblyVersion);
Console.WriteLine("Assembly Informational Version: " + BuildVersionInfo.AssemblyInformationalVersion);
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


