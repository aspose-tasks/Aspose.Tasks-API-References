---
title: "تعداد Border"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.Visualization.Border. يحدد نوع الحدود."
type: docs
weight: 2970
url: /ar/net/aspose.tasks.visualization/border/
---
## Border enumeration

يحدد حدود النوع.

```csharp
public enum Border
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| NoBorder | `0` | بدون حدود. |
| AroundEveryPage | `1` | حول كل صفحة. |
| OutsidePages | `2` | في الصفحات الخارجية. |

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


