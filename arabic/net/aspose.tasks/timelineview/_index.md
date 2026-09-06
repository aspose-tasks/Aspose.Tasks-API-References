---
title: "الفئة TimelineView"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.TimelineView. تمثل عرضًا زمنيًا لمشروع."
type: docs
weight: 2580
url: /ar/net/aspose.tasks/timelineview/
---
## TimelineView class

يمثّل عرض المخطط الزمني لمشروع.

```csharp
public class TimelineView : View
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [TimelineView](timelineview/)() | يُنشئ مثيلة جديدة من الفئة `TimelineView`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [DateFormat](../../aspose.tasks/timelineview/dateformat/) { get; set; } | يحصل أو يضبط قيمة تشير إلى كيفية تنسيق التواريخ في عرض Timeline. |
| [DisplayOverlapped](../../aspose.tasks/timelineview/displayoverlapped/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كان سيتم عرض المهام المتداخلة على عدة صفوف. |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | يحصل أو يضبط مرشحًا يُستخدم في عرض واحد. |
| [Group](../../aspose.tasks/view/group/) { get; set; } | يحصل أو يضبط مجموعة من العرض الواحد. |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كان Microsoft Project يبرز الفلتر للعرض الواحد. |
| [Name](../../aspose.tasks/view/name/) { get; set; } | يحصل أو يضبط اسم كائن View. |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | يحصل على نسخة من الفئة [`PageInfo`](../view/pageinfo/). تمثل بيانات إعداد الصفحة الموجودة في تنسيق ملف mpp. |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | يحصل على الأصل لكائن View. للقراءة فقط [`Project`](../project/). |
| [Screen](../../aspose.tasks/view/screen/) { get; } | يحصل على نوع الشاشة للعرض الواحد. للقراءة فقط [`ViewScreen`](../viewscreen/). |
| [ShowDates](../../aspose.tasks/timelineview/showdates/) { get; } | يحصل على قيمة تشير إلى ما إذا كان سيتم إظهار التواريخ. |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كان Microsoft Project يعرض اسم العرض الواحد في قائمة العرض أو قوائم العروض الأخرى المنسدلة في الشريط. |
| [ShowPanZoom](../../aspose.tasks/timelineview/showpanzoom/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كان سيتم إظهار التحكم في التحريك والتكبير. |
| [ShowTimescale](../../aspose.tasks/timelineview/showtimescale/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كان سيتم إظهار مقياس الوقت. |
| [ShowToday](../../aspose.tasks/timelineview/showtoday/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كان سيتم عرض خط يمثل اليوم. |
| [Table](../../aspose.tasks/view/table/) { get; set; } | يحصل أو يضبط جدولًا للعرض الواحد. |
| [TextLinesCount](../../aspose.tasks/timelineview/textlinescount/) { get; set; } | يحصل أو يضبط قيمة تشير إلى عدد الخطوط المستخدمة لعرض المهمة في المخطط الزمني. |
| [Type](../../aspose.tasks/view/type/) { get; } | يحصل على نوع العنصر في العرض الواحد، مثل المهام أو الموارد. للقراءة فقط [`ItemType`](../itemtype/). |
| [Uid](../../aspose.tasks/view/uid/) { get; } | يحصل على المعرف الفريد للعرض. |
| [VisualObjectsPlacements](../../aspose.tasks/view/visualobjectsplacements/) { get; } | يحصل على مجموعة من الكائنات التي تمثل موضع ومظهر [`OleObject`](../oleobject/) في العرض. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [CompareTo](../../aspose.tasks/view/compareto/)(View) | يقارن النسخة الحالية مع كائن آخر من نفس النوع ويعيد عددًا صحيحًا يشير إلى ما إذا كانت النسخة الحالية تسبق أو تلي أو تقع في نفس الموضع في ترتيب الفرز كما الكائن الآخر. |
| override [Equals](../../aspose.tasks/view/equals/)(object) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد. |
| override [GetHashCode](../../aspose.tasks/view/gethashcode/)() | يعيد قيمة رمز تجزئة للنسخة من الفئة [`Resource`](../resource/). |

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

* class [View](../view/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


