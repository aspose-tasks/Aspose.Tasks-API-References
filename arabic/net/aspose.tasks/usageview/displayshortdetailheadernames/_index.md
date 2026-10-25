---
title: "UsageView.DisplayShortDetailHeaderNames"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية UsageView. يحصل على أو يعيّن قيمة تشير إلى ما إذا كان يجب عرض أسماء رؤوس التفاصيل المختصرة أم لا"
type: docs
weight: 40
url: /ar/net/aspose.tasks/usageview/displayshortdetailheadernames/
---
## UsageView.DisplayShortDetailHeaderNames property

يحصل أو يضبط قيمة تشير إلى ما إذا كان سيتم عرض أسماء رؤوس التفاصيل القصيرة أم لا.

```csharp
public bool DisplayShortDetailHeaderNames { get; set; }
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


