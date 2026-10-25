---
title: "CalendarException"
second_title: "Aspose.Tasks لـ Python عبر .NET مرجع API"
description: 
type: docs
weight: 160
url: /ar/python-net/aspose.tasks/calendarexception/
---

## CalendarException class

يمثل فترات زمنية استثنائية في تقويم.

يعرض نوع CalendarException الأعضاء التالية:
## المُنشئات
| الاسم | الوصف |
| :- | :- |
| CalendarException() | ينشئ مثلاً جديداً من الفئة [CalendarException](/tasks/python-net/aspose.tasks/calendarexception/). |
## الخصائص
| الاسم | الوصف |
| :- | :- |
| entered_by_occurrences | يحصل أو يعيّن قيمة تشير إلى ما إذا كان نطاق التكرار معرفًا بإدخال عدد من التكرارات.<br/>            False يحدد أن نطاق التكرار معرف بإدخال تاريخ الانتهاء. |
| from_date | يحصل أو يعيّن بداية وقت الاستثناء. |
| to_date | يحصل أو يعيّن نهاية وقت الاستثناء. |
| occurrences | يحصل أو يعيّن عدد التكرارات التي يكون فيها استثناء التقويم صالحًا. |
| name | يحصل أو يعيّن اسم الاستثناء. |
| نوع | يحصل أو يعيّن نوع الاستثناء. |
| period | يحصل أو يعيّن فترة التكرار للاستثناء. |
| days_of_week | يحصل على DayTypeCollection لهذا الكائن.<br/>            أيام الأسبوع التي يكون فيها الاستثناء صالحًا. |
| month_item | يحصل أو يعيّن عنصر الشهر الذي يُجدول له تكرار الاستثناء. |
| month_position | يحصل أو يعيّن موضع عنصر الشهر داخل الشهر. |
| month | يحصل أو يعيّن الشهر الذي يُجدول له تكرار الاستثناء. |
| month_day | يحصل أو يعيّن يوم الشهر الذي يُجدول له تكرار الاستثناء. |
| day_working | يحصل أو يضبط قيمة تشير إلى ما إذا كان التاريخ المحدد أو نوع اليوم يعمل. |
| working_times | يحصل أو يعيّن كائن WorkingTimeCollection.<br/>            مجموعة أوقات العمل التي تحدد الوقت العامل في أيام الأسبوع. |
| parent_calendar | يحصل على التقويم الأب لهذا الكائن. |
## الطرق
| الاسم | الوصف |
| :- | :- |
| delete() | يحذف مثيل Exception من كائن CalendarExceptionCollection الخاص بالتقويم الأب. |
| check_exception(dt) | يرجع true إذا كان المثيل المحدد من بنية datetime هو يوم الاستثناء. |
| get_working_time() | يعيد وقت العمل لاستثناء التقويم. |
| get_exception_dates() | يعيد التواريخ التي ينطبق عليها استثناء التقويم. |

### انظر أيضًا

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

