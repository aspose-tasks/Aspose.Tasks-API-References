---
title: "PageMargins.Bottom"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية PageMargins. يحصل أو يعيّن حجم الهامش السفلي بالسنتيمترات"
type: docs
weight: 30
url: /ar/net/aspose.tasks.visualization/pagemargins/bottom/
---
## PageMargins.Bottom property

يحصل أو يعيّن حجم الهامش السفلي بالسنتيمترات.

```csharp
public double Bottom { get; set; }
```

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

* class [PageMargins](../)
* namespace [Aspose.Tasks.Visualization](../../pagemargins/)
* assembly [Aspose.Tasks](../../../)


