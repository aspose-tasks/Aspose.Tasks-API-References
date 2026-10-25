---
title: "GanttChartView"
second_title: "Aspose.Tasks لـ Python عبر .NET مرجع API"
description: 
type: docs
weight: 390
url: /ar/python-net/aspose.tasks/ganttchartview/
---

## GanttChartView class

يمثل عرض مخطط جانت.

يعرض نوع GanttChartView الأعضاء التالية:
## المُنشئات
| الاسم | الوصف |
| :- | :- |
| GanttChartView() | ينشئ مثلاً جديداً من الفئة [GanttChartView](/tasks/python-net/aspose.tasks/ganttchartview/) . |
## الخصائص
| الاسم | الوصف |
| :- | :- |
| filter | يحصل أو يعيّن مرشحًا يُستخدم في عرض واحد. |
| مجموعة | يحصل أو يعيّن مجموعة من العرض الفردي. |
| uid | يحصل على المعرف الفريد لعرض. |
| highlight_filter | يحصل أو يعيّن قيمة تشير إلى ما إذا كان Microsoft Project يسلط الضوء على المرشح للعرض الفردي. |
| name | يحصل أو يعيّن اسم كائن View. |
| screen | يحصل على نوع الشاشة للعرض الفردي.<br/>            Read-only [ViewScreen](/tasks/python-net/aspose.tasks/viewscreen/). |
| parent_project | يحصل على الأصل لكائن View.<br/>            Read-only [Project](/tasks/python-net/aspose.tasks/project/). |
| جدول | يحصل أو يعيّن جدول للعرض الفردي. |
| type | يحصل على نوع العنصر في العرض الفردي، مثل المهام أو الموارد.<br/>            Read-only [ItemType](/tasks/python-net/aspose.tasks/itemtype/). |
| show_in_menu | يحصل أو يعيّن قيمة تشير إلى ما إذا كان Microsoft Project يعرض اسم العرض الفردي في قائمة العرض أو القوائم المنسدلة للعرض الآخر في الشريط. |
| page_info | يحصل على نسخة من الفئة [page_info](/tasks/python-net/aspose.tasks/view/). تمثل بيانات إعداد الصفحة الموجودة في تنسيق ملف mpp. |
| visual_objects_placements | يحصل على مجموعة من الكائنات التي تمثل وضع ومظهر [OleObject](/tasks/python-net/aspose.tasks/oleobject/) في العرض. |
| bar_size | يحصل أو يضبط الارتفاع، بالنقاط، لأشرطة Gantt في مخطط Gantt. |
| gridlines | يحصل أو يضبط قائمة [gridlines](/tasks/python-net/aspose.tasks/ganttchartview/) لعرض مخطط Gantt. |
| text_styles | يحصل أو يضبط قائمة [TextStyle](/tasks/python-net/aspose.tasks.visualization/textstyle/) لعرض مخطط Gantt. |
| show_drawings | يحصل أو يضبط قيمة تشير إلى ما إذا كان يجب إظهار الرسومات على مخطط Gantt. |
| show_bar_splits | يحصل أو يضبط قيمة تشير إلى ما إذا كان يجب إظهار تقسيمات المهام على مخطط Gantt. |
| roll_up_gantt_bars | يحصل أو يضبط قيمة تشير إلى ما إذا كان يجب دمج الأشرطة على مخطط Gantt. |
| bar_rounding | يحصل أو يضبط قيمة تشير إلى ما إذا كانت الأشرطة تُقرب إلى أقرب يوم.<br/>            القيمة الافتراضية هي True. |
| bottom_timescale_tier | يحصل أو يعيّن إعدادات مستوى مقياس الزمن السفلي للعرض.<br/>            [TimescaleTier](/tasks/python-net/aspose.tasks.visualization/timescaletier/) |
| middle_timescale_tier | يحصل أو يعيّن إعدادات مستوى مقياس الزمن الأوسط للعرض.<br/>            [TimescaleTier](/tasks/python-net/aspose.tasks.visualization/timescaletier/). |
| top_timescale_tier | يحصل أو يضبط إعدادات الطبقة العليا لمقياس الوقت في العرض.<br/>            [TimescaleTier](/tasks/python-net/aspose.tasks.visualization/timescaletier/). |
| timescale_size_percentage |  |
| hide_rollup_bars_when_summary_expanded | يحصل أو يضبط قيمة تشير إلى ما إذا كانت أشرطة التجميع ستُخفى عند توسيع مهمة الملخص. |
| progress_lines | يحصل أو يضبط خطوط التقدم لعرض مخطط Gantt.<br/>            [progress_lines](/tasks/python-net/aspose.tasks/ganttchartview/). |
| auto_filters | يحصل على قائمة من عوامل التصفية التلقائية لعرض مخطط جانت. |
| table_text_styles | يحصل على قائمة بأنماط نص الجدول لعرض مخطط جانت.<br/>            [TableTextStyle](/tasks/python-net/aspose.tasks.visualization/tabletextstyle/). |
| bar_styles | يحصل على قائمة بأنماط الأشرطة الأصلية (الشائعة) لعرض مخطط جانت.<br/>            [GanttBarStyle](/tasks/python-net/aspose.tasks.visualization/ganttbarstyle/). |
| custom_bar_styles | يحصل على قائمة بأنماط الأشرطة المخصصة لكل مهمة لعرض مخطط جانت.<br/>            [GanttBarStyle](/tasks/python-net/aspose.tasks.visualization/ganttbarstyle/). |
| non_working_time_color | يحصل أو يضبط لون وقت غير العمل. |
## الطرق
| الاسم | الوصف |
| :- | :- |
| compare_to(other) | يقارن النسخة الحالية مع كائن آخر من نفس النوع ويعيد عددًا صحيحًا يشير إلى ما إذا كانت النسخة الحالية تسبق أو تتبع أو تقع في نفس الموضع في ترتيب الفرز مقارنةً بالكائن الآخر. |

### انظر أيضًا

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

