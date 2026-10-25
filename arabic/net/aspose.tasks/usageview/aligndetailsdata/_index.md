---
title: "UsageView.AlignDetailsData"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية UsageView. يحصل على أو يعيّن محاذاة بيانات التفاصيل"
type: docs
weight: 10
url: /ar/net/aspose.tasks/usageview/aligndetailsdata/
---
## UsageView.AlignDetailsData property

الحصول على أو تعيين محاذاة بيانات التفاصيل.

```csharp
public HorizontalStringAlignment AlignDetailsData { get; set; }
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

* enum [HorizontalStringAlignment](../../../aspose.tasks.visualization/horizontalstringalignment/)
* class [UsageView](../)
* namespace [Aspose.Tasks](../../usageview/)
* assembly [Aspose.Tasks](../../../)


