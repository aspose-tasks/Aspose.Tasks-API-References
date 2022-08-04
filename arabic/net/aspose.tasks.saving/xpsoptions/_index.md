---
title: XpsOptions
second_title: Aspose.Tasks لمرجع .NET API
description: يسمح بتحديد خيارات إضافية عند عرض صفحات المشروع على XPS.
type: docs
weight: 1980
url: /ar/net/aspose.tasks.saving/xpsoptions/
---
## XpsOptions class

يسمح بتحديد خيارات إضافية عند عرض صفحات المشروع على XPS.

```csharp
public class XpsOptions : SaveOptions
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [XpsOptions](xpsoptions)() | يقوم بتهيئة مثيل جديد لملف[`XpsOptions`](../xpsoptions) فئة . |

## الخصائص

| اسم | وصف |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles) { get; set; } | الحصول على أو تعيين قائمة مثيلات ملف[`BarStyle`](../../aspose.tasks.visualization/barstyle) الفئة التي تظهر في عرض المشروع. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize) { get; set; } | الحصول على أو تعيين حجم الصفحة المخصص بالنقاط (نقطة واحدة = 1/72 بوصة) . |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان يجب رسم وقت غير العمل (القيمة الافتراضية هي TRUE) . |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate) { get; set; } | الحصول على أو تحديد تاريخ انتهاء التقديم إلى. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان يجب زيادة ارتفاع الصف ليناسب محتواه. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines) { get; set; } | يحصل أو يحدد قائمة[`Gridline`](../../aspose.tasks.visualization/gridline) التي تظهر في عرض المشروع. |
| [LegendOnEachPage](../../aspose.tasks.saving/saveoptions/legendoneachpage) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان يجب عرض وسيلة الإيضاح في كل صفحة (القيمة الافتراضية هي TRUE) . |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان يجب عرض المهام الهامة باللون الأحمر (القيمة الافتراضية هي FALSE) . |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor) { get; set; } | الحصول على أو تعيين لون وقت غير العمل. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount) { get; } | الحصول على أو تحديد عدد صفحات المشروع. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize) { get; set; } | الحصول على أو تحديد حجم الصفحة المراد عرضها (القيمة الافتراضية هي PageSize.A4) . |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat) { get; set; } | يحصل أو يحدد ملف[`PresentationFormat`](../saveoptions/presentationformat) حيث سيتم حفظ المستند. |
| [RenderMetafileAsBitmap](../../aspose.tasks.saving/xpsoptions/rendermetafileasbitmap) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان يجب تقديم ملف تعريف كصورة نقطية. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان يجب تقديم مشروع إلى صفحة واحدة عند حفظ المشروع بتنسيق رسومي. سيتم تغيير حجم الصفحة بحيث يمكن احتواء المشروع المعروض في صفحة واحدة. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars) { get; set; } | الحصول على قيمة أو تعيينها تشير إلى ما إذا كان يجب وضع علامة على المهام الفرعية على شريط المهام الموجزة. بالنسبة للمهام الفرعية ، يشير حقل "التجميع" إلى ما إذا كانت المعلومات الموجودة في أشرطة جانت للمهام الفرعية سيتم عرضها في شريط المهام الموجزة. يشير الحقل إلى ما إذا كان شريط المهام الموجزة يعرض أشرطة مجمعة . يجب أن يكون لديك حقل "التجميع" للمهام الموجزة معينًا إلى "نعم" لأية مهام فرعية ليتم عرضها عليها. |
| [SaveFormat](../../aspose.tasks.saving/saveoptions/saveformat) { get; } | الحصول على أو تحديد التنسيق الذي سيتم حفظ المستند به إذا تم استخدام كائن خيارات الحفظ هذا. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate) { get; set; } | الحصول على أو تحديد تاريخ بدء العرض من . |
| [TasksComparer](../../aspose.tasks.saving/saveoptions/taskscomparer) { get; set; } | الحصول على المقارنة أو تعيينها لفرز المهام على مخطط جانت ومخطط ورقة المهام. |
| [TasksFilter](../../aspose.tasks.saving/saveoptions/tasksfilter) { get; set; } | الحصول على أو تعيين الشرط الذي يتم استخدامه لتصفية المهام المعروضة على مخططات استخدام ورقة جانت وورقة المهام والمهام. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles) { get; set; } | الحصول على أو تعيين قائمة مثيلات ملف[`TextStyle`](../../aspose.tasks.visualization/textstyle) الفئة التي تظهر في عرض المشروع. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale) { get; set; } | يحصل أو يحدد ملف[`Timescale`](../saveoptions/timescale) القيمة التي تُستخدم للتحكم في كيفية عرض المقياس الزمني (إن وجد) عند حفظ المشروع بتنسيق رسومي. |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان يجب استخدام فرشاة التدرج عند عرض مخطط جانت. |
| [View](../../aspose.tasks.saving/saveoptions/view) { get; set; } | الحصول على أو تعيين قائمة بأعمدة العرض المراد عرضها ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn) ) . إذا لم يتم تعيينها ، فسيتم عرض معرفات المهام وأسماء المهام والبدء والنهاية فقط.[`ViewSettings`](../saveoptions/viewsettings) تم تعيين الخصائص ، الأعمدة من عرض تتجاوز الأعمدة من ViewSettings . |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings) { get; set; } | الحصول على عرض أو تعيينه ([`View`](../saveoptions/view) لتقديمه. يمكنك استخدام هذه الخيارات لتحديد طريقة العرض التي يجب حفظها بتنسيق PDF أو HTML أو صورة بشكل صريح . إذا تم تعيين هذه الخاصية ،[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat) يتم تجاهل الخاصية عند حفظ المشروع. يجب أن يكون العرض من إحدى الشاشات التالية (([`Screen`](../../aspose.tasks/view/screen) )): (جانت ، TaskSheet ، TaskUsage ، ResourceSheet ، ResourceUsage) |

### أنظر أيضا

* class [SaveOptions](../saveoptions)
* مساحة الاسم [Aspose.Tasks.Saving](../../aspose.tasks.saving)
* المجسم [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
