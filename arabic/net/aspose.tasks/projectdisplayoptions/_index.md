---
title: "الفئة ProjectDisplayOptions"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.ProjectDisplayOptions. تمثل خيارات العرض لمثيل مشروع."
type: docs
weight: 1450
url: /ar/net/aspose.tasks/projectdisplayoptions/
---
## ProjectDisplayOptions class

يمثل خيارات العرض لنسخة مشروع.

```csharp
public class ProjectDisplayOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [ProjectDisplayOptions](projectdisplayoptions/)() | يُنشئ مثيلًا جديدًا للفئة `ProjectDisplayOptions`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AddSpaceBeforeLabel](../../aspose.tasks/projectdisplayoptions/addspacebeforelabel/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب إضافة مسافة قبل القيمة الرقمية واختصار الوقت (1 wk مقابل 1wk). |
| [DayLabel](../../aspose.tasks/projectdisplayoptions/daylabel/) { get; set; } | يحصل أو يعيّن طريقة عرض تسمية اليوم. |
| [HourLabel](../../aspose.tasks/projectdisplayoptions/hourlabel/) { get; set; } | يحصل أو يعيّن طريقة عرض تسمية الساعة. |
| [MinuteLabel](../../aspose.tasks/projectdisplayoptions/minutelabel/) { get; set; } | يحصل أو يعيّن طريقة عرض تسمية الدقيقة. |
| [MonthLabel](../../aspose.tasks/projectdisplayoptions/monthlabel/) { get; set; } | يحصل أو يعيّن طريقة عرض تسمية الشهر. |
| [ShowProjectSummaryTask](../../aspose.tasks/projectdisplayoptions/showprojectsummarytask/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب عرض معلومات ملخص حول مشروع كامل في صف واحد مع شريط مهمة الملخص الخاص به في أعلى عرض مخطط جانت. |
| [ShowTaskScheduleSuggestions](../../aspose.tasks/projectdisplayoptions/showtaskschedulesuggestions/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب إظهار الاقتراحات عندما يحدد Project تعارضًا محتملًا في الجدولة مع مهمة مجدولة يدويًا. هذا الخيار متاح لإصدار Project 2010 وما بعده. |
| [ShowTaskScheduleWarnings](../../aspose.tasks/projectdisplayoptions/showtaskschedulewarnings/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب عرض التحذيرات عندما يحدد Project تعارضًا محتملًا في الجدولة مع مهمة مجدولة يدويًا. هذا الخيار متاح لإصدار Project 2010 وما بعده. |
| [UnderlineHyperlinks](../../aspose.tasks/projectdisplayoptions/underlinehyperlinks/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب تسطير الروابط التشعبية. |
| [WeekLabel](../../aspose.tasks/projectdisplayoptions/weeklabel/) { get; set; } | يحصل أو يعيّن طريقة عرض تسمية الأسبوع. |
| [YearLabel](../../aspose.tasks/projectdisplayoptions/yearlabel/) { get; set; } | يحصل أو يعيّن طريقة عرض تسمية السنة. |

## الأمثلة

يعرض كيفية استخدام خيارات عرض المشروع.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// عيّن قيمة تشير إلى ما إذا كان يجب عرض التحذيرات عندما يحدد Project تعارضًا محتملًا في الجدولة مع مهمة مجدولة يدويًا.
// هذا الخيار متاح لإصدار Project 2010 وما بعده.
project.DisplayOptions.ShowTaskScheduleWarnings = false;

// قيمة تشير إلى ما إذا كان يجب إضافة مسافة قبل القيمة العددية واختصار الوقت (1 wk مقابل 1wk)
project.DisplayOptions.AddSpaceBeforeLabel = true;

// تعيين كيفية عرض تسمية الدقيقة
project.DisplayOptions.MinuteLabel = MinuteLabelDisplay.Min;

// تحديد كيفية عرض تسمية الساعة
project.DisplayOptions.HourLabel = HourLabelDisplay.Hr;

// عيّن طريقة عرض تسمية اليوم
project.DisplayOptions.DayLabel = DayLabelDisplay.Dy;

// عيّن طريقة عرض تسمية الأسبوع
project.DisplayOptions.WeekLabel = WeekLabelDisplay.Week;

// ضبط كيفية عرض تسمية الشهر
project.DisplayOptions.MonthLabel = MonthLabelDisplay.Mon;

// ضبط كيفية عرض تسمية السنة
project.DisplayOptions.YearLabel = YearLabelDisplay.Year;

// عيّن قيمة تشير إلى ما إذا كان يجب عرض معلومات ملخص حول مشروع كامل في صف واحد مع شريط مهمة ملخص خاص به في أعلى عرض مخطط جانت.
project.DisplayOptions.ShowProjectSummaryTask = true;

// عيّن قيمة تشير إلى ما إذا كان يجب عرض الاقتراحات عندما يحدد Project تعارضًا محتملًا في الجدولة مع مهمة مجدولة يدويًا.
project.DisplayOptions.ShowTaskScheduleSuggestions = true;

// عيّن قيمة تشير إلى ما إذا كان يجب تسطير الروابط التشعبية.
project.DisplayOptions.UnderlineHyperlinks = true;

project.Save(OutDir + "WorkWithProjectDisplayOptions.mpp", SaveFileFormat.Mpp);
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


