---
title: "ProjectDisplayOptions.ShowTaskScheduleWarnings"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ProjectDisplayOptions. يحصل أو يضبط قيمة تشير إلى ما إذا كان يجب إظهار التحذيرات عندما يحدد Project تعارضًا محتملًا في الجدولة مع مهمة مجدولة يدويًا. هذا الخيار متاح لإصدار Project 2010 وما بعده"
type: docs
weight: 90
url: /ar/net/aspose.tasks/projectdisplayoptions/showtaskschedulewarnings/
---
## ProjectDisplayOptions.ShowTaskScheduleWarnings property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب عرض التحذيرات عندما يحدد Project تعارضًا محتملًا في الجدولة مع مهمة مجدولة يدويًا. هذا الخيار متاح لإصدار Project 2010 وما بعده.

```csharp
public bool ShowTaskScheduleWarnings { get; set; }
```

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

* class [ProjectDisplayOptions](../)
* namespace [Aspose.Tasks](../../projectdisplayoptions/)
* assembly [Aspose.Tasks](../../../)


