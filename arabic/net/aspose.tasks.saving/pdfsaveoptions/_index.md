---
title: "الفئة PdfSaveOptions"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.Saving.PdfSaveOptions. تسمح بتحديد خيارات إضافية عند عرض صفحات المشروع إلى PDF"
type: docs
weight: 2130
url: /ar/net/aspose.tasks.saving/pdfsaveoptions/
---
## PdfSaveOptions class

يسمح بتحديد خيارات إضافية عند تحويل صفحات المشروع إلى PDF.

```csharp
public class PdfSaveOptions : SaveOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions/)() | ينشئ مثيلاً جديداً من الفئة `PdfSaveOptions` التي يمكن استخدامها لحفظ مستند بتنسيق [`PDF`](../savefileformat/). |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles/) { get; set; } | يحصل أو يعيّن قائمة مثيلات الفئة [`BarStyle`](../../aspose.tasks.visualization/barstyle/) التي تظهر في عرض المشروع. |
| [Compliance](../../aspose.tasks.saving/pdfsaveoptions/compliance/) { get; set; } | يحصل أو يعيّن مستوى الامتثال المطلوب للمستند PDF المُولَّد. القيمة الافتراضية هي Pdf15. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize/) { get; set; } | يحصل أو يعيّن حجم الصفحة المخصص بالنقاط (نقطة واحدة = 1/72 بوصة). |
| [DigitalSignatureDetails](../../aspose.tasks.saving/pdfsaveoptions/digitalsignaturedetails/) { get; set; } | يحصل أو يعيّن تفاصيل التوقيع الرقمي. إذا لم يتم تعيينه، فلن يتم أي توقيع. |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب رسم وقت عدم العمل (القيمة الافتراضية هي TRUE). |
| [EncryptionDetails](../../aspose.tasks.saving/pdfsaveoptions/encryptiondetails/) { get; set; } | يحصل أو يعيّن تفاصيل التشفير. إذا لم يتم تعيينه، فلن يتم أي تشفير. |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate/) { get; set; } | يحصل أو يعيّن تاريخ الانتهاء من عملية العرض. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب زيادة ارتفاع الصف ليتناسب مع محتواه. |
| [FontSettings](../../aspose.tasks.saving/pdfsaveoptions/fontsettings/) { get; } | يحدد إعدادات الخط المستخدمة عند عرض رؤية المشروع. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines/) { get; set; } | يحصل أو يعيّن قائمة من [`Gridline`](../../aspose.tasks.visualization/gridline/) التي تظهر في عرض المشروع. |
| [IsPortrait](../../aspose.tasks.saving/saveoptions/isportrait/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان اتجاه الصفحة عموديًا؛ تُعيد false إذا كان اتجاه الصفحة أفقيًا. |
| [LegendDrawingOptions](../../aspose.tasks.saving/saveoptions/legenddrawingoptions/) { get; set; } | يحصل أو يعيّن قيمة تحدد كيفية عرض وسيلة الإيضاح. القيمة الافتراضية هي LegendDrawingOptions.OnEveryPage. |
| [LegendItems](../../aspose.tasks.saving/saveoptions/legenditems/) { get; set; } | يحصل أو يعيّن مصفوفة من PageLegendItem التي تحدد أي الأشرطة يجب عرضها في وسيلة إيضاح الصفحة. إذا كانت null، تُعرض العناصر الافتراضية. |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب عرض المهام الحرجة باللون الأحمر (القيمة الافتراضية هي FALSE). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor/) { get; set; } | يحصل أو يعيّن لون وقت عدم العمل. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount/) { get; } | يحصل أو يعيّن عدد صفحات المشروع. |
| [Pages](../../aspose.tasks.saving/pdfsaveoptions/pages/) { get; set; } | يحصل أو يعيّن قائمة أرقام الصفحات التي سيتم حفظها عند حفظ تخطيط المشروع إلى ملفات منفصلة. سيتم حفظ جميع الصفحات إذا كانت هذه القائمة فارغة. |
| [PageSavingCallback](../../aspose.tasks.saving/pdfsaveoptions/pagesavingcallback/) { get; set; } | يحصل أو يعيّن رد اتصال معرف من قبل المستخدم يُستخدم للحصول على تدفق إخراج لكل صفحة مُعرضة. يُطبق عندما يتم استخدام خيار [`SaveToSeparateFiles`](./savetoseparatefiles/). |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | يحصل أو يعيّن حجم الصفحة التي سيتم عرضها (القيمة الافتراضية هي PageSize.A4). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | يحصل أو يعيّن الـ [`PresentationFormat`](../saveoptions/presentationformat/) الذي سيُحفظ به المستند. |
| [ReduceFooterGap](../../aspose.tasks.saving/pdfsaveoptions/reducefootergap/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب تقليل الفجوة بين المهمة الأخيرة وتذييل الصفحة. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب عرض المشروع في صفحة واحدة عندما يُحفظ المشروع بصيغة رسومية. سيتم تغيير حجم الصفحة بحيث يتناسب المشروع المعروض على صفحة واحدة. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب وضع علامة على المهام الفرعية في شريط مهمة الملخص. بالنسبة للمهام الفرعية، يشير حقل Rollup إلى ما إذا كانت معلومات أشرطة جانت للمهام الفرعية ستُدمج في شريط مهمة الملخص. بالنسبة لمهام الملخص، يشير حقل Rollup إلى ما إذا كان شريط مهمة الملخص يعرض أشرطة مدمجة. يجب أن يكون حقل Rollup لمهام الملخص مضبوطًا على Yes لتتمكن أي مهام فرعية من الدمج معها. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | يحصل أو يعيّن التنسيق الذي سيتم حفظ المستند به إذا تم استخدام كائن خيارات الحفظ هذا. |
| [SaveToSeparateFiles](../../aspose.tasks.saving/pdfsaveoptions/savetoseparatefiles/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان سيتم حفظ صفحات المشروع إلى ملفات منفصلة. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | يحصل أو يعيّن التاريخ الذي يبدأ منه العرض. |
| [TaskLinkDrawingCallback](../../aspose.tasks.saving/saveoptions/tasklinkdrawingcallback/) { get; set; } | يحصل أو يعيّن رد الاتصال الذي يمكن استخدامه لتخصيص بعض جوانب عرض روابط المهام. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | يحصل أو يعيّن المقارن لفرز المهام على مخطط جانت ومخطط ورقة المهام. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | يحصل أو يعيّن الشرط المستخدم لتصفية المهام المعروضة على مخططات جانت، ورقة المهام، واستخدام المهام. |
| [TextCompression](../../aspose.tasks.saving/pdfsaveoptions/textcompression/) { get; set; } | يحصل أو يعيّن نوع الضغط الذي سيُستخدم لجميع تدفقات المحتوى باستثناء الصور. القيمة الافتراضية هي Flate. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | يحصل أو يعيّن قائمة أنماط النص التي تُطبق أثناء عرض منظور المشروع. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | يحصل أو يعيّن قيمة [`Timescale`](../saveoptions/timescale/) التي تُستخدم للتحكم في طريقة عرض المقياس الزمني (إن وجد) عند حفظ المشروع بتنسيق رسومي. |
| [TimescaleFitBehavior](../../aspose.tasks.saving/saveoptions/timescalefitbehavior/) { get; set; } | يحصل أو يعيّن سلوكًا يحدد كيفية محاذاة الطرف الأيمن للمقياس الزمني مع نهاية الصفحة. |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب استخدام فرشاة تدرجية عند عرض مخطط جانت. |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | يحصل أو يعيّن قائمة بأعمدة العرض التي سيتم عرضها ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)). إذا لم يتم تعيينها فستُعرض فقط معرفات المهام، أسماء المهام، البداية والنهاية. إذا تم تعيين كل من خاصيتي View و[`ViewSettings`](../saveoptions/viewsettings/)، فإن الأعمدة من View تتجاوز الأعمدة من ViewSettings. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | يحصل أو يعيّن منظورًا ([`View`](../saveoptions/view/)) للعرض. يمكنك استخدام هذا الخيار لتحديد بشكل صريح أي منظور يجب حفظه بتنسيقات PDF أو HTML أو Image. إذا تم تعيين هذه الخاصية، يتم تجاهل خاصية [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) عند حفظ المشروع. يجب أن يكون المنظر من إحدى الشاشات التالية (([`Screen`](../../aspose.tasks/view/screen/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage). |

## الأمثلة

يوضح كيفية حفظ الصفحات المختارة لمشروع في ملف PDF.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");
var options = new PdfSaveOptions();
options.RenderToSinglePage = false;
options.Pages = new List<int>();

// دعنا نتحقق من عدد الصفحات التي يمكن تصديرها
Console.WriteLine("Page Count: " + options.PageCount);

options.Pages.Add(1);
options.Pages.Add(4);
project.Save(OutDir + "SaveToMultiplePDFFiles_out.pdf", options);
```

### انظر أيضًا

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


