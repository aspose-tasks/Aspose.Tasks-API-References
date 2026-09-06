---
title: "الفئة SaveOptions"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.Saving.SaveOptions. هذه فئة أساسية مجردة للفئات التي تسمح للمستخدم بتحديد خيارات إضافية عند حفظ مشروع بتنسيق معين."
type: docs
weight: 2190
url: /ar/net/aspose.tasks.saving/saveoptions/
---
## SaveOptions class

هذه فئة أساسية مجردة للفئات التي تسمح للمستخدم بتحديد خيارات إضافية عند حفظ المشروع بتنسيق معين.

```csharp
public abstract class SaveOptions : SimpleSaveOptions
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles/) { get; set; } | يحصل أو يعيّن قائمة مثيلات الفئة [`BarStyle`](../../aspose.tasks.visualization/barstyle/) التي تظهر في عرض المشروع. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize/) { get; set; } | يحصل أو يعيّن حجم الصفحة المخصص بالنقاط (نقطة واحدة = 1/72 بوصة). |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب رسم وقت عدم العمل (القيمة الافتراضية هي TRUE). |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate/) { get; set; } | يحصل أو يعيّن تاريخ الانتهاء من عملية العرض. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب زيادة ارتفاع الصف ليتناسب مع محتواه. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines/) { get; set; } | يحصل أو يعيّن قائمة من [`Gridline`](../../aspose.tasks.visualization/gridline/) التي تظهر في عرض المشروع. |
| [IsPortrait](../../aspose.tasks.saving/saveoptions/isportrait/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان اتجاه الصفحة عموديًا؛ تُعيد false إذا كان اتجاه الصفحة أفقيًا. |
| [LegendDrawingOptions](../../aspose.tasks.saving/saveoptions/legenddrawingoptions/) { get; set; } | يحصل أو يعيّن قيمة تحدد كيفية عرض وسيلة الإيضاح. القيمة الافتراضية هي LegendDrawingOptions.OnEveryPage. |
| [LegendItems](../../aspose.tasks.saving/saveoptions/legenditems/) { get; set; } | يحصل أو يعيّن مصفوفة من PageLegendItem التي تحدد أي الأشرطة يجب عرضها في وسيلة إيضاح الصفحة. إذا كانت null، تُعرض العناصر الافتراضية. |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب عرض المهام الحرجة باللون الأحمر (القيمة الافتراضية هي FALSE). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor/) { get; set; } | يحصل أو يعيّن لون وقت عدم العمل. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount/) { get; } | يحصل أو يعيّن عدد صفحات المشروع. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | يحصل أو يعيّن حجم الصفحة التي سيتم عرضها (القيمة الافتراضية هي PageSize.A4). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | يحصل أو يعيّن الـ[`PresentationFormat`](./presentationformat/) الذي سيُحفظ به المستند. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب عرض المشروع في صفحة واحدة عندما يُحفظ المشروع بصيغة رسومية. سيتم تغيير حجم الصفحة بحيث يتناسب المشروع المعروض على صفحة واحدة. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب وضع علامة على المهام الفرعية في شريط مهمة الملخص. بالنسبة للمهام الفرعية، يشير حقل Rollup إلى ما إذا كانت معلومات أشرطة جانت للمهام الفرعية ستُدمج في شريط مهمة الملخص. بالنسبة لمهام الملخص، يشير حقل Rollup إلى ما إذا كان شريط مهمة الملخص يعرض أشرطة مدمجة. يجب أن يكون حقل Rollup لمهام الملخص مضبوطًا على Yes لتتمكن أي مهام فرعية من الدمج معها. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | يحصل أو يعيّن التنسيق الذي سيتم حفظ المستند به إذا تم استخدام كائن خيارات الحفظ هذا. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | يحصل أو يعيّن التاريخ الذي يبدأ منه العرض. |
| [TaskLinkDrawingCallback](../../aspose.tasks.saving/saveoptions/tasklinkdrawingcallback/) { get; set; } | يحصل أو يعيّن رد الاتصال الذي يمكن استخدامه لتخصيص بعض جوانب عرض روابط المهام. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | يحصل أو يعيّن المقارن لفرز المهام على مخطط جانت ومخطط ورقة المهام. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | يحصل أو يعيّن الشرط المستخدم لتصفية المهام المعروضة على مخططات جانت، ورقة المهام، واستخدام المهام. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | يحصل أو يعيّن قائمة أنماط النص التي تُطبق أثناء عرض منظور المشروع. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | يحصل أو يعيّن قيمة الـ[`Timescale`](./timescale/) المستخدمة للتحكم في كيفية عرض مقياس الوقت (إن وجد) عند حفظ المشروع بتنسيق رسومي. |
| [TimescaleFitBehavior](../../aspose.tasks.saving/saveoptions/timescalefitbehavior/) { get; set; } | يحصل أو يعيّن سلوكًا يحدد كيفية محاذاة الطرف الأيمن للمقياس الزمني مع نهاية الصفحة. |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب استخدام فرشاة تدرجية عند عرض مخطط جانت. |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | يحصل أو يعيّن قائمة بأعمدة العرض التي سيتم عرضها ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)). إذا لم يتم تعيينها فستُعرض فقط معرفات المهام، أسماء المهام، تاريخ البدء والانتهاء. إذا تم تعيين كل من خاصيتي View و[`ViewSettings`](./viewsettings/)، فإن الأعمدة من View تتجاوز الأعمدة من ViewSettings. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | يحصل أو يعيّن عرضًا ([`View`](./view/)) للعرض. يمكنك استخدام هذه الخيارات لتحديد صراحةً أي عرض يجب حفظه بصيغة PDF أو HTML أو صورة. إذا تم تعيين هذه الخاصية، يتم تجاهل خاصية [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) عند حفظ المشروع. يجب أن يكون العرض من إحدى الشاشات التالية (([`Screen`](../../aspose.tasks/view/screen/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage). |

## ملاحظات

يتم تمرير مثيل لأي فئة مشتقة من الفئة SaveOptions إلى عمليات التحميل عبر الدفق أو السلسلة لتحديد خيارات مخصصة عند حفظ المستند.

## الأمثلة

يعرض كيفية ضبط الخيار لتحديد ما إذا كان يجب زيادة ارتفاع الصف ليتناسب مع محتواه.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    // ضبط خيار ملاءمة المحتوى إلى true
    FitContent = true,
    Timescale = Timescale.Months,
    PresentationFormat = PresentationFormat.TaskUsage
};
project.Save(OutDir + "FitContentsToCellSize_out.pdf", options);
```

### انظر أيضًا

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


