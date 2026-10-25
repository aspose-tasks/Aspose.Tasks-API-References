---
title: "Calendar"
second_title: "Aspose.Tasks لـ Python عبر .NET مرجع API"
description: 
type: docs
weight: 140
url: /ar/python-net/aspose.tasks/calendar/
---

## Calendar class

يمثل تقويمًا يُستخدم في مشروع.

يعرض نوع Calendar الأعضاء التالية:
## الخصائص
| الاسم | الوصف |
| :- | :- |
| name | يحصل أو يضبط اسم التقويم. |
| uid | يحصل أو يعيّن المعرف الفريد للتقويم. |
| week_days | يحصل على WeekDaysCollection لهذا التقويم.<br/>            مجموعة أيام الأسبوع التي تحدد التقويم. |
| exceptions | يحصل على كائن CalendarExceptionCollection.<br/>            مجموعة الاستثناءات المرتبطة بالتقويم. |
| work_weeks | يحصل على كائن WorkWeekCollections.<br/>            مجموعة أسابيع العمل المرتبطة بالتقويم. |
| is_base_calendar | يحصل على قيمة تشير إلى ما إذا كان التقويم تقويمًا أساسيًا. |
| base_calendar | يحصل أو يعيّن التقويم الأساسي الذي يعتمد عليه هذا التقويم.<br/>            ينطبق فقط إذا لم يكن التقويم تقويمًا أساسيًا. |
| is_baseline_calendar | يحصل أو يعيّن قيمة تشير إلى ما إذا كان التقويم تقويمًا لخط الأساس. |
| guid | يحصل على معرف GUID للتقويم. |
| primavera_properties | يحصل على كائن يحتوي على خصائص خاصة بـ Primavera لتقويم تم قراءته من صيغ Primavera. |
## الطرق
| الاسم | الوصف |
| :- | :- |
| get_start_date_from_finish_and_duration(finish, duration) | يعيد تاريخ البدء بناءً على تاريخ الانتهاء المحدد والمدة. |
| get_start_date_from_finish_and_duration(finish, duration) | يعيد تاريخ البدء بناءً على تاريخ الانتهاء والمدة المحددين. |
| get_working_hours(start, finish) | إرجاع WorkUnit - بدء، انتهاء ومدة ساعات العمل للفترة الزمنية المحددة. |
| get_working_hours(dt) | إرجاع WorkUnit - بدء، انتهاء ومدة ساعات العمل للفترة الزمنية المحددة. |
| get_finish_date_by_start_and_work(start, work) | يحسب التاريخ الذي ستنقضي فيه كمية الوقت العمل المحددة وفقًا للتقويم. |
| get_finish_date_by_start_and_work(start, work) | يحسب التاريخ الذي ستنقضي فيه كمية الوقت العمل المحددة وفقًا للتقويم. |
| get_intersection_calendar(calendar1, calendar2) | يحصل على مثيل [ICalendar](/tasks/python-net/aspose.tasks/icalendar/) يمكن استخدامه لإجراء حسابات على تقاطع جداول عمل تقويمين. |
| make_standard_calendar(calendar) | ينشئ تقويمًا قياسيًا افتراضيًا. |
| make_24_hour_calendar(calendar) | يجعل التقويم المحدد تقويمًا 24 ساعة.<br/>            تقويم 24 ساعة هو تقويم يعمل فيه كل يوم من الأسبوع بساعات عمل مستمرة على مدار الساعة. |
| make_night_shift_calendar(calendar) | يجعل التقويم المحدد تقويمًا لورديات الليل. |
| delete() | يزيل التقويم من المشروع. |
| is_day_working(dt) | يحدد ما إذا كان اليوم المحدد يوم عمل وفقًا للتقويم. |
| get_working_hours_time_span(start, finish) | يعيد مقدار ساعات العمل بين التواريخ المحددة. |
| get_task_finish_date_from_duration(task, duration) | يحسب تاريخ وانتهاء المهمة والوقت من تاريخ بدايتها، الأجزاء المقسمة ومدة العمل. |
| get_working_times(dt) | يعيد [WorkingTimeCollection](/tasks/python-net/aspose.tasks/workingtimecollection/) لأوقات العمل للتاريخ المحدد. |
| get_previous_working_day_end(date) | يحسب نهاية تاريخ العمل السابق من التاريخ المحدد. |
| get_next_working_day_start(date) | يحسب بداية يوم العمل التالي للتاريخ المحدد. |
| get_work_start(date) | يحسب بداية وقت العمل التالي بدءًا من التاريخ والوقت المحددين. |
| is_empty() | يعيد ما إذا كان التقويم لا يحتوي على ساعات عمل معرفة. |

### انظر أيضًا

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

