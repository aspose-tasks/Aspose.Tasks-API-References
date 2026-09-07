---
title: "Enum DateLabel"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Visualization.DateLabel enum. टाइमस्केल में तिथि और समय लेबल के प्रदर्शन प्रारूप को निर्दिष्ट करता है"
type: docs
weight: 2980
url: /hi/net/aspose.tasks.visualization/datelabel/
---
## DateLabel enumeration

टाइमस्केल में तिथि और समय लेबल के प्रदर्शन स्वरूप को निर्दिष्ट करता है।

```csharp
public enum DateLabel
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| None | `35` | कोई तिथि प्रदर्शित नहीं की गई है। |
| DayDdd | `19` | उदाहरण हैं Mon, Tue। |
| DayDddDd | `105` | उदाहरण हैं Mon 30, Tue 1 |
| DayDddMDd | `112` | उदाहरण हैं Mon S 30, Tue O 1 |
| DayDddMmDd | `108` | उदाहरण हैं Mon 9/30, Tue 10/1 |
| DayDddMmDdYy | `52` | उदाहरण हैं Mon 9/30/02, Tue 10/1/02 |
| DayDddMmmDd | `23` | उदाहरण हैं Mon Sep 30, Tue Oct 1 |
| DayDddMmmDdYyy | `22` | उदाहरण हैं Mon Sep 30 '02, Tue Oct 1 '02 |
| DayDddMmmmDd | `111` | उदाहरण हैं Mon September 30, Tue October 1 |
| DayDddd | `18` | उदाहरण हैं Tuesday, Wednesday। |
| DayDdi | `119` | उदाहरण हैं Mo, Tu |
| DayDdiDd | `106` | उदाहरण हैं Mo 30, Tu 1 |
| DayDdiMDd | `113` | उदाहरण हैं Mo S 30, Tu O 1 |
| DayDdiMmDd | `109` | उदाहरण हैं Mo 9/30, Tu 10/1 |
| DayDi | `20` | उदाहरण हैं M, T |
| DayDiDdSpace | `107` | उदाहरण हैं M 30, T 1 |
| DayDiMDd | `114` | उदाहरण हैं M S 30, T O 1 |
| DayDiMmDd | `110` | उदाहरण हैं M 9/30, T 10/1 |
| DayDiDdNoSpace | `121` | उदाहरण हैं M30, T1 |
| DayMDd | `115` | उदाहरण हैं S 30, O 1 |
| DayMmDd | `27` | उदाहरण हैं 9/30, 10/1 |
| DayMmDdYy | `26` | उदाहरण हैं 9/30/02, 10/1/02 |
| DayMmmDd | `25` | उदाहरण हैं Sep 30, Oct 1 |
| DayMmmDdYyy | `24` | उदाहरण हैं Sep 30 '02, Oct 10 '02 |
| DayFromEndDayDd | `41` | उदाहरण हैं Day 2, Day 1, Day -1, Day -2 परियोजना के अंत से। |
| DayFromEndDd | `54` | उदाहरण हैं 2, 1, -1, -2 |
| DayFromEndDdd | `53` | उदाहरण हैं D2, D1, D-1, D-2 |
| DayFromStartDayDd | `40` | उदाहरण हैं Day -2, Day -1, Day 1, Day 2 परियोजना की शुरुआत से। |
| DayFromStartDd | `56` | उदाहरण हैं -2, -1, 1, 2 |
| DayFromStartDdd | `55` | उदाहरण हैं D-2, D-1, D1, D2 |
| DayOfMonthDd | `21` | उदाहरण हैं 30, 1 |
| DayOfYearDd | `118` | उदाहरण हैं 77, 78 |
| DayOfYearDdYyy | `116` | उदाहरण हैं 77 '10, 78 '10 |
| DayOfYearDdYyyy | `117` | उदाहरण हैं 77 2010, 78 2010 |
| DayDdMmYyyy | `256` | उदाहरण है 19/07/2016. |
| HalfYearH | `128` | उदाहरण हैं 1, 2. समय इकाई को TimescaleHalfYears होना चाहिए। |
| HalfYearHh | `127` | उदाहरण हैं H1, H2 |
| HalfYearHhYyy | `126` | उदाहरण हैं H1 '10, H2 '10 |
| HalfYearHhhHalf | `123` | उदाहरण हैं 1st Half, 2d Half |
| HalfYearHHyy | `129` | उदाहरण हैं 1H10, 2H10 |
| HalfYearHlfH | `125` | उदाहरण हैं Half 1, Half 2 |
| HalfYearHlfHYyyy | `124` | उदाहरण हैं Half 1, 2010; Half 2, 2010 |
| HalfYearFromEndH | `135` | उदाहरण हैं 2, 1, -1, -2. परियोजना के समाप्ति तिथि से अर्ध वर्ष। |
| HalfYearFromEndHalfH | `133` | उदाहरण हैं Half 2, Half 1, Half -1, Half -2 |
| HalfYearFromEndHh | `134` | उदाहरण हैं H2, H1, H-1, H-2 |
| HalfYearFromStartH | `132` | उदाहरण हैं -2, -1, 1, 2. परियोजना की शुरुआत तिथि से अर्ध वर्ष। |
| HalfYearFromStartHalfH | `130` | उदाहरण हैं Half -2, Half -1, Half 1, Half 2 |
| HalfYearFromStartHh | `131` | उदाहरण हैं H-2, H-1, H1, H2 |
| HourDddMmmDdHhAm | `28` | उदाहरण हैं Wed Mar 18, 8 AM; Wed Mar 18, 9 AM. समय इकाई TimescaleHours होना चाहिए। |
| HourHh | `32` | उदाहरण हैं 8, 9, 10, 11 |
| HourHhMmAm | `30` | उदाहरण हैं 8:00 AM, 9:00 AM |
| HourHhAm | `31` | उदाहरण हैं 8AM, 9AM |
| HourMmDdHhAm | `120` | उदाहरण हैं 3/18 8 AM, 3/18 9 AM |
| HourMmmDdHhAm | `29` | उदाहरण हैं Mar 18, 8 AM; Mar 18, 9 AM |
| HourFromEndHh | `77` | उदाहरण हैं 3, 2, 1, -1, -2 घंटे प्रोजेक्ट समाप्ति से। |
| HourFromEndHhh | `76` | उदाहरण हैं H3, H2, H1, H-1, H-2 |
| HourFromEndHourHh | `39` | उदाहरण हैं घंटा 3, घंटा 2, घंटा 1, घंटा -1, घंटा -2 |
| HourFromStartHh | `79` | उदाहरण हैं -2, -1, 1, 2, 3 घंटे प्रोजेक्ट प्रारंभ से। |
| HourFromStartHhh | `78` | उदाहरण हैं H-2, H-1, H1, H2, H3 |
| HourFromStartHourHh | `38` | उदाहरण हैं घंटा -2, घंटा -1, घंटा 1, घंटा 2, घंटा 3 |
| MinuteHhMmAm | `33` | उदाहरण हैं 8:00 AM, 8:01 AM, 8:02 AM. समय इकाई TimescaleMinutes होना चाहिए। |
| MinuteMm | `34` | उदाहरण हैं 0, 1, 2, ..., 59 मिनट |
| MinuteFromEndMinuteMm | `37` | उदाहरण हैं मिनट 181, मिनट 180, ..., मिनट 1, मिनट -1 प्रोजेक्ट समाप्ति से। |
| MinuteFromEndMm | `81` | उदाहरण हैं 181, 180, ..., 1, -1 |
| MinuteFromEndMmm | `80` | उदाहरण हैं M181, M180, ..., M1, M-1 |
| MinuteFromStartMinuteMm | `36` | उदाहरण हैं मिनट -2, मिनट -1, मिनट 1, ... मिनट 180 प्रोजेक्ट प्रारंभ से। |
| MinuteFromStartMm | `83` | उदाहरण हैं -2, -1, 1, ..., 180 |
| MinuteFromStartMmm | `82` | उदाहरण हैं M-2, M-1, M1, ..., M180 |
| MonthM | `11` | उदाहरण हैं M, A, M, J, J. समय इकाई TimescaleMonths होना चाहिए। |
| MonthMm | `57` | उदाहरण हैं 11, 12, 1, 2 |
| MonthMmYy | `86` | उदाहरण हैं 3/10, 4/10, 5/10 |
| MonthMmYyy | `85` | उदाहरण हैं 3 '10, 4 '10, 5 '10 |
| MonthMmm | `10` | उदाहरण हैं Mar, Apr, May |
| MonthMmmYyy | `8` | उदाहरण हैं Mar '10, Apr '10, May '10 |
| MonthMmmm | `9` | उदाहरण हैं March, April, May |
| MonthMmmmYyyy | `7` | उदाहरण हैं March 2010, April 2010, May 2010 |
| MonthFromEndMm | `59` | उदाहरण हैं 2, 1, -1, -2 months प्रोजेक्ट अंत से। |
| MonthFromEndMmm | `58` | उदाहरण हैं M2, M1, M-1, M-2 |
| MonthFromEndMonthMm | `45` | उदाहरण हैं Month 2, Month 1, Month -1, Month -2 |
| MonthFromStartMm | `61` | उदाहरण हैं -2, -2, 1, 2 months प्रोजेक्ट शुरू से। |
| MonthFromStartMmm | `60` | उदाहरण हैं M-2, M-1, M1, M2 |
| MonthFromStartMonthMm | `44` | उदाहरण हैं Month -2, Month -1, Month 1, Month 2 |
| QuarterQ | `62` | उदाहरण हैं 3, 4, 1. समय इकाई TimescaleQuarters होना चाहिए। |
| QuarterQq | `6` | उदाहरण हैं Q3, Q4, Q1 |
| QuarterQqYyy | `4` | उदाहरण हैं Q3 '10, Q4 '10, Q1 '11 |
| QuarterQqqQuarter | `2` | उदाहरण हैं 3rd Quarter, 1st Quarter |
| QuarterQQyy | `51` | उदाहरण हैं 3Q10, 4Q10, 1Q11 |
| QuarterQtrQ | `5` | उदाहरण हैं Qtr3, Qtr4, Qtr1 |
| QuarterQtrQYyyy | `3` | उदाहरण हैं Qtr3, 2010; Qtr4, 2010; Qtr1, 2011 |
| QuarterFromEndQ | `64` | उदाहरण हैं 5, 4, 3, 2, 1, -1 quarters प्रोजेक्ट अंत से। |
| QuarterFromEndQq | `63` | उदाहरण हैं Q5, Q4, Q3, Q2, Q1, Q-1 |
| QuarterFromEndQuarterQ | `47` | उदाहरण हैं Quarter 5, Quarter 4, Quarter 3, Quarter 2, Quarter 1, Quarter -1 |
| QuarterFromStartQ | `66` | उदाहरण हैं -5, -4, -3, -2, -1, 1 quarters प्रोजेक्ट शुरू से। |
| QuarterFromStartQq | `65` | उदाहरण हैं Q-5, Q-4, Q-3, Q-2, Q-1, Q1 |
| QuarterFromStartQuarterQ | `46` | उदाहरण हैं Quarter -5, Quarter -4, Quarter -3, Quarter -2, Quarter -1, Quarter 1 |
| ThirdsOfMonthsDd | `136` | उदाहरण हैं 1, 11, 21, 1. समय इकाई TimescaleThirdsOfMonths होना चाहिए। |
| ThirdsOfMonthsDdd | `137` | उदाहरण हैं B, M, E, B |
| ThirdsOfMonthsDddd | `138` | उदाहरण हैं शुरुआत, मध्य, अंत, शुरुआत |
| ThirdsOfMonthsMmDd | `139` | उदाहरण है 3/1. |
| ThirdsOfMonthsMmDdYy | `145` | उदाहरण है 3/1/10. |
| ThirdsOfMonthsMmDdd | `140` | उदाहरण हैं 3/B, 3/M, 3/E, 4/B |
| ThirdsOfMonthsMmDddYy | `146` | उदाहरण है 3/B/10. |
| ThirdsOfMonthsMmmDd | `142` | उदाहरण हैं मार्च 1, मार्च 11, मार्च 21, अप्रैल 1 |
| ThirdsOfMonthsMmmDdYy | `147` | उदाहरण हैं मार्च 1, '10; मार्च 11, '10; मार्च 21, '10; अप्रैल 1, 10 |
| ThirdsOfMonthsMmmDdd | `143` | उदाहरण हैं मार्च B, मार्च M, मार्च E, अप्रैल B |
| ThirdsOfMonthsMmmDddYy | `148` | उदाहरण हैं मार्च B, '10; मार्च M, '10; मार्च E, '10; अप्रैल B '10 |
| ThirdsOfMonthsMmmmDd | `144` | उदाहरण हैं मार्च 1, मार्च 11, मार्च 21, अप्रैल 1 |
| ThirdsOfMonthsMmmmDdYyyy | `149` | उदाहरण हैं मार्च 1, 2010; मार्च 11, 2010; मार्च 21, 2010; अप्रैल 1, 2010 |
| ThirdsOfMonthsMmmmDddd | `141` | उदाहरण हैं मार्च शुरुआत, मार्च मध्य, मार्च अंत, अप्रैल शुरुआत |
| ThirdsOfMonthsMmmmDdddYyyy | `150` | उदाहरण हैं मार्च शुरुआत, 2010; मार्च मध्य, 2010; मार्च अंत, 2010; अप्रैल शुरुआत, 2010 |
| WeekDddDd | `88` | उदाहरण हैं रविवार 21, रविवार 28, रविवार 4. समय इकाई को TimescaleWeeks होना चाहिए। |
| WeekDddMDd | `97` | उदाहरण हैं रविवार M 21, रविवार M 28, रविवार A 4 |
| WeekDddMmDd | `90` | उदाहरण हैं रविवार 3/21, रविवार 3/28, रविवार 4/4 |
| WeekDddMmDdYy | `100` | उदाहरण हैं रविवार 3/21/10, रविवार 3/28/10, रविवार 4/4/10 |
| WeekDddMmmDd | `93` | उदाहरण हैं रविवार मार्च 21, रविवार मार्च 28, रविवार अप्रैल 4 |
| WeekDddMmmDdYyy | `101` | उदाहरण हैं रविवार मार्च 21, '10; रविवार मार्च 28, '10; रविवार अप्रैल 4, '10 |
| WeekDddMmmmDd | `96` | उदाहरण हैं रविवार मार्च 21, रविवार मार्च 28, रविवार अप्रैल 4 |
| WeekDddMmmmDdYyy | `102` | उदाहरण हैं रविवार मार्च 21, '10; रविवार मार्च 28, '10; रविवार अप्रैल 4, '10 |
| WeekDddWw | `103` | उदाहरण हैं रविवार 12, रविवार 13, रविवार 14 |
| WeekDdiMDd | `98` | उदाहरण हैं रविवार M 21, रविवार M 28, रविवार A 4 |
| WeekDdiMmDd | `91` | उदाहरण हैं रविवार 3/21. रविवार 3/28, रविवार 4/4 |
| WeekDdiMmmDd | `94` | उदाहरण हैं रविवार मार्च 21, रविवार मार्च 28, रविवार अप्रैल 4 |
| WeekDiMDd | `99` | उदाहरण हैं S M 21, S M 28, S A 4 |
| WeekDiMmDd | `92` | उदाहरण हैं S 3/21, S 3/28, S 4/4 |
| WeekDiMmmDd | `95` | उदाहरण हैं S Mar 21, S Mar 28, S Apr 4 |
| WeekMDd | `89` | उदाहरण हैं M21, M28, A 4 |
| WeekMmDd | `17` | उदाहरण हैं 3/21, 3/28, 4/4 |
| WeekMmDdYy | `16` | उदाहरण है '3/21/10'। |
| WeekMmmDd | `15` | उदाहरण हैं Mar 21, Mar 28, Apr 4 |
| WeekMmmDdYyy | `13` | उदाहरण हैं Mar 21, '10; Mar 28, '10; Apr 4, '10 |
| WeekMmmmDd | `14` | उदाहरण हैं March 21, March 28, April 4 |
| WeekMmmmDdYyyy | `12` | उदाहरण हैं March 21, 2010; March 28, 2010; April 4, 2010 |
| WeekDayOfMonthDd | `87` | उदाहरण हैं 21, 28, 4 |
| WeekFromEndWeekWw | `43` | उदाहरण हैं Week 2, Week 1, Week -1 प्रोजेक्ट समाप्ति से। |
| WeekFromEndWw | `68` | उदाहरण हैं 2, 1, -1 |
| WeekFromEndWww | `67` | उदाहरण हैं W2, W1, W-1 |
| WeekFromStartWeekWw | `42` | उदाहरण हैं Week -1, Week 1, Week 2 प्रोजेक्ट प्रारम्भ से। |
| WeekFromStartWw | `70` | उदाहरण हैं -1, 1, 2 |
| WeekFromStartWww | `69` | उदाहरण हैं W-1, W1, W2 |
| WeekNumberDdWw | `104` | उदाहरण हैं 1 12, 1 13, 1 14 (सप्ताह 12 का दिन 1, सप्ताह 13 का दिन 1, आदि) |
| WeekNumberWw | `50` | उदाहरण हैं 12, 13, 14 |
| YearYy | `75` | उदाहरण हैं 10, 11, 12. समय इकाई को TimescaleYears होना चाहिए। |
| YearYyy | `1` | उदाहरण हैं '10, '11, '12 |
| YearYyyy | `0` | उदाहरण हैं 2010, 2011, 2012 |
| YearFromEndYearYy | `49` | उदाहरण हैं Year 2, Year 1, Year -1 प्रोजेक्ट समाप्ति से। |
| YearFromEndYy | `72` | उदाहरण हैं 2, 1, -1 |
| YearFromEndYyy | `71` | उदाहरण हैं Y2, Y1, Y-1 |
| YearFromStartYearYy | `48` | उदाहरण हैं Year -1, Year 1, Year 2 प्रोजेक्ट प्रारम्भ से। |
| YearFromStartYy | `74` | उदाहरण हैं -1, 1, 2 |
| YearFromStartYyy | `73` | उदाहरण हैं Y-1, Y1, Y2 |

## उदाहरण

टाइमस्केल टियर लेबल को कस्टमाइज़ करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");

// टास्क लिंक जोड़ें
project.TaskLinks.Add(project.RootTask.Children.Add("Task 1"), project.RootTask.Children.Add("Task 2"));

var view = (GanttChartView)project.DefaultView;

// टाइमस्केल टियर्स को ट्यून करें

// शीर्ष टियर को ट्यून करें
// Gantt चार्ट व्यू का शीर्ष टाइमस्केल टियर सेट करें।
view.MiddleTimescaleTier = new TimescaleTier();
// टाइमस्केल टियर के लिए टाइमस्केल यूनिट <see cref=\"T:Aspose.Tasks.Visualization.TimescaleUnit\" /> सेट करें।
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
// टियर के लिए लेबल दिखाने वाले समय इकाई अंतराल को सेट करें।
view.MiddleTimescaleTier.Count = 1;
// टाइमस्केल टियर के लिए तिथि लेबल <see cref=\"T:Aspose.Tasks.Visualization.DateLabel\" /> सेट करें।
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
// टियर के प्रत्येक समय अवधि में लेबल को कैसे संरेखित किया जाए, सेट करें (<see cref=\"T:System.Drawing.StringAlignment\" />).
view.MiddleTimescaleTier.Alignment = HorizontalStringAlignment.Center;
// टियर में समय अवधि को अलग करने वाले टिक मार्क दिखाने चाहिए या नहीं, यह दर्शाने के लिए मान सेट करें।
view.MiddleTimescaleTier.ShowTicks = true;
// वित्तीय वर्ष के आधार पर टियर लेबल सेट करने के लिए मान निर्धारित करें।
view.MiddleTimescaleTier.UsesFiscalYear = true;

// बेहतर दृश्यता के लिए जोड़ा गया
view.TopTimescaleTier = new TimescaleTier(TimescaleUnit.Months, 1);

// मध्य टियर की तिथियों को अनुकूलित करें
view.TopTimescaleTier.DateTimeConverter = date =>
    new[] { "Янв.", "Фев.", "Мар.", "Апр.", "Май", "Июнь", "Июль", "Авг.", "Сен.", "Окт.", "Ноя.", "Дек." }[date.Month - 1];

project.Set(Prj.TimescaleStart, new DateTime(2012, 7, 30));
project.Set(Prj.TimescaleFinish, new DateTime(2012, 10, 6));

// व्यू में परिभाषित टाइमस्केल सेटिंग्स (view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier) का उपयोग करके टाइमस्केल रेंडर करने के लिए 'Timescale.DefinedInView' विकल्प का उपयोग करें।
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "CustomizeTimescaleTierLabels_out.pdf", pdfSaveOptions);
```

### संबंधित देखें

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


