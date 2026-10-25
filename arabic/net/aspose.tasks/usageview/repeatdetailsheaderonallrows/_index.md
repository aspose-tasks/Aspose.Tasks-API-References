---
title: "UsageView.RepeatDetailsHeaderOnAllRows"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية UsageView. يحصل أو يضبط قيمة تشير إلى ما إذا كان يجب تكرار رأس التفاصيل على جميع صفوف التعيين أم لا"
type: docs
weight: 60
url: /ar/net/aspose.tasks/usageview/repeatdetailsheaderonallrows/
---
## UsageView.RepeatDetailsHeaderOnAllRows property

يحصل أو يضبط قيمة تشير إلى ما إذا كان سيتم تكرار رأس التفاصيل على جميع صفوف التعيين أم لا.

```csharp
public bool RepeatDetailsHeaderOnAllRows { get; set; }
```

## الأمثلة

يوضح كيفية عرض عرض استخدام المهمة مع التفاصيل.

```csharp
var project = new Project(DataDir + "TaskUsageViewWithDetails.mpp");

// احصل على العرض
UsageView view = (TaskUsageView)project.DefaultView;

// عمود رأس التفاصيل لن يتم عرضه
view.DisplayDetailsHeaderColumn = false;
view.RepeatDetailsHeaderOnAllRows = false;
view.DisplayShortDetailHeaderNames = false;
view.AlignDetailsData = HorizontalStringAlignment.Near;
project.Save(OutDir + "task usage1_out.pdf", SaveFileFormat.Pdf);

// عرض عمود رأس التفاصيل
view.DisplayDetailsHeaderColumn = true;

// تكرار رأس التفاصيل على جميع صفوف التعيينات
view.RepeatDetailsHeaderOnAllRows = true;
view.AlignDetailsData = HorizontalStringAlignment.Far;
project.Save(OutDir + "task usage2_out.pdf", SaveFileFormat.Pdf);
```

### انظر أيضًا

* class [UsageView](../)
* namespace [Aspose.Tasks](../../usageview/)
* assembly [Aspose.Tasks](../../../)


