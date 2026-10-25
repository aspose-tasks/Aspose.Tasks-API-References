---
title: "الفئة UsageView"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.UsageView. تمثل عرض الاستخدام في مشروع"
type: docs
weight: 2650
url: /ar/net/aspose.tasks/usageview/
---
## UsageView class

يمثّل عرض الاستخدام في مشروع.

```csharp
public abstract class UsageView : View
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AlignDetailsData](../../aspose.tasks/usageview/aligndetailsdata/) { get; set; } | الحصول على أو تعيين محاذاة بيانات التفاصيل. |
| [BottomTimescaleTier](../../aspose.tasks/usageview/bottomtimescaletier/) { get; set; } | الحصول على أو تعيين إعدادات الطبقة السفلية لمقياس الوقت في العرض. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/) |
| [DisplayDetailsHeaderColumn](../../aspose.tasks/usageview/displaydetailsheadercolumn/) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان سيتم عرض عمود رأس التفاصيل في العرض أم لا. |
| [DisplayShortDetailHeaderNames](../../aspose.tasks/usageview/displayshortdetailheadernames/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كان سيتم عرض أسماء رؤوس التفاصيل القصيرة أم لا. |
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

* class [View](../view/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


