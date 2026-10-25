---
title: "تعداد DateLabel"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.Visualization.DateLabel. يحدد تنسيق العرض لتسميات التاريخ والوقت في مقياس الزمن."
type: docs
weight: 2980
url: /ar/net/aspose.tasks.visualization/datelabel/
---
## DateLabel enumeration

يحدد تنسيق العرض لتسميات التاريخ والوقت في مقياس الزمن.

```csharp
public enum DateLabel
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `35` | لا يتم عرض أي تاريخ. |
| DayDdd | `19` | الأمثلة هي Mon، Tue. |
| DayDddDd | `105` | الأمثلة هي Mon 30، Tue 1 |
| DayDddMDd | `112` | الأمثلة هي Mon S 30، Tue O 1 |
| DayDddMmDd | `108` | الأمثلة هي Mon 9/30، Tue 10/1 |
| DayDddMmDdYy | `52` | الأمثلة هي Mon 9/30/02، Tue 10/1/02 |
| DayDddMmmDd | `23` | الأمثلة هي Mon Sep 30، Tue Oct 1 |
| DayDddMmmDdYyy | `22` | الأمثلة هي Mon Sep 30 '02، Tue Oct 1 '02 |
| DayDddMmmmDd | `111` | الأمثلة هي Mon September 30، Tue October 1 |
| DayDddd | `18` | الأمثلة هي Tuesday، Wednesday. |
| DayDdi | `119` | الأمثلة هي Mo، Tu |
| DayDdiDd | `106` | الأمثلة هي Mo 30، Tu 1 |
| DayDdiMDd | `113` | الأمثلة هي Mo S 30، Tu O 1 |
| DayDdiMmDd | `109` | الأمثلة هي Mo 9/30، Tu 10/1 |
| DayDi | `20` | الأمثلة هي M، T |
| DayDiDdSpace | `107` | الأمثلة هي M 30، T 1 |
| DayDiMDd | `114` | الأمثلة هي M S 30، T O 1 |
| DayDiMmDd | `110` | الأمثلة هي M 9/30، T 10/1 |
| DayDiDdNoSpace | `121` | الأمثلة هي M30، T1 |
| DayMDd | `115` | الأمثلة هي S 30، O 1 |
| DayMmDd | `27` | الأمثلة هي 9/30، 10/1 |
| DayMmDdYy | `26` | الأمثلة هي 9/30/02، 10/1/02 |
| DayMmmDd | `25` | الأمثلة هي Sep 30, Oct 1 |
| DayMmmDdYyy | `24` | الأمثلة هي Sep 30 '02, Oct 10 '02 |
| DayFromEndDayDd | `41` | الأمثلة هي Day 2, Day 1, Day -1, Day -2 من نهاية المشروع. |
| DayFromEndDd | `54` | الأمثلة هي 2, 1, -1, -2 |
| DayFromEndDdd | `53` | الأمثلة هي D2, D1, D-1, D-2 |
| DayFromStartDayDd | `40` | الأمثلة هي Day -2, Day -1, Day 1, Day 2 من بداية المشروع. |
| DayFromStartDd | `56` | الأمثلة هي -2, -1, 1, 2 |
| DayFromStartDdd | `55` | الأمثلة هي D-2, D-1, D1, D2 |
| DayOfMonthDd | `21` | الأمثلة هي 30, 1 |
| DayOfYearDd | `118` | الأمثلة هي 77, 78 |
| DayOfYearDdYyy | `116` | الأمثلة هي 77 '10, 78 '10 |
| DayOfYearDdYyyy | `117` | الأمثلة هي 77 2010, 78 2010 |
| DayDdMmYyyy | `256` | المثال هو 19/07/2016. |
| HalfYearH | `128` | الأمثلة هي 1, 2. يتطلب وحدة الوقت أن تكون TimescaleHalfYears. |
| HalfYearHh | `127` | الأمثلة هي H1, H2 |
| HalfYearHhYyy | `126` | الأمثلة هي H1 '10, H2 '10 |
| HalfYearHhhHalf | `123` | الأمثلة هي 1st Half, 2d Half |
| HalfYearHHyy | `129` | الأمثلة هي 1H10, 2H10 |
| HalfYearHlfH | `125` | الأمثلة هي Half 1, Half 2 |
| HalfYearHlfHYyyy | `124` | الأمثلة هي Half 1, 2010; Half 2, 2010 |
| HalfYearFromEndH | `135` | الأمثلة هي 2, 1, -1, -2. نصف سنوات من تاريخ نهاية المشروع. |
| HalfYearFromEndHalfH | `133` | الأمثلة هي Half 2, Half 1, Half -1, Half -2 |
| HalfYearFromEndHh | `134` | الأمثلة هي H2, H1, H-1, H-2 |
| HalfYearFromStartH | `132` | الأمثلة هي -2, -1, 1, 2. نصف سنوات من تاريخ بداية المشروع. |
| HalfYearFromStartHalfH | `130` | الأمثلة هي Half -2, Half -1, Half 1, Half 2 |
| HalfYearFromStartHh | `131` | الأمثلة هي H-2, H-1, H1, H2 |
| HourDddMmmDdHhAm | `28` | الأمثلة هي Wed Mar 18, 8 AM; Wed Mar 18, 9 AM. يتطلب أن تكون وحدة الوقت TimescaleHours. |
| HourHh | `32` | الأمثلة هي 8, 9, 10, 11 |
| HourHhMmAm | `30` | الأمثلة هي 8:00 AM, 9:00 AM |
| HourHhAm | `31` | الأمثلة هي 8AM, 9AM |
| HourMmDdHhAm | `120` | الأمثلة هي 3/18 8 AM, 3/18 9 AM |
| HourMmmDdHhAm | `29` | الأمثلة هي Mar 18, 8 AM; Mar 18, 9 AM |
| HourFromEndHh | `77` | الأمثلة هي 3, 2, 1, -1, -2 ساعات من نهاية المشروع. |
| HourFromEndHhh | `76` | الأمثلة هي H3, H2, H1, H-1, H-2 |
| HourFromEndHourHh | `39` | الأمثلة هي ساعة 3, ساعة 2, ساعة 1, ساعة -1, ساعة -2 |
| HourFromStartHh | `79` | الأمثلة هي -2, -1, 1, 2, 3 ساعات من بداية المشروع. |
| HourFromStartHhh | `78` | الأمثلة هي H-2, H-1, H1, H2, H3 |
| HourFromStartHourHh | `38` | الأمثلة هي ساعة -2, ساعة -1, ساعة 1, ساعة 2, ساعة 3 |
| MinuteHhMmAm | `33` | الأمثلة هي 8:00 AM, 8:01 AM, 8:02 AM. يتطلب أن تكون وحدة الوقت TimescaleMinutes. |
| MinuteMm | `34` | الأمثلة هي 0, 1, 2, ..., 59 دقائق |
| MinuteFromEndMinuteMm | `37` | الأمثلة هي دقيقة 181, دقيقة 180, ..., دقيقة 1, دقيقة -1 من نهاية المشروع. |
| MinuteFromEndMm | `81` | الأمثلة هي 181, 180, ..., 1, -1 |
| MinuteFromEndMmm | `80` | الأمثلة هي M181, M180, ..., M1, M-1 |
| MinuteFromStartMinuteMm | `36` | الأمثلة هي دقيقة -2, دقيقة -1, دقيقة 1, ... دقيقة 180 من بداية المشروع. |
| MinuteFromStartMm | `83` | الأمثلة هي -2, -1, 1, ..., 180 |
| MinuteFromStartMmm | `82` | الأمثلة هي M-2, M-1, M1, ..., M180 |
| MonthM | `11` | الأمثلة هي M, A, M, J, J. يتطلب أن تكون وحدة الوقت TimescaleMonths. |
| MonthMm | `57` | الأمثلة هي 11, 12, 1, 2 |
| MonthMmYy | `86` | الأمثلة هي 3/10, 4/10, 5/10 |
| MonthMmYyy | `85` | الأمثلة هي 3 '10, 4 '10, 5 '10 |
| MonthMmm | `10` | الأمثلة هي Mar, Apr, May |
| MonthMmmYyy | `8` | الأمثلة هي Mar '10, Apr '10, May '10 |
| MonthMmmm | `9` | الأمثلة هي March, April, May |
| MonthMmmmYyyy | `7` | الأمثلة هي March 2010, April 2010, May 2010 |
| MonthFromEndMm | `59` | الأمثلة هي 2, 1, -1, -2 شهرًا من نهاية المشروع. |
| MonthFromEndMmm | `58` | الأمثلة هي M2, M1, M-1, M-2 |
| MonthFromEndMonthMm | `45` | الأمثلة هي Month 2, Month 1, Month -1, Month -2 |
| MonthFromStartMm | `61` | الأمثلة هي -2, -2, 1, 2 شهرًا من بداية المشروع. |
| MonthFromStartMmm | `60` | الأمثلة هي M-2, M-1, M1, M2 |
| MonthFromStartMonthMm | `44` | الأمثلة هي Month -2, Month -1, Month 1, Month 2 |
| QuarterQ | `62` | الأمثلة هي 3, 4, 1. يتطلب أن تكون وحدة الوقت TimescaleQuarters. |
| QuarterQq | `6` | الأمثلة هي Q3, Q4, Q1 |
| QuarterQqYyy | `4` | الأمثلة هي Q3 '10, Q4 '10, Q1 '11 |
| QuarterQqqQuarter | `2` | الأمثلة هي 3rd Quarter, 1st Quarter |
| QuarterQQyy | `51` | الأمثلة هي 3Q10, 4Q10, 1Q11 |
| QuarterQtrQ | `5` | الأمثلة هي Qtr3, Qtr4, Qtr1 |
| QuarterQtrQYyyy | `3` | الأمثلة هي Qtr3, 2010; Qtr4, 2010; Qtr1, 2011 |
| QuarterFromEndQ | `64` | الأمثلة هي 5, 4, 3, 2, 1, -1 ربعًا من نهاية المشروع. |
| QuarterFromEndQq | `63` | الأمثلة هي Q5, Q4, Q3, Q2, Q1, Q-1 |
| QuarterFromEndQuarterQ | `47` | الأمثلة هي Quarter 5, Quarter 4, Quarter 3, Quarter 2, Quarter 1, Quarter -1 |
| QuarterFromStartQ | `66` | الأمثلة هي -5, -4, -3, -2, -1, 1 ربعًا من بداية المشروع. |
| QuarterFromStartQq | `65` | الأمثلة هي Q-5, Q-4, Q-3, Q-2, Q-1, Q1 |
| QuarterFromStartQuarterQ | `46` | الأمثلة هي Quarter -5, Quarter -4, Quarter -3, Quarter -2, Quarter -1, Quarter 1 |
| ThirdsOfMonthsDd | `136` | الأمثلة هي 1, 11, 21, 1. يتطلب أن تكون وحدة الوقت TimescaleThirdsOfMonths. |
| ThirdsOfMonthsDdd | `137` | الأمثلة هي B, M, E, B |
| ThirdsOfMonthsDddd | `138` | الأمثلة هي البداية، الوسط، النهاية، البداية |
| ThirdsOfMonthsMmDd | `139` | المثال هو 3/1. |
| ThirdsOfMonthsMmDdYy | `145` | المثال هو 3/1/10. |
| ThirdsOfMonthsMmDdd | `140` | الأمثلة هي 3/B، 3/M، 3/E، 4/B |
| ThirdsOfMonthsMmDddYy | `146` | المثال هو 3/B/10. |
| ThirdsOfMonthsMmmDd | `142` | الأمثلة هي مارس 1، مارس 11، مارس 21، أبريل 1 |
| ThirdsOfMonthsMmmDdYy | `147` | الأمثلة هي مارس 1، ’10؛ مارس 11، ’10؛ مارس 21، ’10؛ أبريل 1، 10 |
| ThirdsOfMonthsMmmDdd | `143` | الأمثلة هي مارس B، مارس M، مارس E، أبريل B |
| ThirdsOfMonthsMmmDddYy | `148` | الأمثلة هي مارس B، ’10؛ مارس M، ’10؛ مارس E، ’10؛ أبريل B ’10 |
| ThirdsOfMonthsMmmmDd | `144` | الأمثلة هي مارس 1، مارس 11، مارس 21، أبريل 1 |
| ThirdsOfMonthsMmmmDdYyyy | `149` | الأمثلة هي مارس 1، 2010؛ مارس 11، 2010؛ مارس 21، 2010؛ أبريل 1، 2010 |
| ThirdsOfMonthsMmmmDddd | `141` | الأمثلة هي مارس البداية، مارس الوسط، مارس النهاية، أبريل البداية |
| ThirdsOfMonthsMmmmDdddYyyy | `150` | الأمثلة هي مارس البداية، 2010؛ مارس الوسط، 2010؛ مارس النهاية، 2010؛ أبريل البداية، 2010 |
| WeekDddDd | `88` | الأمثلة هي الأحد 21، الأحد 28، الأحد 4. يتطلب وحدة الوقت أن تكون TimescaleWeeks. |
| WeekDddMDd | `97` | الأمثلة هي الأحد M 21، الأحد M 28، الأحد A 4 |
| WeekDddMmDd | `90` | الأمثلة هي الأحد 3/21، الأحد 3/28، الأحد 4/4 |
| WeekDddMmDdYy | `100` | الأمثلة هي الأحد 3/21/10، الأحد 3/28/10، الأحد 4/4/10 |
| WeekDddMmmDd | `93` | الأمثلة هي الأحد مارس 21، الأحد مارس 28، الأحد أبريل 4 |
| WeekDddMmmDdYyy | `101` | الأمثلة هي الأحد مارس 21، ’10؛ الأحد مارس 28، ’10؛ الأحد أبريل 4، ’10 |
| WeekDddMmmmDd | `96` | الأمثلة هي الأحد مارس 21، الأحد مارس 28، الأحد أبريل 4 |
| WeekDddMmmmDdYyy | `102` | الأمثلة هي الأحد مارس 21، ’10؛ الأحد مارس 28، ’10؛ الأحد أبريل 4، ’10 |
| WeekDddWw | `103` | الأمثلة هي الأحد 12، الأحد 13، الأحد 14 |
| WeekDdiMDd | `98` | الأمثلة هي الأحد M 21، الأحد M 28، الأحد A 4 |
| WeekDdiMmDd | `91` | الأمثلة هي الأحد 3/21. الأحد 3/28، الأحد 4/4 |
| WeekDdiMmmDd | `94` | الأمثلة هي الأحد مارس 21، الأحد مارس 28، الأحد أبريل 4 |
| WeekDiMDd | `99` | الأمثلة هي S M 21, S M 28, S A 4 |
| WeekDiMmDd | `92` | الأمثلة هي S 3/21, S 3/28, S 4/4 |
| WeekDiMmmDd | `95` | الأمثلة هي S Mar 21, S Mar 28, S Apr 4 |
| WeekMDd | `89` | الأمثلة هي M21, M28, A 4 |
| WeekMmDd | `17` | الأمثلة هي 3/21, 3/28, 4/4 |
| WeekMmDdYy | `16` | المثال هو '3/21/10'. |
| WeekMmmDd | `15` | الأمثلة هي Mar 21, Mar 28, Apr 4 |
| WeekMmmDdYyy | `13` | الأمثلة هي Mar 21, '10; Mar 28, '10; Apr 4, '10 |
| WeekMmmmDd | `14` | الأمثلة هي March 21, March 28, April 4 |
| WeekMmmmDdYyyy | `12` | الأمثلة هي March 21, 2010; March 28, 2010; April 4, 2010 |
| WeekDayOfMonthDd | `87` | الأمثلة هي 21, 28, 4 |
| WeekFromEndWeekWw | `43` | الأمثلة هي الأسبوع 2, الأسبوع 1, الأسبوع -1 من نهاية المشروع. |
| WeekFromEndWw | `68` | الأمثلة هي 2, 1, -1 |
| WeekFromEndWww | `67` | الأمثلة هي W2, W1, W-1 |
| WeekFromStartWeekWw | `42` | الأمثلة هي الأسبوع -1, الأسبوع 1, الأسبوع 2 من بداية المشروع. |
| WeekFromStartWw | `70` | الأمثلة هي -1, 1, 2 |
| WeekFromStartWww | `69` | الأمثلة هي W-1, W1, W2 |
| WeekNumberDdWw | `104` | الأمثلة هي 1 12, 1 13, 1 14 (اليوم 1 من الأسبوع 12, اليوم 1 من الأسبوع 13, وهكذا) |
| WeekNumberWw | `50` | الأمثلة هي 12, 13, 14 |
| YearYy | `75` | الأمثلة هي 10, 11, 12. يتطلب أن تكون وحدة الوقت TimescaleYears. |
| YearYyy | `1` | الأمثلة هي '10, '11, '12 |
| YearYyyy | `0` | الأمثلة هي 2010, 2011, 2012 |
| YearFromEndYearYy | `49` | الأمثلة هي السنة 2, السنة 1, السنة -1 من نهاية المشروع. |
| YearFromEndYy | `72` | الأمثلة هي 2, 1, -1 |
| YearFromEndYyy | `71` | الأمثلة هي Y2, Y1, Y-1 |
| YearFromStartYearYy | `48` | الأمثلة هي السنة -1, السنة 1, السنة 2 من بداية المشروع. |
| YearFromStartYy | `74` | الأمثلة هي -1, 1, 2 |
| YearFromStartYyy | `73` | الأمثلة هي Y-1, Y1, Y2 |

## الأمثلة

يعرض كيفية تخصيص تسميات طبقة مقياس الوقت.

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");

// إضافة روابط المهام
project.TaskLinks.Add(project.RootTask.Children.Add("Task 1"), project.RootTask.Children.Add("Task 2"));

var view = (GanttChartView)project.DefaultView;

// ضبط طبقات مقياس الوقت

// ضبط الطبقة العليا
// ضبط الطبقة العليا لمقياس الوقت في عرض مخطط جانت.
view.MiddleTimescaleTier = new TimescaleTier();
// ضبط وحدة مقياس الوقت <see cref=\"T:Aspose.Tasks.Visualization.TimescaleUnit\" /> للطبقة الزمنية.
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
// ضبط الفاصل الزمني لوحدة الوقت الذي تُظهر فيه التسميات للطبقة.
view.MiddleTimescaleTier.Count = 1;
// ضبط تسمية التاريخ <see cref=\"T:Aspose.Tasks.Visualization.DateLabel\" /> للطبقة الزمنية.
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
// ضبط طريقة محاذاة التسميات داخل كل فترة زمنية للطبقة (<see cref=\"T:System.Drawing.StringAlignment\" />).
view.MiddleTimescaleTier.Alignment = HorizontalStringAlignment.Center;
// تعيين قيمة تشير إلى ما إذا كان يجب إظهار علامات الفواصل التي تفصل الفترات الزمنية في المستوى.
view.MiddleTimescaleTier.ShowTicks = true;
// تعيين قيمة تشير إلى ما إذا كان يجب أن تستند تسميات المستوى إلى السنة المالية.
view.MiddleTimescaleTier.UsesFiscalYear = true;

// تمت الإضافة لتحسين التصور.
view.TopTimescaleTier = new TimescaleTier(TimescaleUnit.Months, 1);

// تخصيص تواريخ المستوى الأوسط.
view.TopTimescaleTier.DateTimeConverter = date =>
    new[] { "Янв.", "Фев.", "Мар.", "Апр.", "Май", "Июнь", "Июль", "Авг.", "Сен.", "Окт.", "Ноя.", "Дек." }[date.Month - 1];

project.Set(Prj.TimescaleStart, new DateTime(2012, 7, 30));
project.Set(Prj.TimescaleFinish, new DateTime(2012, 10, 6));

// استخدم خيار 'Timescale.DefinedInView' لتصوير المقاييس الزمنية باستخدام إعدادات المقاييس الزمنية المعرفة في العرض (view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier).
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "CustomizeTimescaleTierLabels_out.pdf", pdfSaveOptions);
```

### انظر أيضًا

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


