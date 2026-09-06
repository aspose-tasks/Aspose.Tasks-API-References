---
title: "RecurringInterval.DailyWorkday"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية RecurringInterval. تحصل أو تعيين قيمة تشير إلى ما إذا كان اليوم يوم عمل لخطوط التقدم اليومية"
type: docs
weight: 30
url: /ar/net/aspose.tasks.visualization/recurringinterval/dailyworkday/
---
## RecurringInterval.DailyWorkday property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان اليوم يوم عمل لخطوط التقدم اليومية.

```csharp
public bool DailyWorkday { get; set; }
```

## الأمثلة

يظهر كيفية إضافة فترة متكررة يومية لخطوط التقدم.

```csharp
var project = new Project(DataDir + "Project2007.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[1];

view.ProgressLines.RecurringInterval = new RecurringInterval();
// تعيين رقم يوم النمط اليومي
view.ProgressLines.RecurringInterval.DailyDayNumber = 2;
// تعيين قيمة تشير إلى ما إذا كان اليوم يوم عمل لخطوط التقدم اليومية.
view.ProgressLines.RecurringInterval.DailyWorkday = true;
```

### انظر أيضًا

* class [RecurringInterval](../)
* namespace [Aspose.Tasks.Visualization](../../recurringinterval/)
* assembly [Aspose.Tasks](../../../)


