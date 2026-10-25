---
title: "Enum DateLabel"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Visualization.DateLabel enum. 타임스케일에서 날짜 및 시간 레이블의 표시 형식을 지정합니다"
type: docs
weight: 2980
url: /ko/net/aspose.tasks.visualization/datelabel/
---
## DateLabel enumeration

시간 눈금표에서 날짜 및 시간 레이블의 표시 형식을 지정합니다.

```csharp
public enum DateLabel
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| None | `35` | 날짜가 표시되지 않습니다. |
| DayDdd | `19` | 예시: Mon, Tue. |
| DayDddDd | `105` | 예시: Mon 30, Tue 1 |
| DayDddMDd | `112` | 예시: Mon S 30, Tue O 1 |
| DayDddMmDd | `108` | 예시: Mon 9/30, Tue 10/1 |
| DayDddMmDdYy | `52` | 예시: Mon 9/30/02, Tue 10/1/02 |
| DayDddMmmDd | `23` | 예시: Mon Sep 30, Tue Oct 1 |
| DayDddMmmDdYyy | `22` | 예시: Mon Sep 30 '02, Tue Oct 1 '02 |
| DayDddMmmmDd | `111` | 예시: Mon September 30, Tue October 1 |
| DayDddd | `18` | 예시: Tuesday, Wednesday. |
| DayDdi | `119` | 예시: Mo, Tu |
| DayDdiDd | `106` | 예시: Mo 30, Tu 1 |
| DayDdiMDd | `113` | 예시: Mo S 30, Tu O 1 |
| DayDdiMmDd | `109` | 예시: Mo 9/30, Tu 10/1 |
| DayDi | `20` | 예시: M, T |
| DayDiDdSpace | `107` | 예시: M 30, T 1 |
| DayDiMDd | `114` | 예시: M S 30, T O 1 |
| DayDiMmDd | `110` | 예시: M 9/30, T 10/1 |
| DayDiDdNoSpace | `121` | 예시: M30, T1 |
| DayMDd | `115` | 예시: S 30, O 1 |
| DayMmDd | `27` | 예시: 9/30, 10/1 |
| DayMmDdYy | `26` | 예시: 9/30/02, 10/1/02 |
| DayMmmDd | `25` | 예시는 Sep 30, Oct 1입니다 |
| DayMmmDdYyy | `24` | 예시는 Sep 30 '02, Oct 10 '02입니다 |
| DayFromEndDayDd | `41` | 예시는 프로젝트 종료 기준 Day 2, Day 1, Day -1, Day -2입니다. |
| DayFromEndDd | `54` | 예시는 2, 1, -1, -2입니다 |
| DayFromEndDdd | `53` | 예시는 D2, D1, D-1, D-2입니다 |
| DayFromStartDayDd | `40` | 예시는 프로젝트 시작 기준 Day -2, Day -1, Day 1, Day 2입니다. |
| DayFromStartDd | `56` | 예시는 -2, -1, 1, 2입니다 |
| DayFromStartDdd | `55` | 예시는 D-2, D-1, D1, D2입니다 |
| DayOfMonthDd | `21` | 예시는 30, 1입니다 |
| DayOfYearDd | `118` | 예시는 77, 78입니다 |
| DayOfYearDdYyy | `116` | 예시는 77 '10, 78 '10입니다 |
| DayOfYearDdYyyy | `117` | 예시는 77 2010, 78 2010입니다 |
| DayDdMmYyyy | `256` | 예시는 19/07/2016입니다. |
| HalfYearH | `128` | 예시는 1, 2입니다. 시간 단위는 TimescaleHalfYears여야 합니다. |
| HalfYearHh | `127` | 예시는 H1, H2입니다 |
| HalfYearHhYyy | `126` | 예시는 H1 '10, H2 '10입니다 |
| HalfYearHhhHalf | `123` | 예시는 1st Half, 2d Half입니다 |
| HalfYearHHyy | `129` | 예시는 1H10, 2H10입니다 |
| HalfYearHlfH | `125` | 예시는 Half 1, Half 2입니다 |
| HalfYearHlfHYyyy | `124` | 예시는 Half 1, 2010; Half 2, 2010입니다 |
| HalfYearFromEndH | `135` | 예시는 2, 1, -1, -2입니다. 프로젝트 종료 날짜 기준 반년 단위입니다. |
| HalfYearFromEndHalfH | `133` | 예시는 Half 2, Half 1, Half -1, Half -2입니다 |
| HalfYearFromEndHh | `134` | 예시는 H2, H1, H-1, H-2입니다 |
| HalfYearFromStartH | `132` | 예시는 -2, -1, 1, 2입니다. 프로젝트 시작 날짜 기준 반년 단위입니다. |
| HalfYearFromStartHalfH | `130` | 예시는 Half -2, Half -1, Half 1, Half 2입니다 |
| HalfYearFromStartHh | `131` | 예시: H-2, H-1, H1, H2 |
| HourDddMmmDdHhAm | `28` | 예시: Wed Mar 18, 8 AM; Wed Mar 18, 9 AM. 시간 단위는 TimescaleHours이어야 합니다. |
| HourHh | `32` | 예시: 8, 9, 10, 11 |
| HourHhMmAm | `30` | 예시: 8:00 AM, 9:00 AM |
| HourHhAm | `31` | 예시: 8AM, 9AM |
| HourMmDdHhAm | `120` | 예시: 3/18 8 AM, 3/18 9 AM |
| HourMmmDdHhAm | `29` | 예시: Mar 18, 8 AM; Mar 18, 9 AM |
| HourFromEndHh | `77` | 예시: 프로젝트 종료 시점으로부터 3, 2, 1, -1, -2시간. |
| HourFromEndHhh | `76` | 예시: H3, H2, H1, H-1, H-2 |
| HourFromEndHourHh | `39` | 예시: 시간 3, 시간 2, 시간 1, 시간 -1, 시간 -2 |
| HourFromStartHh | `79` | 예시: 프로젝트 시작 시점으로부터 -2, -1, 1, 2, 3시간. |
| HourFromStartHhh | `78` | 예시: H-2, H-1, H1, H2, H3 |
| HourFromStartHourHh | `38` | 예시: 시간 -2, 시간 -1, 시간 1, 시간 2, 시간 3 |
| MinuteHhMmAm | `33` | 예시: 8:00 AM, 8:01 AM, 8:02 AM. 시간 단위는 TimescaleMinutes이어야 합니다. |
| MinuteMm | `34` | 예시: 0, 1, 2, ..., 59분 |
| MinuteFromEndMinuteMm | `37` | 예시: 프로젝트 종료 시점으로부터 Minute 181, Minute 180, ..., Minute 1, Minute -1 |
| MinuteFromEndMm | `81` | 예시: 181, 180, ..., 1, -1 |
| MinuteFromEndMmm | `80` | 예시: M181, M180, ..., M1, M-1 |
| MinuteFromStartMinuteMm | `36` | 예시: 프로젝트 시작 시점으로부터 Minute -2, Minute -1, Minute 1, ... Minute 180 |
| MinuteFromStartMm | `83` | 예시: -2, -1, 1, ..., 180 |
| MinuteFromStartMmm | `82` | 예시: M-2, M-1, M1, ..., M180 |
| MonthM | `11` | 예시: M, A, M, J, J. 시간 단위는 TimescaleMonths이어야 합니다. |
| MonthMm | `57` | 예시: 11, 12, 1, 2 |
| MonthMmYy | `86` | 예시: 3/10, 4/10, 5/10 |
| MonthMmYyy | `85` | 예시: 3 '10, 4 '10, 5 '10 |
| MonthMmm | `10` | 예시는 Mar, Apr, May |
| MonthMmmYyy | `8` | 예시는 Mar '10, Apr '10, May '10 |
| MonthMmmm | `9` | 예시는 March, April, May |
| MonthMmmmYyyy | `7` | 예시는 March 2010, April 2010, May 2010 |
| MonthFromEndMm | `59` | 예시는 프로젝트 종료 시점부터 2개월, 1개월, -1개월, -2개월입니다. |
| MonthFromEndMmm | `58` | 예시는 M2, M1, M-1, M-2 |
| MonthFromEndMonthMm | `45` | 예시는 Month 2, Month 1, Month -1, Month -2 |
| MonthFromStartMm | `61` | 예시는 프로젝트 시작 시점부터 -2개월, -2개월, 1개월, 2개월입니다. |
| MonthFromStartMmm | `60` | 예시는 M-2, M-1, M1, M2 |
| MonthFromStartMonthMm | `44` | 예시는 Month -2, Month -1, Month 1, Month 2 |
| QuarterQ | `62` | 예시는 3, 4, 1. 시간 단위는 TimescaleQuarters이어야 합니다. |
| QuarterQq | `6` | 예시는 Q3, Q4, Q1 |
| QuarterQqYyy | `4` | 예시는 Q3 '10, Q4 '10, Q1 '11 |
| QuarterQqqQuarter | `2` | 예시는 3rd Quarter, 1st Quarter |
| QuarterQQyy | `51` | 예시는 3Q10, 4Q10, 1Q11 |
| QuarterQtrQ | `5` | 예시는 Qtr3, Qtr4, Qtr1 |
| QuarterQtrQYyyy | `3` | 예시는 Qtr3, 2010; Qtr4, 2010; Qtr1, 2011 |
| QuarterFromEndQ | `64` | 예시는 프로젝트 종료 시점부터 5분기, 4분기, 3분기, 2분기, 1분기, -1분기입니다. |
| QuarterFromEndQq | `63` | 예시는 Q5, Q4, Q3, Q2, Q1, Q-1 |
| QuarterFromEndQuarterQ | `47` | 예시는 Quarter 5, Quarter 4, Quarter 3, Quarter 2, Quarter 1, Quarter -1 |
| QuarterFromStartQ | `66` | 예시는 프로젝트 시작 시점부터 -5분기, -4분기, -3분기, -2분기, -1분기, 1분기입니다. |
| QuarterFromStartQq | `65` | 예시는 Q-5, Q-4, Q-3, Q-2, Q-1, Q1 |
| QuarterFromStartQuarterQ | `46` | 예시는 Quarter -5, Quarter -4, Quarter -3, Quarter -2, Quarter -1, Quarter 1 |
| ThirdsOfMonthsDd | `136` | 예시는 1, 11, 21, 1. 시간 단위는 TimescaleThirdsOfMonths이어야 합니다. |
| ThirdsOfMonthsDdd | `137` | 예시는 B, M, E, B |
| ThirdsOfMonthsDddd | `138` | 예제는 시작, 중간, 끝, 시작 |
| ThirdsOfMonthsMmDd | `139` | 예시는 3/1입니다. |
| ThirdsOfMonthsMmDdYy | `145` | 예시는 3/1/10입니다. |
| ThirdsOfMonthsMmDdd | `140` | 예제는 3/B, 3/M, 3/E, 4/B입니다. |
| ThirdsOfMonthsMmDddYy | `146` | 예시는 3/B/10입니다. |
| ThirdsOfMonthsMmmDd | `142` | 예제는 3월 1일, 3월 11일, 3월 21일, 4월 1일 |
| ThirdsOfMonthsMmmDdYy | `147` | 예제는 3월 1일, '10; 3월 11일, '10; 3월 21일, '10; 4월 1일, 10 |
| ThirdsOfMonthsMmmDdd | `143` | 예제는 3월 B, 3월 M, 3월 E, 4월 B |
| ThirdsOfMonthsMmmDddYy | `148` | 예제는 3월 B, '10; 3월 M, '10; 3월 E, '10; 4월 B '10 |
| ThirdsOfMonthsMmmmDd | `144` | 예제는 3월 1일, 3월 11일, 3월 21일, 4월 1일 |
| ThirdsOfMonthsMmmmDdYyyy | `149` | 예제는 3월 1일, 2010; 3월 11일, 2010; 3월 21일, 2010; 4월 1일, 2010 |
| ThirdsOfMonthsMmmmDddd | `141` | 예제는 3월 시작, 3월 중간, 3월 끝, 4월 시작 |
| ThirdsOfMonthsMmmmDdddYyyy | `150` | 예제는 3월 시작, 2010; 3월 중간, 2010; 3월 끝, 2010; 4월 시작, 2010 |
| WeekDddDd | `88` | 예제는 일요일 21, 일요일 28, 일요일 4. 시간 단위는 TimescaleWeeks이어야 합니다. |
| WeekDddMDd | `97` | 예제는 일요일 M 21, 일요일 M 28, 일요일 A 4 |
| WeekDddMmDd | `90` | 예제는 일요일 3/21, 일요일 3/28, 일요일 4/4 |
| WeekDddMmDdYy | `100` | 예제는 일요일 3/21/10, 일요일 3/28/10, 일요일 4/4/10 |
| WeekDddMmmDd | `93` | 예제는 일요일 3월 21일, 일요일 3월 28일, 일요일 4월 4일 |
| WeekDddMmmDdYyy | `101` | 예제는 일요일 3월 21일, '10; 일요일 3월 28일, '10; 일요일 4월 4일, '10 |
| WeekDddMmmmDd | `96` | 예제는 일요일 3월 21일, 일요일 3월 28일, 일요일 4월 4일 |
| WeekDddMmmmDdYyy | `102` | 예제는 일요일 3월 21일, '10; 일요일 3월 28일, '10; 일요일 4월 4일, '10 |
| WeekDddWw | `103` | 예제는 일요일 12, 일요일 13, 일요일 14 |
| WeekDdiMDd | `98` | 예제는 일요일 M 21, 일요일 M 28, 일요일 A 4 |
| WeekDdiMmDd | `91` | 예제는 일요일 3/21. 일요일 3/28, 일요일 4/4 |
| WeekDdiMmmDd | `94` | 예제는 일요일 3월 21일, 일요일 3월 28일, 일요일 4월 4일 |
| WeekDiMDd | `99` | 예시: S M 21, S M 28, S A 4 |
| WeekDiMmDd | `92` | 예시: S 3/21, S 3/28, S 4/4 |
| WeekDiMmmDd | `95` | 예시: S Mar 21, S Mar 28, S Apr 4 |
| WeekMDd | `89` | 예시: M21, M28, A 4 |
| WeekMmDd | `17` | 예시: 3/21, 3/28, 4/4 |
| WeekMmDdYy | `16` | 예시는 '3/21/10'. |
| WeekMmmDd | `15` | 예시: Mar 21, Mar 28, Apr 4 |
| WeekMmmDdYyy | `13` | 예시: Mar 21, '10; Mar 28, '10; Apr 4, '10 |
| WeekMmmmDd | `14` | 예시: March 21, March 28, April 4 |
| WeekMmmmDdYyyy | `12` | 예시: March 21, 2010; March 28, 2010; April 4, 2010 |
| WeekDayOfMonthDd | `87` | 예시: 21, 28, 4 |
| WeekFromEndWeekWw | `43` | 예시: Week 2, Week 1, Week -1 프로젝트 종료 시점부터. |
| WeekFromEndWw | `68` | 예시: 2, 1, -1 |
| WeekFromEndWww | `67` | 예시: W2, W1, W-1 |
| WeekFromStartWeekWw | `42` | 예시: Week -1, Week 1, Week 2 프로젝트 시작 시점부터. |
| WeekFromStartWw | `70` | 예시: -1, 1, 2 |
| WeekFromStartWww | `69` | 예시: W-1, W1, W2 |
| WeekNumberDdWw | `104` | 예시: 1 12, 1 13, 1 14 (주 12의 1일, 주 13의 1일 등) |
| WeekNumberWw | `50` | 예시: 12, 13, 14 |
| YearYy | `75` | 예시: 10, 11, 12. 시간 단위는 TimescaleYears이어야 합니다. |
| YearYyy | `1` | 예시: '10, '11, '12 |
| YearYyyy | `0` | 예시: 2010, 2011, 2012 |
| YearFromEndYearYy | `49` | 예시: Year 2, Year 1, Year -1 프로젝트 종료 시점부터. |
| YearFromEndYy | `72` | 예시: 2, 1, -1 |
| YearFromEndYyy | `71` | 예시: Y2, Y1, Y-1 |
| YearFromStartYearYy | `48` | 예시: Year -1, Year 1, Year 2 프로젝트 시작 시점부터. |
| YearFromStartYy | `74` | 예시: -1, 1, 2 |
| YearFromStartYyy | `73` | 예제는 Y-1, Y1, Y2 |

## 예제

작업 링크 추가

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");

// 시간 눈금 티어 조정
project.TaskLinks.Add(project.RootTask.Children.Add("Task 1"), project.RootTask.Children.Add("Task 2"));

var view = (GanttChartView)project.DefaultView;

// 상위 티어 조정

// 간트 차트 보기의 최상위 시간 눈금 티어를 설정합니다.
// 시간 눈금 티어에 대한 시간 눈금 단위 <see cref="T:Aspose.Tasks.Visualization.TimescaleUnit" />를 설정합니다.
view.MiddleTimescaleTier = new TimescaleTier();
// 티어에 레이블을 표시할 시간 단위 간격을 설정합니다.
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
// 시간 눈금 티어에 대한 날짜 레이블 <see cref="T:Aspose.Tasks.Visualization.DateLabel" />을 설정합니다.
view.MiddleTimescaleTier.Count = 1;
// 티어의 각 시간 기간 내에서 레이블을 정렬하는 방법을 설정합니다 (<see cref="T:System.Drawing.StringAlignment" />).
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
// 계층의 각 시간 기간 내에서 레이블을 정렬하는 방법을 설정합니다 (<see cref="T:System.Drawing.StringAlignment" />).
view.MiddleTimescaleTier.Alignment = HorizontalStringAlignment.Center;
// 계층에서 시간 기간을 구분하는 눈금 표시를 표시할지 여부를 나타내는 값을 설정합니다.
view.MiddleTimescaleTier.ShowTicks = true;
// 계층 레이블을 회계 연도에 기반하도록 할지 여부를 나타내는 값을 설정합니다.
view.MiddleTimescaleTier.UsesFiscalYear = true;

// 시각화를 개선하기 위해 추가되었습니다.
view.TopTimescaleTier = new TimescaleTier(TimescaleUnit.Months, 1);

// 중간 계층 날짜를 사용자 지정합니다.
view.TopTimescaleTier.DateTimeConverter = date =>
    new[] { "Янв.", "Фев.", "Мар.", "Апр.", "Май", "Июнь", "Июль", "Авг.", "Сен.", "Окт.", "Ноя.", "Дек." }[date.Month - 1];

project.Set(Prj.TimescaleStart, new DateTime(2012, 7, 30));
project.Set(Prj.TimescaleFinish, new DateTime(2012, 10, 6));

// 뷰에 정의된 타임스케일 설정(view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier)을 사용하여 타임스케일을 렌더링하려면 'Timescale.DefinedInView' 옵션을 사용합니다.
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "CustomizeTimescaleTierLabels_out.pdf", pdfSaveOptions);
```

### 또 보기

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


