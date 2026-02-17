---
title: Enum DateLabel
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.DateLabel enum. Specifies the display format for date and time labels in a timescale
type: docs
weight: 2960
url: /net/aspose.tasks.visualization/datelabel/
---
## DateLabel enumeration

Specifies the display format for date and time labels in a timescale.

```csharp
public enum DateLabel
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| None | `35` | No date is displayed. |
| DayDdd | `19` | Examples are Mon, Tue. |
| DayDddDd | `105` | Examples are Mon 30, Tue 1 |
| DayDddMDd | `112` | Examples are Mon S 30, Tue O 1 |
| DayDddMmDd | `108` | Examples are Mon 9/30, Tue 10/1 |
| DayDddMmDdYy | `52` | Examples are Mon 9/30/02, Tue 10/1/02 |
| DayDddMmmDd | `23` | Examples are Mon Sep 30, Tue Oct 1 |
| DayDddMmmDdYyy | `22` | Examples are Mon Sep 30 '02, Tue Oct 1 '02 |
| DayDddMmmmDd | `111` | Examples are Mon September 30, Tue October 1 |
| DayDddd | `18` | Examples are Tuesday, Wednesday. |
| DayDdi | `119` | Examples are Mo, Tu |
| DayDdiDd | `106` | Examples are Mo 30, Tu 1 |
| DayDdiMDd | `113` | Examples are Mo S 30, Tu O 1 |
| DayDdiMmDd | `109` | Examples are Mo 9/30, Tu 10/1 |
| DayDi | `20` | Examples are M, T |
| DayDiDdSpace | `107` | Examples are M 30, T 1 |
| DayDiMDd | `114` | Examples are M S 30, T O 1 |
| DayDiMmDd | `110` | Examples are M 9/30, T 10/1 |
| DayDiDdNoSpace | `121` | Examples are M30, T1 |
| DayMDd | `115` | Examples are S 30, O 1 |
| DayMmDd | `27` | Examples are 9/30, 10/1 |
| DayMmDdYy | `26` | Examples are 9/30/02, 10/1/02 |
| DayMmmDd | `25` | Examples are Sep 30, Oct 1 |
| DayMmmDdYyy | `24` | Examples are Sep 30 '02, Oct 10 '02 |
| DayFromEndDayDd | `41` | Examples are Day 2, Day 1, Day -1, Day -2 from the project end. |
| DayFromEndDd | `54` | Examples are 2, 1, -1, -2 |
| DayFromEndDdd | `53` | Examples are D2, D1, D-1, D-2 |
| DayFromStartDayDd | `40` | Examples are Day -2, Day -1, Day 1, Day 2 from the project start. |
| DayFromStartDd | `56` | Examples are -2, -1, 1, 2 |
| DayFromStartDdd | `55` | Examples are D-2, D-1, D1, D2 |
| DayOfMonthDd | `21` | Examples are 30, 1 |
| DayOfYearDd | `118` | Examples are 77, 78 |
| DayOfYearDdYyy | `116` | Examples are 77 '10, 78 '10 |
| DayOfYearDdYyyy | `117` | Examples are 77 2010, 78 2010 |
| DayDdMmYyyy | `256` | Example is 19/07/2016. |
| HalfYearH | `128` | Examples are 1, 2. Requires the time unit to be TimescaleHalfYears. |
| HalfYearHh | `127` | Examples are H1, H2 |
| HalfYearHhYyy | `126` | Examples are H1 '10, H2 '10 |
| HalfYearHhhHalf | `123` | Examples are 1st Half, 2d Half |
| HalfYearHHyy | `129` | Examples are 1H10, 2H10 |
| HalfYearHlfH | `125` | Examples are Half 1, Half 2 |
| HalfYearHlfHYyyy | `124` | Examples are Half 1, 2010; Half 2, 2010 |
| HalfYearFromEndH | `135` | Examples are 2, 1, -1, -2. Half years from the project end date. |
| HalfYearFromEndHalfH | `133` | Examples are Half 2, Half 1, Half -1, Half -2 |
| HalfYearFromEndHh | `134` | Examples are H2, H1, H-1, H-2 |
| HalfYearFromStartH | `132` | Examples are -2, -1, 1, 2. Half years from the project start date. |
| HalfYearFromStartHalfH | `130` | Examples are Half -2, Half -1, Half 1, Half 2 |
| HalfYearFromStartHh | `131` | Examples are H-2, H-1, H1, H2 |
| HourDddMmmDdHhAm | `28` | Examples are Wed Mar 18, 8 AM; Wed Mar 18, 9 AM. Requires the time unit to be TimescaleHours. |
| HourHh | `32` | Examples are 8, 9, 10, 11 |
| HourHhMmAm | `30` | Examples are 8:00 AM, 9:00 AM |
| HourHhAm | `31` | Examples are 8AM, 9AM |
| HourMmDdHhAm | `120` | Examples are 3/18 8 AM, 3/18 9 AM |
| HourMmmDdHhAm | `29` | Examples are Mar 18, 8 AM; Mar 18, 9 AM |
| HourFromEndHh | `77` | Examples are 3, 2, 1, -1, -2 hours from the project end. |
| HourFromEndHhh | `76` | Examples are H3, H2, H1, H-1, H-2 |
| HourFromEndHourHh | `39` | Examples are Hour 3, Hour 2, Hour 1, Hour -1, Hour -2 |
| HourFromStartHh | `79` | Examples are -2, -1, 1, 2, 3 hours from the project start. |
| HourFromStartHhh | `78` | Examples are H-2, H-1, H1, H2, H3 |
| HourFromStartHourHh | `38` | Examples are Hour -2, Hour -1, Hour 1, Hour 2, Hour 3 |
| MinuteHhMmAm | `33` | Examples are 8:00 AM, 8:01 AM, 8:02 AM. Requires the time unit to be TimescaleMinutes. |
| MinuteMm | `34` | Examples are 0, 1, 2, ..., 59 minutes |
| MinuteFromEndMinuteMm | `37` | Examples are Minute 181, Minute 180, ..., Minute 1, Minute -1 from the project end. |
| MinuteFromEndMm | `81` | Examples are 181, 180, ..., 1, -1 |
| MinuteFromEndMmm | `80` | Examples are M181, M180, ..., M1, M-1 |
| MinuteFromStartMinuteMm | `36` | Examples are Minute -2, Minute -1, Minute 1, ... Minute 180 from the project start. |
| MinuteFromStartMm | `83` | Examples are -2, -1, 1, ..., 180 |
| MinuteFromStartMmm | `82` | Examples are M-2, M-1, M1, ..., M180 |
| MonthM | `11` | Examples are M, A, M, J, J. Requires the time unit to be TimescaleMonths. |
| MonthMm | `57` | Examples are 11, 12, 1, 2 |
| MonthMmYy | `86` | Examples are 3/10, 4/10, 5/10 |
| MonthMmYyy | `85` | Examples are 3 '10, 4 '10, 5 '10 |
| MonthMmm | `10` | Examples are Mar, Apr, May |
| MonthMmmYyy | `8` | Examples are Mar '10, Apr '10, May '10 |
| MonthMmmm | `9` | Examples are March, April, May |
| MonthMmmmYyyy | `7` | Examples are March 2010, April 2010, May 2010 |
| MonthFromEndMm | `59` | Examples are 2, 1, -1, -2 months from the project end. |
| MonthFromEndMmm | `58` | Examples are M2, M1, M-1, M-2 |
| MonthFromEndMonthMm | `45` | Examples are Month 2, Month 1, Month -1, Month -2 |
| MonthFromStartMm | `61` | Examples are -2, -2, 1, 2 months from the project start. |
| MonthFromStartMmm | `60` | Examples are M-2, M-1, M1, M2 |
| MonthFromStartMonthMm | `44` | Examples are Month -2, Month -1, Month 1, Month 2 |
| QuarterQ | `62` | Examples are 3, 4, 1. Requires the time unit to be TimescaleQuarters. |
| QuarterQq | `6` | Examples are Q3, Q4, Q1 |
| QuarterQqYyy | `4` | Examples are Q3 '10, Q4 '10, Q1 '11 |
| QuarterQqqQuarter | `2` | Examples are 3rd Quarter, 1st Quarter |
| QuarterQQyy | `51` | Examples are 3Q10, 4Q10, 1Q11 |
| QuarterQtrQ | `5` | Examples are Qtr3, Qtr4, Qtr1 |
| QuarterQtrQYyyy | `3` | Examples are Qtr3, 2010; Qtr4, 2010; Qtr1, 2011 |
| QuarterFromEndQ | `64` | Examples are 5, 4, 3, 2, 1, -1 quarters from the project end. |
| QuarterFromEndQq | `63` | Examples are Q5, Q4, Q3, Q2, Q1, Q-1 |
| QuarterFromEndQuarterQ | `47` | Examples are Quarter 5, Quarter 4, Quarter 3, Quarter 2, Quarter 1, Quarter -1 |
| QuarterFromStartQ | `66` | Examples are -5, -4, -3, -2, -1, 1 quarters from the project start. |
| QuarterFromStartQq | `65` | Examples are Q-5, Q-4, Q-3, Q-2, Q-1, Q1 |
| QuarterFromStartQuarterQ | `46` | Examples are Quarter -5, Quarter -4, Quarter -3, Quarter -2, Quarter -1, Quarter 1 |
| ThirdsOfMonthsDd | `136` | Examples are 1, 11, 21, 1. Requires the time unit to be TimescaleThirdsOfMonths. |
| ThirdsOfMonthsDdd | `137` | Examples are B, M, E, B |
| ThirdsOfMonthsDddd | `138` | Examples are Beginning, Middle, End, Beginning |
| ThirdsOfMonthsMmDd | `139` | Example is 3/1. |
| ThirdsOfMonthsMmDdYy | `145` | Example is 3/1/10. |
| ThirdsOfMonthsMmDdd | `140` | Examples are 3/B, 3/M, 3/E, 4/B |
| ThirdsOfMonthsMmDddYy | `146` | Example is 3/B/10. |
| ThirdsOfMonthsMmmDd | `142` | Examples are Mar 1, Mar 11, Mar 21, Apr 1 |
| ThirdsOfMonthsMmmDdYy | `147` | Examples are Mar 1, '10; Mar 11, '10; Mar 21, '10; Apr 1, 10 |
| ThirdsOfMonthsMmmDdd | `143` | Examples are Mar B, Mar M, Mar E, Apr B |
| ThirdsOfMonthsMmmDddYy | `148` | Examples are Mar B, '10; Mar M, '10; Mar E, '10; Apr B '10 |
| ThirdsOfMonthsMmmmDd | `144` | Examples are March 1, March 11, March 21, April 1 |
| ThirdsOfMonthsMmmmDdYyyy | `149` | Examples are March 1, 2010; March 11, 2010; March 21, 2010; April 1, 2010 |
| ThirdsOfMonthsMmmmDddd | `141` | Examples are March Beginning, March Middle, March End, April Beginning |
| ThirdsOfMonthsMmmmDdddYyyy | `150` | Examples are March Beginning, 2010; March Middle, 2010; March End, 2010; April Beginning, 2010 |
| WeekDddDd | `88` | Examples are Sun 21, Sun 28, Sun 4. Requires the time unit to be TimescaleWeeks. |
| WeekDddMDd | `97` | Examples are Sun M 21, Sun M 28, Sun A 4 |
| WeekDddMmDd | `90` | Examples are Sun 3/21, Sun 3/28, Sun 4/4 |
| WeekDddMmDdYy | `100` | Examples are Sun 3/21/10, Sun 3/28/10, Sun 4/4/10 |
| WeekDddMmmDd | `93` | Examples are Sun Mar 21, Sun Mar 28, Sun Apr 4 |
| WeekDddMmmDdYyy | `101` | Examples are Sun Mar 21, '10; Sun Mar 28, '10; Sun Apr 4, '10 |
| WeekDddMmmmDd | `96` | Examples are Sun Mar 21, Sun March 28, Sun Apr 4 |
| WeekDddMmmmDdYyy | `102` | Examples are Sun March 21, '10; Sun March 28, '10; Sun April 4, '10 |
| WeekDddWw | `103` | Examples are Sun 12, Sun 13, Sun 14 |
| WeekDdiMDd | `98` | Examples are Su M 21, Su M 28, Su A 4 |
| WeekDdiMmDd | `91` | Examples are Su 3/21. Su 3/28, Su 4/4 |
| WeekDdiMmmDd | `94` | Examples are Su Mar 21, Su Mar 28, Su Apr 4 |
| WeekDiMDd | `99` | Examples are S M 21, S M 28, S A 4 |
| WeekDiMmDd | `92` | Examples are S 3/21, S 3/28, S 4/4 |
| WeekDiMmmDd | `95` | Examples are S Mar 21, S Mar 28, S Apr 4 |
| WeekMDd | `89` | Examples are M21, M28, A 4 |
| WeekMmDd | `17` | Examples are 3/21, 3/28, 4/4 |
| WeekMmDdYy | `16` | Example is '3/21/10'. |
| WeekMmmDd | `15` | Examples are Mar 21, Mar 28, Apr 4 |
| WeekMmmDdYyy | `13` | Examples are Mar 21, '10; Mar 28, '10; Apr 4, '10 |
| WeekMmmmDd | `14` | Examples are March 21, March 28, April 4 |
| WeekMmmmDdYyyy | `12` | Examples are March 21, 2010; March 28, 2010; April 4, 2010 |
| WeekDayOfMonthDd | `87` | Examples are 21, 28, 4 |
| WeekFromEndWeekWw | `43` | Examples are Week 2, Week 1, Week -1 from the project end. |
| WeekFromEndWw | `68` | Examples are 2, 1, -1 |
| WeekFromEndWww | `67` | Examples are W2, W1, W-1 |
| WeekFromStartWeekWw | `42` | Examples are Week -1, Week 1, Week 2 from the project start. |
| WeekFromStartWw | `70` | Examples are -1, 1, 2 |
| WeekFromStartWww | `69` | Examples are W-1, W1, W2 |
| WeekNumberDdWw | `104` | Examples are 1 12, 1 13, 1 14 (day 1 of week 12, day 1 of week 13, and so forth) |
| WeekNumberWw | `50` | Examples are 12, 13, 14 |
| YearYy | `75` | Examples are 10, 11, 12. Requires the time unit to be TimescaleYears. |
| YearYyy | `1` | Examples are '10, '11, '12 |
| YearYyyy | `0` | Examples are 2010, 2011, 2012 |
| YearFromEndYearYy | `49` | Examples are Year 2, Year 1, Year -1 from the project end. |
| YearFromEndYy | `72` | Examples are 2, 1, -1 |
| YearFromEndYyy | `71` | Examples are Y2, Y1, Y-1 |
| YearFromStartYearYy | `48` | Examples are Year -1, Year 1, Year 2 from the project start. |
| YearFromStartYy | `74` | Examples are -1, 1, 2 |
| YearFromStartYyy | `73` | Examples are Y-1, Y1, Y2 |

## Examples

Shows how to customize timescale tier labels.

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");

// Add task links
project.TaskLinks.Add(project.RootTask.Children.Add("Task 1"), project.RootTask.Children.Add("Task 2"));

var view = (GanttChartView)project.DefaultView;

// tune timescale tiers

// tune the top tier
// set the top timescale tier of the Gantt Chart view.
view.MiddleTimescaleTier = new TimescaleTier();
// set timescale unit <see cref="T:Aspose.Tasks.Visualization.TimescaleUnit" /> for the timescale tier.
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
// set the time unit interval in which to show labels for the tier.
view.MiddleTimescaleTier.Count = 1;
// set date label <see cref="T:Aspose.Tasks.Visualization.DateLabel" /> for the timescale tier.
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
// set how to align labels within each time period of the tier (<see cref="T:System.Drawing.StringAlignment" />).
view.MiddleTimescaleTier.Alignment = HorizontalStringAlignment.Center;
// set a value indicating whether whether to show tick marks that separate time periods in the tier.
view.MiddleTimescaleTier.ShowTicks = true;
// set a value indicating whether to base the tier labels on the fiscal year.
view.MiddleTimescaleTier.UsesFiscalYear = true;

// added for better visualization
view.TopTimescaleTier = new TimescaleTier(TimescaleUnit.Months, 1);

// customize middle tier dates
view.TopTimescaleTier.DateTimeConverter = date =>
    new[] { "Янв.", "Фев.", "Мар.", "Апр.", "Май", "Июнь", "Июль", "Авг.", "Сен.", "Окт.", "Ноя.", "Дек." }[date.Month - 1];

project.Set(Prj.TimescaleStart, new DateTime(2012, 7, 30));
project.Set(Prj.TimescaleFinish, new DateTime(2012, 10, 6));

// Use 'Timescale.DefinedInView' option to render timescales using timescale settings defined in view (view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier). 
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "CustomizeTimescaleTierLabels_out.pdf", pdfSaveOptions);
```

### See Also

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


