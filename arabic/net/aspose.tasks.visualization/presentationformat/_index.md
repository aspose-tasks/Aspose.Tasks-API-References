---
title: "تعداد PresentationFormat"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.Visualization.PresentationFormat. تعداد لتنسيق العرض"
type: docs
weight: 3270
url: /ar/net/aspose.tasks.visualization/presentationformat/
---
## PresentationFormat enumeration

تعداد لتنسيق العرض.

```csharp
public enum PresentationFormat
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| GanttChart | `0` | تنسيق عرض مخطط جانت. |
| TaskUsage | `1` | تنسيق عرض استخدام المهمة. |
| ResourceUsage | `2` | تنسيق عرض استخدام المورد. |
| ResourceSheet | `3` | تنسيق عرض ورقة المورد. |
| TaskSheet | `4` | تنسيق عرض ورقة المهمة. |

## الأمثلة

يعرض كيفية عرض طريقة ورقة المورد.

```csharp
var project = new Project(DataDir + "ResourceSheetView.mpp");

SaveOptions options = new PdfSaveOptions();

// اضبط تنسيق العرض إلى ورقة المورد
options.PresentationFormat = PresentationFormat.ResourceSheet;
project.Save(OutDir + "ResourceSheetView_out.pdf", options);
```

### انظر أيضًا

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


