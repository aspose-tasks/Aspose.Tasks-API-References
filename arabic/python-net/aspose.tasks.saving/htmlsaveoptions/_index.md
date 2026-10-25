---
title: "HtmlSaveOptions"
second_title: "Aspose.Tasks لـ Python عبر .NET مرجع API"
description: 
type: docs
weight: 20
url: /ar/python-net/aspose.tasks.saving/htmlsaveoptions/
---

## HtmlSaveOptions class

يسمح بتحديد خيارات إضافية عند عرض صفحات المشروع إلى HTML.

يعرض نوع HtmlSaveOptions الأعضاء التالية:
## المُنشئات
| الاسم | الوصف |
| :- | :- |
| HtmlSaveOptions() | يُنشئ مثلاً جديداً من الفئة [HtmlSaveOptions](/tasks/python-net/aspose.tasks.saving/htmlsaveoptions/) . |
## الخصائص
| الاسم | الوصف |
| :- | :- |
| save_format |  |
| bar_styles | يحصل أو يعيّن قائمة مثيلات الفئة [BarStyle](/tasks/python-net/aspose.tasks.visualization/barstyle/) التي تظهر في عرض المشروع. |
| draw_non_working_time | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب رسم الوقت غير العامل (القيمة الافتراضية هي TRUE). |
| end_date | يحصل أو يعيّن تاريخ الانتهاء من العرض. |
| timescale_fit_behavior | يحصل أو يعيّن سلوكًا يحدد كيفية محاذاة الطرف الأيمن للمقياس الزمني مع نهاية الصفحة. |
| fit_content | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب زيادة ارتفاع الصف ليتناسب مع محتواه. |
| gridlines | يحصل أو يضبط قائمة من [Gridline](/tasks/python-net/aspose.tasks.visualization/gridline/) التي تظهر في عرض المشروع. |
| legend_drawing_options | يحصل أو يضبط قيمة تحدد كيفية عرض وسيلة الإيضاح. القيمة الافتراضية هي LegendDrawingOptions.OnEveryPage. |
| legend_items | يحصل أو يضبط مصفوفة من PageLegendItem التي تحدد أي الأشرطة يجب عرضها في وسيلة إيضاح الصفحة.<br/>            إذا كانت null، يتم عرض العناصر الافتراضية. |
| mark_critical_tasks | يحصل أو يضبط قيمة تشير إلى ما إذا كان يجب عرض المهام الحرجة باللون الأحمر (القيمة الافتراضية هي FALSE). |
| non_working_time_color | يحصل أو يضبط لون وقت عدم العمل. |
| page_count | يحصل أو يضبط عدد صفحات المشروع. |
| page_size | يحصل أو يضبط حجم الصفحة التي سيتم عرضها (القيمة الافتراضية هي PageSize.A4). |
| is_portrait | يحصل أو يضبط قيمة تشير إلى ما إذا كان اتجاه الصفحة عموديًا؛ يرجع false إذا كان اتجاه الصفحة أفقيًا. |
| presentation_format | يحصل أو يضبط [presentation_format](/tasks/python-net/aspose.tasks.saving/saveoptions/) الذي سيُحفظ به المستند. |
| roll_up_gantt_bars | يحصل أو يضبط قيمة تشير إلى ما إذا كان يجب تمييز المهام الفرعية على شريط المهمة الملخصة.<br/>            بالنسبة للمهام الفرعية، حقل Rollup يشير إلى ما إذا كانت معلومات أشرطة جانت للمهام الفرعية ستُدمج في شريط المهمة الملخصة.<br/>            بالنسبة للمهام الملخصة، حقل Rollup يشير إلى ما إذا كان شريط المهمة الملخصة يعرض أشرطة مدمجة.<br/>            يجب أن تكون قيمة حقل Rollup للمهام الملخصة مضبوطة على Yes لكي يتم دمج أي مهام فرعية فيها. |
| start_date | يحصل أو يضبط التاريخ الذي يبدأ منه العرض. |
| text_styles | يحصل أو يضبط قائمة أنماط النص التي تُطبق أثناء عرض عرض المشروع. |
| timescale | يحصل أو يضبط قيمة [timescale](/tasks/python-net/aspose.tasks.saving/saveoptions/) التي تُستخدم للتحكم في كيفية عرض المقياس الزمني (إن وجد) عند حفظ المشروع بصيغة رسومية. |
| use_gradient_brush | يحصل أو يضبط قيمة تشير إلى ما إذا كان يجب استخدام فرشاة تدرجية عند عرض تخطيط المشروع. |
| view | يحصل أو يضبط قائمة أعمدة العرض التي سيتم عرضها ([GanttChartColumn](/tasks/python-net/aspose.tasks.visualization/ganttchartcolumn/)).<br/>            إذا لم يتم ضبطها، فسيتم عرض معرفات المهام، أسماء المهام، البداية والنهاية فقط.<br/>            إذا تم ضبط كل من خاصيتي View و[view_settings](/tasks/python-net/aspose.tasks.saving/saveoptions/)، فإن الأعمدة من View تتجاوز الأعمدة من ViewSettings. |
| view_settings | يحصل أو يضبط عرضًا ([view](/tasks/python-net/aspose.tasks.saving/saveoptions/)) للعرض. يمكنك استخدام هذا الخيار لتحديد بشكل صريح أي عرض يجب حفظه بصيغ PDF أو HTML أو Image.<br/>            إذا تم ضبط هذه الخاصية، يتم تجاهل خاصية [PresentationFormat](/tasks/python-net/aspose.tasks.visualization/presentationformat/) عند حفظ المشروع.<br/>            يجب أن يكون العرض من إحدى الشاشات التالية (([screen](/tasks/python-net/aspose.tasks/view/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |
| custom_page_size | يحصل أو يعيّن حجم الصفحة المخصص بالنقاط (1 نقطة = 1/72 بوصة). |
| render_to_single_page | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب عرض المشروع في صفحة واحدة<br/>            عندما يتم حفظ المشروع بصيغة رسومية.<br/>            سيتم تغيير حجم الصفحة بحيث يمكن أن يتناسب المشروع المعروض على صفحة واحدة. |
| css_style_prefix | يحصل أو يعيّن بادئة نمط CSS. |
| font_settings | يحدد إعدادات الخط المستخدمة عند عرض رؤية المشروع. |
| reduce_footer_gap | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب تقليل الفجوة بين المهمة الأخيرة وتذييل الصفحة. |
| include_project_name_in_page_header | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب تضمين اسم المشروع في رأس صفحة HTML. |
| include_project_name_in_title | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب تضمين اسم المشروع في عنوان HTML. |
| pages | يحصل أو يعيّن قائمة بأرقام الصفحات التي يجب حفظها عند عرض تخطيط المشروع. |
| export_css | يحصل أو يعيّن طريقة تصدير CSS. |
| export_images | يحصل أو يعيّن طريقة تصدير الصور. |
| export_fonts | يحصل أو يعيّن طريقة تصدير الخطوط. |
| css_saving_callback | يحصل أو يعيّن رد الاتصال الذي يُستدعى لإنشاء مورد لتخزين CSS. |
| font_saving_callback | يحصل أو يعيّن رد الاتصال الذي يُستدعى لإنشاء مورد لتخزين الخط. |
| image_saving_callback | يحصل أو يعيّن رد الاتصال الذي يُستدعى لإنشاء مورد لتخزين الخط. |
| font_face_types | يحصل أو يعيّن أنواع خطوط الوجه. |
| page_saving_callback | يحصل أو يعيّن رد نداء معرف من قبل المستخدم يُستخدم للحصول على تدفق إخراج لكل صفحة مُصوَّرة. |

### انظر أيضًا

* namespace [aspose.tasks.saving](/tasks/python-net/aspose.tasks.saving/)
* assembly [Aspose.Tasks](/tasks/python-net/)

