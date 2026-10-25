---
title: "الفئة TaskUsageView"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Aspose.Tasks.TaskUsageView الفئة. يمثل عرض استخدام المهمة في مشروع."
type: docs
weight: 2480
url: /ar/net/aspose.tasks/taskusageview/
---
## TaskUsageView class

يمثّل عرض استخدام المهمة في مشروع.

```csharp
public class TaskUsageView : UsageView
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AlignDetailsData](../../aspose.tasks/usageview/aligndetailsdata/) { get; set; } | الحصول على أو تعيين محاذاة بيانات التفاصيل. |
| [BottomTimescaleTier](../../aspose.tasks/usageview/bottomtimescaletier/) { get; set; } | الحصول على أو تعيين إعدادات الطبقة السفلية لمقياس الوقت في العرض. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/) |
| [DisplayDetailsHeaderColumn](../../aspose.tasks/usageview/displaydetailsheadercolumn/) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان سيتم عرض عمود رأس التفاصيل في العرض أم لا. |
| [DisplayShortDetailHeaderNames](../../aspose.tasks/usageview/displayshortdetailheadernames/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كان سيتم عرض أسماء رؤوس التفاصيل القصيرة أم لا. |
| [FieldCollection](../../aspose.tasks/taskusageview/fieldcollection/) { get; } | يحصل على كائن [`TaskUsageViewFieldCollection`](../taskusageviewfieldcollection/) لهذا TaskUsageView. |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | يحصل أو يضبط مرشحًا يُستخدم في عرض واحد. |
| [Group](../../aspose.tasks/view/group/) { get; set; } | يحصل أو يضبط مجموعة من العرض الواحد. |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كان Microsoft Project يبرز الفلتر للعرض الواحد. |
| [MiddleTimescaleTier](../../aspose.tasks/usageview/middletimescaletier/) { get; set; } | يحصل أو يضبط إعدادات المستوى الأوسط للجدول الزمني للعرض. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/). |
| [Name](../../aspose.tasks/view/name/) { get; set; } | يحصل أو يضبط اسم كائن View. |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | يحصل على نسخة من الفئة [`PageInfo`](../view/pageinfo/). تمثل بيانات إعداد الصفحة الموجودة في تنسيق ملف mpp. |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | يحصل على الأصل لكائن View. للقراءة فقط [`Project`](../project/). |
| [RepeatDetailsHeaderOnAllRows](../../aspose.tasks/usageview/repeatdetailsheaderonallrows/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كان سيتم تكرار رأس التفاصيل على جميع صفوف التعيين أم لا. |
| [Screen](../../aspose.tasks/view/screen/) { get; } | يحصل على نوع الشاشة للعرض الواحد. للقراءة فقط [`ViewScreen`](../viewscreen/). |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كان Microsoft Project يعرض اسم العرض الواحد في قائمة العرض أو قوائم العروض الأخرى المنسدلة في الشريط. |
| [Table](../../aspose.tasks/view/table/) { get; set; } | يحصل أو يضبط جدولًا للعرض الواحد. |
| [TimescaleSizePercentage](../../aspose.tasks/usageview/timescalesizepercentage/) { get; set; } |  |
| [TopTimescaleTier](../../aspose.tasks/usageview/toptimescaletier/) { get; set; } | يحصل أو يضبط إعدادات المستوى العلوي للجدول الزمني للعرض. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/). |
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

يعرض كيفية عرض رؤية استخدام المهام مع إعدادات مقياس الزمن المحددة مسبقًا.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

// حدد SaveOptions وحدد إعدادات TimeScale المحددة مسبقًا 'Days'.
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Days,

    // اضبط تنسيق العرض إلى TaskUsage
    PresentationFormat = PresentationFormat.TaskUsage
};

var outputProject = "TaskUsageView_result_days_out.pdf";
project.Save(OutDir + outputProject, options);

// اضبط إعدادات مقياس الزمن إلى ThirdsOfMonths
options.Timescale = Timescale.ThirdsOfMonths;

outputProject = "TaskUsageView_result_thirdsOfMonths_out.pdf";
project.Save(OutDir + outputProject, options);

// اضبط إعدادات مقياس الزمن إلى Months
options.Timescale = Timescale.Months;

outputProject = "TaskUsageView_result_months_out.pdf";
project.Save(OutDir + outputProject, options);
```

### انظر أيضًا

* class [UsageView](../usageview/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


