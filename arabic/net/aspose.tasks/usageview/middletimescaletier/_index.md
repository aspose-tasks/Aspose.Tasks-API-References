---
title: "UsageView.MiddleTimescaleTier"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية UsageView. يحصل أو يضبط إعدادات مستوى الوقت المتوسط للعرض. TimescaleTier"
type: docs
weight: 50
url: /ar/net/aspose.tasks/usageview/middletimescaletier/
---
## UsageView.MiddleTimescaleTier property

يحصل أو يضبط إعدادات مستوى الوقت المتوسط للعرض. [`TimescaleTier`](../../../aspose.tasks.visualization/timescaletier/).

```csharp
public TimescaleTier MiddleTimescaleTier { get; set; }
```

## الأمثلة

يعرض كيفية عرض رؤية استخدام المهمة مع إعدادات مقياس الوقت المعرفة في إعدادات العرض.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = project.Views.ToList()[2] as TaskUsageView;

view.TopTimescaleTier.Unit = TimescaleUnit.None;

view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
view.MiddleTimescaleTier.Label = DateLabel.WeekDddMDd;
view.MiddleTimescaleTier.Count = 1;

view.BottomTimescaleTier.Unit = TimescaleUnit.Days;
view.BottomTimescaleTier.Label = DateLabel.DayMmDd;
view.BottomTimescaleTier.Count = 1;

// حدد SaveOptions وحدد أنه يجب استخدام إعدادات مقياس الزمن لـ TaskUsageView.
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    PresentationFormat = PresentationFormat.TaskUsage
};

project.Save(OutDir + "TaskUsageView_CustomTimescale_out.pdf", options);
```

### انظر أيضًا

* class [TimescaleTier](../../../aspose.tasks.visualization/timescaletier/)
* class [UsageView](../)
* namespace [Aspose.Tasks](../../usageview/)
* assembly [Aspose.Tasks](../../../)


