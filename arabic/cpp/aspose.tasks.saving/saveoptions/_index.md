---
title: "فئة Aspose::Tasks::Saving::SaveOptions"
linktitle: "SaveOptions"
articleTitle: "SaveOptions"
second_title: "Aspose.Tasks لـ C++"
description: "هذه فئة أساسية مجردة للفئات التي تسمح للمستخدم بتحديد خيارات إضافية عند حفظ مشروع بتنسيق معين."
type: docs
weight: 10
url: /ar/cpp/aspose.tasks.saving/saveoptions/
---

## SaveOptions class

**Inherits:** Aspose::Tasks::Saving::SimpleSaveOptions

هذه فئة أساسية مجردة للفئات التي تسمح للمستخدم بتحديد خيارات إضافية عند حفظ مشروع بتنسيق معين.

يتم تمرير مثيل لأي فئة مشتقة من فئة SaveOptions إلى عمليات التحميل Save للتيار أو Save للسلسلة لتحديد خيارات مخصصة عند حفظ المستند.

## الطرق

| الاسم | الوصف |
| --- | --- |
| [get_BarStyles](./get_barstyles/) | يحصل على قائمة بنماذج فئة BarStyle التي تظهر في عرض المشروع. |
| [get_CustomPageSize](./get_custompagesize/) | يحصل على حجم الصفحة المخصص بالنقاط (نقطة واحدة = 1/72 من البوصة). |
| [get_DrawNonWorkingTime](./get_drawnonworkingtime/) | يحصل على قيمة تشير إلى ما إذا كان يجب رسم وقت غير العمل (القيمة الافتراضية هي TRUE). |
| [get_EndDate](./get_enddate/) | يحصل على تاريخ لإنهاء العرض. |
| [get_FitContent](./get_fitcontent/) | يحصل على قيمة تشير إلى ما إذا كان يجب زيادة ارتفاع الصف ليتناسب مع محتواه. |
| [get_FitTimescaleToEndOfPage](./get_fittimescaletoendofpage/) | يحصل على ما إذا كان يجب عرض قسم التقويم في العرض حتى النهاية (الجانب الأيمن) من الصفحة الأخيرة. إذا كانت القيمة false، يتم عرض قسم التقويم بالضبط حتى EndDate، حتى وإن كان هناك مساحة فارغة في الصفحة. |
| [get_Gridlines](./get_gridlines/) | يحصل على قائمة خطوط الشبكة التي تظهر في عرض المشروع. |
| [get_IsPortrait](./get_isportrait/) | يحصل على قيمة تشير إلى ما إذا كان اتجاه الصفحة عموديًا؛ يرجع false إذا كان اتجاه الصفحة أفقيًا. |
| [get_LegendDrawingOptions](./get_legenddrawingoptions/) | يحصل على قيمة تحدد كيفية عرض وسيلة الإيضاح. القيمة الافتراضية هي LegendDrawingOptions.OnEveryPage. |
| [get_LegendItems](./get_legenditems/) | يحصل على مصفوفة من PageLegendItem التي تحدد أي الأشرطة يجب عرضها في وسيلة إيضاح الصفحة. إذا كانت null، يتم عرض العناصر الافتراضية. |
| [get_MarkCriticalTasks](./get_markcriticaltasks/) | يحصل على قيمة تشير إلى ما إذا كان يجب عرض المهام الحرجة باللون الأحمر (القيمة الافتراضية هي FALSE). |
| [get_NonWorkingTimeColor](./get_nonworkingtimecolor/) | يحصل على لون وقت غير العمل. |
| [get_PageCount](./get_pagecount/) | يحصل على عدد صفحات المشروع. |
| [get_PageSize](./get_pagesize/) | يحصل على حجم الصفحة التي سيتم عرضها (القيمة الافتراضية هي PageSize.A4). |
| [get_PresentationFormat](./get_presentationformat/) | يحصل على PresentationFormat الذي سيتم حفظ المستند به. |
| [get_RenderToSinglePage](./get_rendertosinglepage/) | يحصل على قيمة تشير إلى ما إذا كان يجب عرض المشروع في صفحة واحدة عندما يتم حفظ المشروع بصيغة رسومية. سيتم تغيير حجم الصفحة بحيث يتناسب المشروع المعروض على صفحة واحدة. |
| [get_RollUpGanttBars](./get_rollupganttbars/) | يحصل على قيمة تشير إلى ما إذا كان يجب وضع علامة على المهام الفرعية على شريط المهمة الملخصة. بالنسبة للمهام الفرعية، يشير حقل Rollup إلى ما إذا كانت معلومات أشرطة جانت للمهام الفرعية ستُدمج في شريط المهمة الملخصة. بالنسبة للمهام الملخصة، يشير حقل Rollup إلى ما إذا كان شريط المهمة الملخصة يعرض الأشرطة المدمجة. يجب أن يكون حقل Rollup للمهام الملخصة مضبوطًا على Yes لكي يتم دمج أي مهام فرعية فيها. |
| [get_StartDate](./get_startdate/) | يحصل على التاريخ لبدء العرض منه. |
| [get_TextStyles](./get_textstyles/) | يحصل على قائمة أنماط النص التي تُطبق أثناء عرض عرض المشروع. |
| [get_Timescale](./get_timescale/) | يحصل على قيمة Timescale التي تُستخدم للتحكم في كيفية عرض المقياس الزمني (إن وجد) عندما يتم حفظ المشروع بصيغة رسومية. |
| [get_TimescaleFitBehavior](./get_timescalefitbehavior/) | يحصل على سلوك يحدد كيفية محاذاة الطرف الأيمن للمقياس الزمني مع نهاية الصفحة. |
| [get_UseGradientBrush](./get_usegradientbrush/) | يحصل على قيمة تشير إلى ما إذا كان يجب استخدام فرشاة التدرج عند عرض مخطط جانت. |
| [get_View](./get_view/) | يحصل على قائمة أعمدة العرض التي سيتم عرضها (GanttChartColumn). إذا لم يتم تحديدها، يتم عرض معرفات المهام، أسماء المهام، البداية والنهاية فقط. إذا تم تعيين كل من خصائص View و ViewSettings، فإن الأعمدة من View تتجاوز الأعمدة من ViewSettings. |
| [get_ViewSettings](./get_viewsettings/) | يحصل على عرض (View) لعرضه. يمكنك استخدام هذه الخيارات لتحديد بشكل صريح أي عرض يجب حفظه بصيغ PDF أو HTML أو Image. إذا تم تعيين هذه الخاصية، يتم تجاهل خاصية Visualization::PresentationFormat عند حفظ المشروع. يجب أن يكون العرض من إحدى الشاشات التالية ((Aspose::Tasks::View::Screen)): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage). |
| [set_BarStyles](./set_barstyles/) | يضبط قائمة مثيلات فئة BarStyle التي تظهر في عرض المشروع. |
| [set_CustomPageSize](./set_custompagesize/) | يضبط حجم الصفحة المخصص بالنقاط (نقطة واحدة = 1/72 من البوصة). |
| [set_DrawNonWorkingTime](./set_drawnonworkingtime/) | يضبط قيمة تشير إلى ما إذا كان يجب رسم وقت غير العمل (القيمة الافتراضية هي TRUE). |
| [set_EndDate](./set_enddate/) | يضبط تاريخًا لإنهاء عملية العرض. |
| [set_FitContent](./set_fitcontent/) | يضبط قيمة تشير إلى ما إذا كان يجب زيادة ارتفاع الصف ليتناسب مع محتواه. |
| [set_FitTimescaleToEndOfPage](./set_fittimescaletoendofpage/) | يضبط ما إذا كان قسم التقويم في العرض يجب أن يُعرض حتى النهاية (الجانب الأيمن) للصفحة الأخيرة. إذا كانت القيمة false، يُعرض قسم التقويم بالضبط حتى EndDate، حتى وإن كان هناك مساحة فارغة في الصفحة. |
| [set_Gridlines](./set_gridlines/) | يضبط قائمة خطوط الشبكة التي تظهر في عرض المشروع. |
| [set_IsPortrait](./set_isportrait/) | يضبط قيمة تشير إلى ما إذا كان اتجاه الصفحة عموديًا؛ يرجع false إذا كان اتجاه الصفحة أفقيًا. |
| [set_LegendDrawingOptions](./set_legenddrawingoptions/) | يضبط قيمة تحدد طريقة عرض المفتاح. القيمة الافتراضية هي LegendDrawingOptions.OnEveryPage. |
| [set_LegendItems](./set_legenditems/) | يضبط مصفوفة من PageLegendItem التي تحدد أي الأشرطة يجب عرضها في مفتاح الصفحة. إذا كانت null، تُعرض العناصر الافتراضية. |
| [set_MarkCriticalTasks](./set_markcriticaltasks/) | يضبط قيمة تشير إلى ما إذا كان يجب عرض المهام الحرجة باللون الأحمر (القيمة الافتراضية هي FALSE). |
| [set_NonWorkingTimeColor](./set_nonworkingtimecolor/) | يضبط لون وقت غير العمل. |
| [set_PageSize](./set_pagesize/) | يضبط حجم الصفحة التي سيتم عرضها (القيمة الافتراضية هي PageSize.A4). |
| [set_PresentationFormat](./set_presentationformat/) | يضبط PresentationFormat الذي سيتم حفظ المستند به. |
| [set_RenderToSinglePage](./set_rendertosinglepage/) | يضبط قيمة تشير إلى ما إذا كان يجب عرض المشروع في صفحة واحدة عندما يتم حفظ المشروع بصيغة رسومية. سيتم تغيير حجم الصفحة بحيث يتناسب المشروع المعروض على صفحة واحدة. |
| [set_RollUpGanttBars](./set_rollupganttbars/) | يضبط قيمة تشير إلى ما إذا كان يجب تمييز المهام الفرعية على شريط المهمة الملخصة. بالنسبة للمهام الفرعية، حقل Rollup يحدد ما إذا كانت معلومات أشرطة جانت للمهام الفرعية ستُدمج في شريط المهمة الملخصة. بالنسبة للمهام الملخصة، حقل Rollup يحدد ما إذا كان شريط المهمة الملخصة يعرض أشرطة مدمجة. يجب أن تكون قيمة حقل Rollup للمهام الملخصة مضبوطة على Yes لكي يتم دمج أي مهام فرعية فيها. |
| [set_StartDate](./set_startdate/) | يضبط التاريخ الذي يبدأ منه العرض. |
| [set_TextStyles](./set_textstyles/) | يضبط قائمة أنماط النص التي تُطبق أثناء عرض عرض المشروع. |
| [set_Timescale](./set_timescale/) | يضبط قيمة Timescale التي تُستخدم للتحكم في طريقة عرض المقياس الزمني (إن وجد) عندما يتم حفظ المشروع بصيغة رسومية. |
| [set_TimescaleFitBehavior](./set_timescalefitbehavior/) | يضبط سلوكًا يحدد كيفية محاذاة الطرف الأيمن للمقياس الزمني مع نهاية الصفحة. |
| [set_UseGradientBrush](./set_usegradientbrush/) | يضبط قيمة تشير إلى ما إذا كان يجب استخدام فرشاة تدرجية عند عرض مخطط جانت. |
| [set_View](./set_view/) | يضبط قائمة أعمدة العرض التي سيتم عرضها (GanttChartColumn). إذا لم يتم ضبطها، تُعرض فقط معرفات المهام، أسماء المهام، تاريخ البدء والانتهاء. إذا تم ضبط كل من خصائص View و ViewSettings، فإن الأعمدة من View تتجاوز الأعمدة من ViewSettings. |
| [set_ViewSettings](./set_viewsettings/) | يضبط عرضًا (View) للعرض. يمكنك استخدام هذا الخيار لتحديد بشكل صريح أي عرض يجب حفظه بصيغ PDF أو HTML أو Image. إذا تم ضبط هذه الخاصية، يتم تجاهل خاصية Visualization::PresentationFormat عند حفظ المشروع. يجب أن يكون العرض من إحدى الشاشات التالية ((Aspose::Tasks::View::Screen)): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage). |

