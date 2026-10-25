---
title: "Перечисление DateLabel"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.Visualization.DateLabel. Указывает формат отображения меток даты и времени в шкале времени"
type: docs
weight: 2980
url: /ru/net/aspose.tasks.visualization/datelabel/
---
## DateLabel enumeration

Указывает формат отображения меток даты и времени на шкале времени.

```csharp
public enum DateLabel
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `35` | Дата не отображается. |
| DayDdd | `19` | Примеры: Mon, Tue. |
| DayDddDd | `105` | Примеры: Mon 30, Tue 1 |
| DayDddMDd | `112` | Примеры: Mon S 30, Tue O 1 |
| DayDddMmDd | `108` | Примеры: Mon 9/30, Tue 10/1 |
| DayDddMmDdYy | `52` | Примеры: Mon 9/30/02, Tue 10/1/02 |
| DayDddMmmDd | `23` | Примеры: Mon Sep 30, Tue Oct 1 |
| DayDddMmmDdYyy | `22` | Примеры: Mon Sep 30 '02, Tue Oct 1 '02 |
| DayDddMmmmDd | `111` | Примеры: Mon September 30, Tue October 1 |
| DayDddd | `18` | Примеры: Tuesday, Wednesday. |
| DayDdi | `119` | Примеры: Mo, Tu |
| DayDdiDd | `106` | Примеры: Mo 30, Tu 1 |
| DayDdiMDd | `113` | Примеры: Mo S 30, Tu O 1 |
| DayDdiMmDd | `109` | Примеры: Mo 9/30, Tu 10/1 |
| DayDi | `20` | Примеры: M, T |
| DayDiDdSpace | `107` | Примеры: M 30, T 1 |
| DayDiMDd | `114` | Примеры: M S 30, T O 1 |
| DayDiMmDd | `110` | Примеры: M 9/30, T 10/1 |
| DayDiDdNoSpace | `121` | Примеры: M30, T1 |
| DayMDd | `115` | Примеры: S 30, O 1 |
| DayMmDd | `27` | Примеры: 9/30, 10/1 |
| DayMmDdYy | `26` | Примеры: 9/30/02, 10/1/02 |
| DayMmmDd | `25` | Примеры: Sep 30, Oct 1 |
| DayMmmDdYyy | `24` | Примеры: Sep 30 '02, Oct 10 '02 |
| DayFromEndDayDd | `41` | Примеры: Day 2, Day 1, Day -1, Day -2 от конца проекта. |
| DayFromEndDd | `54` | Примеры: 2, 1, -1, -2 |
| DayFromEndDdd | `53` | Примеры: D2, D1, D-1, D-2 |
| DayFromStartDayDd | `40` | Примеры: Day -2, Day -1, Day 1, Day 2 от начала проекта. |
| DayFromStartDd | `56` | Примеры: -2, -1, 1, 2 |
| DayFromStartDdd | `55` | Примеры: D-2, D-1, D1, D2 |
| DayOfMonthDd | `21` | Примеры: 30, 1 |
| DayOfYearDd | `118` | Примеры: 77, 78 |
| DayOfYearDdYyy | `116` | Примеры: 77 '10, 78 '10 |
| DayOfYearDdYyyy | `117` | Примеры: 77 2010, 78 2010 |
| DayDdMmYyyy | `256` | Пример: 19/07/2016. |
| HalfYearH | `128` | Примеры: 1, 2. Требуется, чтобы единица времени была TimescaleHalfYears. |
| HalfYearHh | `127` | Примеры: H1, H2 |
| HalfYearHhYyy | `126` | Примеры: H1 '10, H2 '10 |
| HalfYearHhhHalf | `123` | Примеры: 1st Half, 2d Half |
| HalfYearHHyy | `129` | Примеры: 1H10, 2H10 |
| HalfYearHlfH | `125` | Примеры: Half 1, Half 2 |
| HalfYearHlfHYyyy | `124` | Примеры: Half 1, 2010; Half 2, 2010 |
| HalfYearFromEndH | `135` | Примеры: 2, 1, -1, -2. Полугода от даты окончания проекта. |
| HalfYearFromEndHalfH | `133` | Примеры: Half 2, Half 1, Half -1, Half -2 |
| HalfYearFromEndHh | `134` | Примеры: H2, H1, H-1, H-2 |
| HalfYearFromStartH | `132` | Примеры: -2, -1, 1, 2. Полугода от даты начала проекта. |
| HalfYearFromStartHalfH | `130` | Примеры: Half -2, Half -1, Half 1, Half 2 |
| HalfYearFromStartHh | `131` | Примеры: H-2, H-1, H1, H2 |
| HourDddMmmDdHhAm | `28` | Примеры: Wed Mar 18, 8 AM; Wed Mar 18, 9 AM. Требуется, чтобы единица времени была TimescaleHours. |
| HourHh | `32` | Примеры: 8, 9, 10, 11 |
| HourHhMmAm | `30` | Примеры: 8:00 AM, 9:00 AM |
| HourHhAm | `31` | Примеры: 8AM, 9AM |
| HourMmDdHhAm | `120` | Примеры: 3/18 8 AM, 3/18 9 AM |
| HourMmmDdHhAm | `29` | Примеры: Mar 18, 8 AM; Mar 18, 9 AM |
| HourFromEndHh | `77` | Примеры: 3, 2, 1, -1, -2 часа от конца проекта. |
| HourFromEndHhh | `76` | Примеры: H3, H2, H1, H-1, H-2 |
| HourFromEndHourHh | `39` | Примеры: Hour 3, Hour 2, Hour 1, Hour -1, Hour -2 |
| HourFromStartHh | `79` | Примеры: -2, -1, 1, 2, 3 часа от начала проекта. |
| HourFromStartHhh | `78` | Примеры: H-2, H-1, H1, H2, H3 |
| HourFromStartHourHh | `38` | Примеры: Hour -2, Hour -1, Hour 1, Hour 2, Hour 3 |
| MinuteHhMmAm | `33` | Примеры: 8:00 AM, 8:01 AM, 8:02 AM. Требуется, чтобы единица времени была TimescaleMinutes. |
| MinuteMm | `34` | Примеры: 0, 1, 2, ..., 59 минут |
| MinuteFromEndMinuteMm | `37` | Примеры: Minute 181, Minute 180, ..., Minute 1, Minute -1 от конца проекта. |
| MinuteFromEndMm | `81` | Примеры: 181, 180, ..., 1, -1 |
| MinuteFromEndMmm | `80` | Примеры: M181, M180, ..., M1, M-1 |
| MinuteFromStartMinuteMm | `36` | Примеры: Minute -2, Minute -1, Minute 1, ... Minute 180 от начала проекта. |
| MinuteFromStartMm | `83` | Примеры: -2, -1, 1, ..., 180 |
| MinuteFromStartMmm | `82` | Примеры: M-2, M-1, M1, ..., M180 |
| MonthM | `11` | Примеры: M, A, M, J, J. Требуется, чтобы единица времени была TimescaleMonths. |
| MonthMm | `57` | Примеры: 11, 12, 1, 2 |
| MonthMmYy | `86` | Примеры: 3/10, 4/10, 5/10 |
| MonthMmYyy | `85` | Примеры: 3 '10, 4 '10, 5 '10 |
| MonthMmm | `10` | Примеры: Mar, Apr, May |
| MonthMmmYyy | `8` | Примеры: Mar '10, Apr '10, May '10 |
| MonthMmmm | `9` | Примеры: March, April, May |
| MonthMmmmYyyy | `7` | Примеры: March 2010, April 2010, May 2010 |
| MonthFromEndMm | `59` | Примеры: 2, 1, -1, -2 месяца от конца проекта. |
| MonthFromEndMmm | `58` | Примеры: M2, M1, M-1, M-2 |
| MonthFromEndMonthMm | `45` | Примеры: Month 2, Month 1, Month -1, Month -2 |
| MonthFromStartMm | `61` | Примеры: -2, -2, 1, 2 месяца от начала проекта. |
| MonthFromStartMmm | `60` | Примеры: M-2, M-1, M1, M2 |
| MonthFromStartMonthMm | `44` | Примеры: Month -2, Month -1, Month 1, Month 2 |
| QuarterQ | `62` | Примеры: 3, 4, 1. Требуется, чтобы единица времени была TimescaleQuarters. |
| QuarterQq | `6` | Примеры: Q3, Q4, Q1 |
| QuarterQqYyy | `4` | Примеры: Q3 '10, Q4 '10, Q1 '11 |
| QuarterQqqQuarter | `2` | Примеры: 3-й квартал, 1-й квартал |
| QuarterQQyy | `51` | Примеры: 3Q10, 4Q10, 1Q11 |
| QuarterQtrQ | `5` | Примеры: Qtr3, Qtr4, Qtr1 |
| QuarterQtrQYyyy | `3` | Примеры: Qtr3, 2010; Qtr4, 2010; Qtr1, 2011 |
| QuarterFromEndQ | `64` | Примеры: 5, 4, 3, 2, 1, -1 кварталов от конца проекта. |
| QuarterFromEndQq | `63` | Примеры: Q5, Q4, Q3, Q2, Q1, Q-1 |
| QuarterFromEndQuarterQ | `47` | Примеры: Quarter 5, Quarter 4, Quarter 3, Quarter 2, Quarter 1, Quarter -1 |
| QuarterFromStartQ | `66` | Примеры: -5, -4, -3, -2, -1, 1 кварталов от начала проекта. |
| QuarterFromStartQq | `65` | Примеры: Q-5, Q-4, Q-3, Q-2, Q-1, Q1 |
| QuarterFromStartQuarterQ | `46` | Примеры: Quarter -5, Quarter -4, Quarter -3, Quarter -2, Quarter -1, Quarter 1 |
| ThirdsOfMonthsDd | `136` | Примеры: 1, 11, 21, 1. Требуется, чтобы единица времени была TimescaleThirdsOfMonths. |
| ThirdsOfMonthsDdd | `137` | Примеры: B, M, E, B |
| ThirdsOfMonthsDddd | `138` | Примеры Начало, Середина, Конец, Начало |
| ThirdsOfMonthsMmDd | `139` | Пример 3/1. |
| ThirdsOfMonthsMmDdYy | `145` | Пример 3/1/10. |
| ThirdsOfMonthsMmDdd | `140` | Примеры 3/B, 3/M, 3/E, 4/B |
| ThirdsOfMonthsMmDddYy | `146` | Пример 3/B/10. |
| ThirdsOfMonthsMmmDd | `142` | Примеры Мар 1, Мар 11, Мар 21, Апр 1 |
| ThirdsOfMonthsMmmDdYy | `147` | Примеры Мар 1, '10; Мар 11, '10; Мар 21, '10; Апр 1, 10 |
| ThirdsOfMonthsMmmDdd | `143` | Примеры Мар B, Мар M, Мар E, Апр B |
| ThirdsOfMonthsMmmDddYy | `148` | Примеры Мар B, '10; Мар M, '10; Мар E, '10; Апр B '10 |
| ThirdsOfMonthsMmmmDd | `144` | Примеры Март 1, Март 11, Март 21, Апрель 1 |
| ThirdsOfMonthsMmmmDdYyyy | `149` | Примеры Март 1, 2010; Март 11, 2010; Март 21, 2010; Апрель 1, 2010 |
| ThirdsOfMonthsMmmmDddd | `141` | Примеры Март Начало, Март Середина, Март Конец, Апрель Начало |
| ThirdsOfMonthsMmmmDdddYyyy | `150` | Примеры Март Начало, 2010; Март Середина, 2010; Март Конец, 2010; Апрель Начало, 2010 |
| WeekDddDd | `88` | Примеры Sun 21, Sun 28, Sun 4. Требуется, чтобы единица времени была TimescaleWeeks. |
| WeekDddMDd | `97` | Примеры Sun M 21, Sun M 28, Sun A 4 |
| WeekDddMmDd | `90` | Примеры Sun 3/21, Sun 3/28, Sun 4/4 |
| WeekDddMmDdYy | `100` | Примеры Sun 3/21/10, Sun 3/28/10, Sun 4/4/10 |
| WeekDddMmmDd | `93` | Примеры Sun Мар 21, Sun Мар 28, Sun Апр 4 |
| WeekDddMmmDdYyy | `101` | Примеры Sun Мар 21, '10; Sun Мар 28, '10; Sun Апр 4, '10 |
| WeekDddMmmmDd | `96` | Примеры Sun Мар 21, Sun Март 28, Sun Апр 4 |
| WeekDddMmmmDdYyy | `102` | Примеры Sun Март 21, '10; Sun Март 28, '10; Sun Апрель 4, '10 |
| WeekDddWw | `103` | Примеры Sun 12, Sun 13, Sun 14 |
| WeekDdiMDd | `98` | Примеры Su M 21, Su M 28, Su A 4 |
| WeekDdiMmDd | `91` | Примеры Su 3/21. Su 3/28, Su 4/4 |
| WeekDdiMmmDd | `94` | Примеры Su Мар 21, Su Мар 28, Su Апр 4 |
| WeekDiMDd | `99` | Примеры: S M 21, S M 28, S A 4 |
| WeekDiMmDd | `92` | Примеры: S 3/21, S 3/28, S 4/4 |
| WeekDiMmmDd | `95` | Примеры: S Mar 21, S Mar 28, S Apr 4 |
| WeekMDd | `89` | Примеры: M21, M28, A 4 |
| WeekMmDd | `17` | Примеры: 3/21, 3/28, 4/4 |
| WeekMmDdYy | `16` | Пример: '3/21/10'. |
| WeekMmmDd | `15` | Примеры: Mar 21, Mar 28, Apr 4 |
| WeekMmmDdYyy | `13` | Примеры: Mar 21, '10; Mar 28, '10; Apr 4, '10 |
| WeekMmmmDd | `14` | Примеры: March 21, March 28, April 4 |
| WeekMmmmDdYyyy | `12` | Примеры: March 21, 2010; March 28, 2010; April 4, 2010 |
| WeekDayOfMonthDd | `87` | Примеры: 21, 28, 4 |
| WeekFromEndWeekWw | `43` | Примеры: Week 2, Week 1, Week -1 от конца проекта. |
| WeekFromEndWw | `68` | Примеры: 2, 1, -1 |
| WeekFromEndWww | `67` | Примеры: W2, W1, W-1 |
| WeekFromStartWeekWw | `42` | Примеры: Week -1, Week 1, Week 2 от начала проекта. |
| WeekFromStartWw | `70` | Примеры: -1, 1, 2 |
| WeekFromStartWww | `69` | Примеры: W-1, W1, W2 |
| WeekNumberDdWw | `104` | Примеры: 1 12, 1 13, 1 14 (день 1 недели 12, день 1 недели 13 и т.д.) |
| WeekNumberWw | `50` | Примеры: 12, 13, 14 |
| YearYy | `75` | Примеры: 10, 11, 12. Требуется, чтобы единица времени была TimescaleYears. |
| YearYyy | `1` | Примеры: '10, '11, '12 |
| YearYyyy | `0` | Примеры: 2010, 2011, 2012 |
| YearFromEndYearYy | `49` | Примеры: Year 2, Year 1, Year -1 от конца проекта. |
| YearFromEndYy | `72` | Примеры: 2, 1, -1 |
| YearFromEndYyy | `71` | Примеры: Y2, Y1, Y-1 |
| YearFromStartYearYy | `48` | Примеры: Year -1, Year 1, Year 2 от начала проекта. |
| YearFromStartYy | `74` | Примеры: -1, 1, 2 |
| YearFromStartYyy | `73` | Примеры: Y-1, Y1, Y2 |

## Примеры

Показывает, как настроить метки уровня шкалы времени.

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");

// Добавить ссылки на задачи
project.TaskLinks.Add(project.RootTask.Children.Add("Task 1"), project.RootTask.Children.Add("Task 2"));

var view = (GanttChartView)project.DefaultView;

// настроить уровни шкалы времени

// настроить верхний уровень
// установить верхний уровень шкалы времени представления диаграммы Ганта.
view.MiddleTimescaleTier = new TimescaleTier();
// установить единицу шкалы времени <see cref="T:Aspose.Tasks.Visualization.TimescaleUnit" /> для уровня шкалы времени.
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
// установить интервал единицы времени, в котором отображаются метки уровня.
view.MiddleTimescaleTier.Count = 1;
// установить метку даты <see cref="T:Aspose.Tasks.Visualization.DateLabel" /> для уровня шкалы времени.
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
// установить способ выравнивания меток внутри каждого временного периода уровня (<see cref="T:System.Drawing.StringAlignment" />).
view.MiddleTimescaleTier.Alignment = HorizontalStringAlignment.Center;
// установить значение, указывающее, следует ли показывать метки деления, разделяющие временные периоды в уровне.
view.MiddleTimescaleTier.ShowTicks = true;
// установить значение, указывающее, следует ли основывать подписи уровней на финансовом году.
view.MiddleTimescaleTier.UsesFiscalYear = true;

// добавлено для лучшей визуализации
view.TopTimescaleTier = new TimescaleTier(TimescaleUnit.Months, 1);

// настроить даты среднего уровня
view.TopTimescaleTier.DateTimeConverter = date =>
    new[] { "Янв.", "Фев.", "Мар.", "Апр.", "Май", "Июнь", "Июль", "Авг.", "Сен.", "Окт.", "Ноя.", "Дек." }[date.Month - 1];

project.Set(Prj.TimescaleStart, new DateTime(2012, 7, 30));
project.Set(Prj.TimescaleFinish, new DateTime(2012, 10, 6));

// Используйте параметр 'Timescale.DefinedInView' для отображения шкал времени с использованием настроек шкалы, определённых во view (view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier).
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "CustomizeTimescaleTierLabels_out.pdf", pdfSaveOptions);
```

### См. также

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


