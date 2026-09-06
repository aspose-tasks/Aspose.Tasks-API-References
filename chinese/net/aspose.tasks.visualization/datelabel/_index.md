---
title: "枚举 DateLabel"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Visualization.DateLabel 枚举。指定时间刻度中日期和时间标签的显示格式"
type: docs
weight: 2980
url: /zh/net/aspose.tasks.visualization/datelabel/
---
## DateLabel enumeration

指定时间尺度中日期和时间标签的显示格式。

```csharp
public enum DateLabel
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| None | `35` | 未显示日期。 |
| DayDdd | `19` | 示例为 Mon, Tue. |
| DayDddDd | `105` | 示例为 Mon 30, Tue 1 |
| DayDddMDd | `112` | 示例为 Mon S 30, Tue O 1 |
| DayDddMmDd | `108` | 示例为 Mon 9/30, Tue 10/1 |
| DayDddMmDdYy | `52` | 示例为 Mon 9/30/02, Tue 10/1/02 |
| DayDddMmmDd | `23` | 示例为 Mon Sep 30, Tue Oct 1 |
| DayDddMmmDdYyy | `22` | 示例为 Mon Sep 30 '02, Tue Oct 1 '02 |
| DayDddMmmmDd | `111` | 示例为 Mon September 30, Tue October 1 |
| DayDddd | `18` | 示例为 Tuesday, Wednesday. |
| DayDdi | `119` | 示例为 Mo, Tu |
| DayDdiDd | `106` | 示例为 Mo 30, Tu 1 |
| DayDdiMDd | `113` | 示例为 Mo S 30, Tu O 1 |
| DayDdiMmDd | `109` | 示例为 Mo 9/30, Tu 10/1 |
| DayDi | `20` | 示例为 M, T |
| DayDiDdSpace | `107` | 示例为 M 30, T 1 |
| DayDiMDd | `114` | 示例为 M S 30, T O 1 |
| DayDiMmDd | `110` | 示例为 M 9/30, T 10/1 |
| DayDiDdNoSpace | `121` | 示例为 M30, T1 |
| DayMDd | `115` | 示例为 S 30, O 1 |
| DayMmDd | `27` | 示例为 9/30, 10/1 |
| DayMmDdYy | `26` | 示例为 9/30/02, 10/1/02 |
| DayMmmDd | `25` | 示例为 Sep 30, Oct 1 |
| DayMmmDdYyy | `24` | 示例为 Sep 30 '02, Oct 10 '02 |
| DayFromEndDayDd | `41` | 示例为项目结束时的 Day 2、Day 1、Day -1、Day -2。 |
| DayFromEndDd | `54` | 示例为 2、1、-1、-2 |
| DayFromEndDdd | `53` | 示例为 D2、D1、D-1、D-2 |
| DayFromStartDayDd | `40` | 示例为项目开始时的 Day -2、Day -1、Day 1、Day 2。 |
| DayFromStartDd | `56` | 示例为 -2、-1、1、2 |
| DayFromStartDdd | `55` | 示例为 D-2、D-1、D1、D2 |
| DayOfMonthDd | `21` | 示例为 30、1 |
| DayOfYearDd | `118` | 示例为 77、78 |
| DayOfYearDdYyy | `116` | 示例为 77 '10、78 '10 |
| DayOfYearDdYyyy | `117` | 示例为 77 2010、78 2010 |
| DayDdMmYyyy | `256` | 示例为 19/07/2016。 |
| HalfYearH | `128` | 示例为 1、2。需要将时间单位设置为 TimescaleHalfYears。 |
| HalfYearHh | `127` | 示例为 H1、H2 |
| HalfYearHhYyy | `126` | 示例为 H1 '10、H2 '10 |
| HalfYearHhhHalf | `123` | 示例为 1st Half、2d Half |
| HalfYearHHyy | `129` | 示例为 1H10、2H10 |
| HalfYearHlfH | `125` | 示例为 Half 1、Half 2 |
| HalfYearHlfHYyyy | `124` | 示例为 Half 1、2010; Half 2、2010 |
| HalfYearFromEndH | `135` | 示例为 2、1、-1、-2。半年从项目结束日期起。 |
| HalfYearFromEndHalfH | `133` | 示例为 Half 2、Half 1、Half -1、Half -2 |
| HalfYearFromEndHh | `134` | 示例为 H2、H1、H-1、H-2 |
| HalfYearFromStartH | `132` | 示例为 -2、-1、1、2。半年从项目开始日期起。 |
| HalfYearFromStartHalfH | `130` | 示例为 Half -2、Half -1、Half 1、Half 2 |
| HalfYearFromStartHh | `131` | 示例为 H-2, H-1, H1, H2 |
| HourDddMmmDdHhAm | `28` | 示例为 Wed Mar 18, 8 AM; Wed Mar 18, 9 AM. 需要时间单位为 TimescaleHours. |
| HourHh | `32` | 示例为 8, 9, 10, 11 |
| HourHhMmAm | `30` | 示例为 8:00 AM, 9:00 AM |
| HourHhAm | `31` | 示例为 8AM, 9AM |
| HourMmDdHhAm | `120` | 示例为 3/18 8 AM, 3/18 9 AM |
| HourMmmDdHhAm | `29` | 示例为 Mar 18, 8 AM; Mar 18, 9 AM |
| HourFromEndHh | `77` | 示例为 3, 2, 1, -1, -2 小时从项目结束算起. |
| HourFromEndHhh | `76` | 示例为 H3, H2, H1, H-1, H-2 |
| HourFromEndHourHh | `39` | 示例为 小时 3, 小时 2, 小时 1, 小时 -1, 小时 -2 |
| HourFromStartHh | `79` | 示例为 -2, -1, 1, 2, 3 小时从项目开始算起. |
| HourFromStartHhh | `78` | 示例为 H-2, H-1, H1, H2, H3 |
| HourFromStartHourHh | `38` | 示例为 小时 -2, 小时 -1, 小时 1, 小时 2, 小时 3 |
| MinuteHhMmAm | `33` | 示例为 8:00 AM, 8:01 AM, 8:02 AM. 需要时间单位为 TimescaleMinutes. |
| MinuteMm | `34` | 示例为 0, 1, 2, ..., 59 分钟 |
| MinuteFromEndMinuteMm | `37` | 示例为 分钟 181, 分钟 180, ..., 分钟 1, 分钟 -1 从项目结束算起. |
| MinuteFromEndMm | `81` | 示例为 181, 180, ..., 1, -1 |
| MinuteFromEndMmm | `80` | 示例为 M181, M180, ..., M1, M-1 |
| MinuteFromStartMinuteMm | `36` | 示例为 分钟 -2, 分钟 -1, 分钟 1, ... 分钟 180 从项目开始算起. |
| MinuteFromStartMm | `83` | 示例为 -2, -1, 1, ..., 180 |
| MinuteFromStartMmm | `82` | 示例为 M-2, M-1, M1, ..., M180 |
| MonthM | `11` | 示例为 M, A, M, J, J. 需要时间单位为 TimescaleMonths. |
| MonthMm | `57` | 示例为 11, 12, 1, 2 |
| MonthMmYy | `86` | 示例为 3/10, 4/10, 5/10 |
| MonthMmYyy | `85` | 示例为 3 '10, 4 '10, 5 '10 |
| MonthMmm | `10` | 示例为 Mar, Apr, May |
| MonthMmmYyy | `8` | 示例为 Mar '10, Apr '10, May '10 |
| MonthMmmm | `9` | 示例为 March, April, May |
| MonthMmmmYyyy | `7` | 示例为 March 2010, April 2010, May 2010 |
| MonthFromEndMm | `59` | 示例为 项目结束后 2, 1, -1, -2 个月. |
| MonthFromEndMmm | `58` | 示例为 M2, M1, M-1, M-2 |
| MonthFromEndMonthMm | `45` | 示例为 Month 2, Month 1, Month -1, Month -2 |
| MonthFromStartMm | `61` | 示例为 项目开始后 -2, -2, 1, 2 个月. |
| MonthFromStartMmm | `60` | 示例为 M-2, M-1, M1, M2 |
| MonthFromStartMonthMm | `44` | 示例为 Month -2, Month -1, Month 1, Month 2 |
| QuarterQ | `62` | 示例为 3, 4, 1. 要求时间单位为 TimescaleQuarters. |
| QuarterQq | `6` | 示例为 Q3, Q4, Q1 |
| QuarterQqYyy | `4` | 示例为 Q3 '10, Q4 '10, Q1 '11 |
| QuarterQqqQuarter | `2` | 示例为 3rd Quarter, 1st Quarter |
| QuarterQQyy | `51` | 示例为 3Q10, 4Q10, 1Q11 |
| QuarterQtrQ | `5` | 示例为 Qtr3, Qtr4, Qtr1 |
| QuarterQtrQYyyy | `3` | 示例为 Qtr3, 2010; Qtr4, 2010; Qtr1, 2011 |
| QuarterFromEndQ | `64` | 示例为 项目结束后 5, 4, 3, 2, 1, -1 季度. |
| QuarterFromEndQq | `63` | 示例为 Q5, Q4, Q3, Q2, Q1, Q-1 |
| QuarterFromEndQuarterQ | `47` | 示例为 Quarter 5, Quarter 4, Quarter 3, Quarter 2, Quarter 1, Quarter -1 |
| QuarterFromStartQ | `66` | 示例为 项目开始后 -5, -4, -3, -2, -1, 1 季度. |
| QuarterFromStartQq | `65` | 示例为 Q-5, Q-4, Q-3, Q-2, Q-1, Q1 |
| QuarterFromStartQuarterQ | `46` | 示例为 Quarter -5, Quarter -4, Quarter -3, Quarter -2, Quarter -1, Quarter 1 |
| ThirdsOfMonthsDd | `136` | 示例为 1, 11, 21, 1. 要求时间单位为 TimescaleThirdsOfMonths. |
| ThirdsOfMonthsDdd | `137` | 示例为 B, M, E, B |
| ThirdsOfMonthsDddd | `138` | 示例为 开始, 中间, 结束, 开始 |
| ThirdsOfMonthsMmDd | `139` | 示例为 3/1. |
| ThirdsOfMonthsMmDdYy | `145` | 示例为 3/1/10. |
| ThirdsOfMonthsMmDdd | `140` | 示例为 3/B, 3/M, 3/E, 4/B |
| ThirdsOfMonthsMmDddYy | `146` | 示例为 3/B/10. |
| ThirdsOfMonthsMmmDd | `142` | 示例为 3月 1日, 3月 11日, 3月 21日, 4月 1日 |
| ThirdsOfMonthsMmmDdYy | `147` | 示例为 3月 1日, '10; 3月 11日, '10; 3月 21日, '10; 4月 1日, 10 |
| ThirdsOfMonthsMmmDdd | `143` | 示例为 3月 B, 3月 M, 3月 E, 4月 B |
| ThirdsOfMonthsMmmDddYy | `148` | 示例为 3月 B, '10; 3月 M, '10; 3月 E, '10; 4月 B '10 |
| ThirdsOfMonthsMmmmDd | `144` | 示例为 3月 1日, 3月 11日, 3月 21日, 4月 1日 |
| ThirdsOfMonthsMmmmDdYyyy | `149` | 示例为 3月 1日, 2010; 3月 11日, 2010; 3月 21日, 2010; 4月 1日, 2010 |
| ThirdsOfMonthsMmmmDddd | `141` | 示例为 3月 开始, 3月 中间, 3月 结束, 4月 开始 |
| ThirdsOfMonthsMmmmDdddYyyy | `150` | 示例为 3月 开始, 2010; 3月 中间, 2010; 3月 结束, 2010; 4月 开始, 2010 |
| WeekDddDd | `88` | 示例为 Sun 21, Sun 28, Sun 4. 要求时间单位为 TimescaleWeeks. |
| WeekDddMDd | `97` | 示例为 Sun M 21, Sun M 28, Sun A 4 |
| WeekDddMmDd | `90` | 示例为 Sun 3/21, Sun 3/28, Sun 4/4 |
| WeekDddMmDdYy | `100` | 示例为 Sun 3/21/10, Sun 3/28/10, Sun 4/4/10 |
| WeekDddMmmDd | `93` | 示例为 Sun 3月 21日, Sun 3月 28日, Sun 4月 4日 |
| WeekDddMmmDdYyy | `101` | 示例为 Sun 3月 21日, '10; Sun 3月 28日, '10; Sun 4月 4日, '10 |
| WeekDddMmmmDd | `96` | 示例为 Sun 3月 21日, Sun 3月 28日, Sun 4月 4日 |
| WeekDddMmmmDdYyy | `102` | 示例为 Sun 3月 21日, '10; Sun 3月 28日, '10; Sun 4月 4日, '10 |
| WeekDddWw | `103` | 示例为 Sun 12, Sun 13, Sun 14 |
| WeekDdiMDd | `98` | 示例为 Su M 21, Su M 28, Su A 4 |
| WeekDdiMmDd | `91` | 示例为 Su 3/21. Su 3/28, Su 4/4 |
| WeekDdiMmmDd | `94` | 示例为 Su 3月 21日, Su 3月 28日, Su 4月 4日 |
| WeekDiMDd | `99` | 示例为 S M 21, S M 28, S A 4 |
| WeekDiMmDd | `92` | 示例为 S 3/21, S 3/28, S 4/4 |
| WeekDiMmmDd | `95` | 示例为 S Mar 21, S Mar 28, S Apr 4 |
| WeekMDd | `89` | 示例为 M21, M28, A 4 |
| WeekMmDd | `17` | 示例为 3/21, 3/28, 4/4 |
| WeekMmDdYy | `16` | 示例为 '3/21/10'。 |
| WeekMmmDd | `15` | 示例为 Mar 21, Mar 28, Apr 4 |
| WeekMmmDdYyy | `13` | 示例为 Mar 21, '10; Mar 28, '10; Apr 4, '10 |
| WeekMmmmDd | `14` | 示例为 March 21, March 28, April 4 |
| WeekMmmmDdYyyy | `12` | 示例为 March 21, 2010; March 28, 2010; April 4, 2010 |
| WeekDayOfMonthDd | `87` | 示例为 21, 28, 4 |
| WeekFromEndWeekWw | `43` | 示例为 Week 2, Week 1, Week -1 来自项目结束。 |
| WeekFromEndWw | `68` | 示例为 2, 1, -1 |
| WeekFromEndWww | `67` | 示例为 W2, W1, W-1 |
| WeekFromStartWeekWw | `42` | 示例为 Week -1, Week 1, Week 2 来自项目开始。 |
| WeekFromStartWw | `70` | 示例为 -1, 1, 2 |
| WeekFromStartWww | `69` | 示例为 W-1, W1, W2 |
| WeekNumberDdWw | `104` | 示例为 1 12, 1 13, 1 14（第 12 周的第 1 天，第 13 周的第 1 天，依此类推） |
| WeekNumberWw | `50` | 示例为 12, 13, 14 |
| YearYy | `75` | 示例为 10, 11, 12。需要将时间单位设为 TimescaleYears。 |
| YearYyy | `1` | 示例为 '10, '11, '12 |
| YearYyyy | `0` | 示例为 2010, 2011, 2012 |
| YearFromEndYearYy | `49` | 示例为 Year 2, Year 1, Year -1 来自项目结束。 |
| YearFromEndYy | `72` | 示例为 2, 1, -1 |
| YearFromEndYyy | `71` | 示例为 Y2, Y1, Y-1 |
| YearFromStartYearYy | `48` | 示例为 Year -1, Year 1, Year 2 来自项目开始。 |
| YearFromStartYy | `74` | 示例为 -1, 1, 2 |
| YearFromStartYyy | `73` | 示例包括 Y-1、Y1、Y2 |

## 示例

展示如何自定义时间尺度层级标签。

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");

// 添加任务链接
project.TaskLinks.Add(project.RootTask.Children.Add("Task 1"), project.RootTask.Children.Add("Task 2"));

var view = (GanttChartView)project.DefaultView;

// 调优时间尺度层级

// 调优顶部层级
// 设置甘特图视图的顶部时间尺度层级。
view.MiddleTimescaleTier = new TimescaleTier();
// 为时间尺度层级设置时间尺度单位 <see cref="T:Aspose.Tasks.Visualization.TimescaleUnit" />。
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
// 设置在层级中显示标签的时间单位间隔。
view.MiddleTimescaleTier.Count = 1;
// 为时间尺度层级设置日期标签 <see cref="T:Aspose.Tasks.Visualization.DateLabel" />。
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
// 设置在层级的每个时间段内对齐标签的方式 (<see cref="T:System.Drawing.StringAlignment" />)。
view.MiddleTimescaleTier.Alignment = HorizontalStringAlignment.Center;
// 设置一个值，指示是否在层级中显示分隔时间段的刻度线。
view.MiddleTimescaleTier.ShowTicks = true;
// 设置一个值，指示是否基于财政年度来确定层级标签。
view.MiddleTimescaleTier.UsesFiscalYear = true;

// 为获得更好的可视化而添加。
view.TopTimescaleTier = new TimescaleTier(TimescaleUnit.Months, 1);

// 自定义中间层级的日期
view.TopTimescaleTier.DateTimeConverter = date =>
    new[] { "Янв.", "Фев.", "Мар.", "Апр.", "Май", "Июнь", "Июль", "Авг.", "Сен.", "Окт.", "Ноя.", "Дек." }[date.Month - 1];

project.Set(Prj.TimescaleStart, new DateTime(2012, 7, 30));
project.Set(Prj.TimescaleFinish, new DateTime(2012, 10, 6));

// 使用 'Timescale.DefinedInView' 选项，根据视图中定义的时间尺度设置（view.TopTimescaleTier、view.MiddleTimescaleTier、view.BottomTimescaleTier）渲染时间尺度。
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "CustomizeTimescaleTierLabels_out.pdf", pdfSaveOptions);
```

### 另见

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


