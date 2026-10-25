---
title: "الفئة PageMargins"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.Visualization.PageMargins. تمثل هوامش الصفحة للطباعة."
type: docs
weight: 3230
url: /ar/net/aspose.tasks.visualization/pagemargins/
---
## PageMargins class

يمثل هوامش الصفحة للطباعة.

```csharp
public class PageMargins
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [PageMargins](pagemargins/)() | المنشئ الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Borders](../../aspose.tasks.visualization/pagemargins/borders/) { get; set; } | يحصل أو يعيّن موضعًا لطباعة الحدود. يمكن أن يكون أحد قيم تعداد [`Border`](../border/). |
| [Bottom](../../aspose.tasks.visualization/pagemargins/bottom/) { get; set; } | يحصل أو يعيّن حجم الهامش السفلي بالسنتيمترات. |
| [Left](../../aspose.tasks.visualization/pagemargins/left/) { get; set; } | يحصل أو يعيّن حجم الهامش الأيسر بالسنتيمترات. |
| [Right](../../aspose.tasks.visualization/pagemargins/right/) { get; set; } | يحصل أو يعيّن حجم الهامش الأيمن بالسنتيمترات. |
| [Top](../../aspose.tasks.visualization/pagemargins/top/) { get; set; } | يحصل أو يعيّن حجم الهامش العلوي بالسنتيمترات. |

## الأمثلة

يعرض كيفية العمل مع هوامش الصفحة.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// دعنا نعدّل العرض الافتراضي.
var margins = project.DefaultView.PageInfo.Margins;

// دعنا نعدّل الهوامش.
margins.Left = 10d;
margins.Top = 10d;
margins.Right = 10d;
margins.Bottom = 10d;
margins.Borders = Border.OutsidePages;

project.Save(OutDir + "WorkWithPageMargins_out.mpp", SaveFileFormat.Mpp);
```

### انظر أيضًا

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


