---
title: "TimelineView.TimelineView"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ TimelineView. يهيئ حالة جديدة من فئة TimelineView"
type: docs
weight: 10
url: /ar/net/aspose.tasks/timelineview/timelineview/
---
## TimelineView constructor

يهيئ حالة جديدة من الفئة [`TimelineView`](../).

```csharp
public TimelineView()
```

## الأمثلة

يظهر كيفية العمل مع &lt;see cref="Aspose.Tasks.TimelineView" /&gt;.

```csharp
var project = new Project();

// تهيئة عرض زمني
var view = new TimelineView();

// ضبط قيمة تشير إلى كيفية تنسيق التواريخ في عرض Timeline.
view.DateFormat = DateFormat.DateDddDd;
// ضبط قيمة تشير إلى ما إذا كان سيتم عرض المهام المتداخلة على عدة صفوف.
view.DisplayOverlapped = true;
// ضبط قيمة تشير إلى ما إذا كان سيتم إظهار التحكم في التحريك والتكبير.
view.ShowPanZoom = true;
// ضبط قيمة تشير إلى ما إذا كان سيتم إظهار مقياس الوقت.
view.ShowTimescale = true;
// ضبط قيمة تشير إلى ما إذا كان سيتم عرض خط يمثل اليوم.
view.ShowToday = true;
// ضبط قيمة تشير إلى عدد الخطوط المستخدمة لعرض المهمة في المخطط الزمني.
view.TextLinesCount = 2;

// يحصل على قيمة تشير إلى ما إذا كان سيتم عرض المهام المتداخلة على عدة صفوف.
Console.WriteLine("Show Dates: " + view.ShowDates);

// إضافة العرض إلى المشروع
project.Views.Add(view);

// إضافة بعض بيانات الاختبار إلى المشروع
var task1 = project.RootTask.Children.Add("Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 4, 29, 8, 0, 0));
task1.Set(Tsk.Duration, task1.ParentProject.GetDuration(24, TimeUnitType.Hour));
var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Start, new DateTime(2020, 4, 29, 8, 0, 0));
task2.Set(Tsk.Duration, task1.ParentProject.GetDuration(40, TimeUnitType.Hour));

project.Save(OutDir + "SetTimeScaleCount_out.pdf", SaveFileFormat.Pdf);
```

### انظر أيضًا

* class [TimelineView](../)
* namespace [Aspose.Tasks](../../timelineview/)
* assembly [Aspose.Tasks](../../../)


