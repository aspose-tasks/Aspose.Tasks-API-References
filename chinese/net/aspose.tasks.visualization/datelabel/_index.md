---
title: DateLabel
second_title: Aspose.Tasks for .NET API 参考
description: 指定时间刻度中日期和时间标签的显示格式
type: docs
weight: 2630
url: /zh/net/aspose.tasks.visualization/datelabel/
---
## DateLabel enumeration

指定时间刻度中日期和时间标签的显示格式。

```csharp
public enum DateLabel
```

### 价值观

| 姓名 | 价值 | 描述 |
| --- | --- | --- |
| None | `35` | 不显示日期。 |
| DayDdd | `19` | 例如周一、周二。 |
| DayDddDd | `105` | 例如周一 30、周二 1 |
| DayDddMDd | `112` | 例如周一 S 30，周二 O 1 |
| DayDddMmDd | `108` | 例如 9 月 30 日星期一、10 月 1 日星期二 |
| DayDddMmDdYy | `52` | 例如 2002 年 9 月 30 日星期一、2002 年 1 月 1 日星期二 |
| DayDddMmmDd | `23` | 示例是 9 月 30 日星期一，10 月 1 日星期二 |
| DayDddMmmDdYyy | `22` | 示例为 2002 年 9 月 30 日星期一、2002 年 10 月 1 日星期二 |
| DayDddMmmmDd | `111` | 示例是 9 月 30 日星期一，10 月 1 日星期二 |
| DayDddd | `18` | 例如星期二、星期三。 |
| DayDdi | `119` | 例子是莫、涂 |
| DayDdiDd | `106` | 例子是 Mo 30, Tu 1 |
| DayDdiMDd | `113` | 例子是 Mo S 30, Tu O 1 |
| DayDdiMmDd | `109` | 例子是 Mo 9/30，Tu 10/1 |
| DayDi | `20` | 例子是 M, T |
| DayDiDdSpace | `107` | 例子是 M 30, T 1 |
| DayDiMDd | `114` | 例如 MS 30，TO 1 |
| DayDiMmDd | `110` | 例如 M 9/30、T 10/1 |
| DayDiDdNoSpace | `121` | 例如 M30、T1 |
| DayMDd | `115` | 例如 S 30, O 1 |
| DayMmDd | `27` | 例如 9/30、10/1 |
| DayMmDdYy | `26` | 例如 9/30/02、10/1/02 |
| DayMmmDd | `25` | 示例为 9 月 30 日、10 月 1 日 |
| DayMmmDdYyy | `24` | 示例为 2002 年 9 月 30 日、2002 年 10 月 10 日 |
| DayFromEndDayDd | `41` | 示例是项目结束后的第 2 天、第 1 天、第 -1 天、第 -2 天。 |
| DayFromEndDd | `54` | 示例为 2、1、-1、-2 |
| DayFromEndDdd | `53` | 示例为 D2、D1、D-1、D-2 |
| DayFromStartDayDd | `40` | 示例是项目开始后的第 -2 天、第 -1 天、第 1 天、第 2 天。 |
| DayFromStartDd | `56` | 示例为 -2、-1、1、2 |
| DayFromStartDdd | `55` | 示例为 D-2、D-1、D1、D2 |
| DayOfMonthDd | `21` | 例子是 30, 1 |
| DayOfYearDd | `118` | 示例为 77、78 |
| DayOfYearDdYyy | `116` | 例如 77 '10, 78 '10 |
| DayOfYearDdYyyy | `117` | 示例为 77 2010、78 2010 |
| DayDdMmYyyy | `256` | 示例是 19/07/2016. |
| HalfYearH | `128` | 示例为 1、2。要求时间单位为 TimescaleHalfYears. |
| HalfYearHh | `127` | 示例为 H1、H2 |
| HalfYearHhYyy | `126` | 示例为 H1 '10、H2 '10 |
| HalfYearHhhHalf | `123` | 示例是第一半，第二半 |
| HalfYearHHyy | `129` | 示例为 1H10、2H10 |
| HalfYearHlfH | `125` | 示例是一半 1，一半 2 |
| HalfYearHlfHYyyy | `124` | 示例为 2010 年半月 1； 2010 年半 2 |
| HalfYearFromEndH | `135` | 示例为 2、1、-1、-2。自项目结束日期起半年。 |
| HalfYearFromEndHalfH | `133` | 示例为半 2、半 1、半 -1、半 -2 |
| HalfYearFromEndHh | `134` | 示例为 H2、H1、H-1、H-2 |
| HalfYearFromStartH | `132` | 示例为 -2、-1、1、2。自项目开始日期起半年。 |
| HalfYearFromStartHalfH | `130` | 示例为半 -2、半 -1、半 1、半 2 |
| HalfYearFromStartHh | `131` | 示例为 H-2、H-1、H1、H2 |
| HourDddMmmDdHhAm | `28` | 示例是 3 月 18 日星期三上午 8 点； 3 月 18 日星期三，上午 9 点。要求时间单位为 TimescaleHours. |
| HourHh | `32` | 示例为 8、9、10、11 |
| HourHhMmAm | `30` | 例如上午 8:00、上午 9:00 |
| HourHhAm | `31` | 例如上午 8 点、上午 9 点 |
| HourMmDdHhAm | `120` | 示例是 3/18 上午 8 点，3/18 上午 9 点 |
| HourMmmDdHhAm | `29` | 示例是 3 月 18 日上午 8 点； 3 月 18 日，上午 9 点 |
| HourFromEndHh | `77` | 示例是项目结束后 3、2、1、-1、-2 小时。 |
| HourFromEndHhh | `76` | 示例为 H3、H2、H1、H-1、H-2 |
| HourFromEndHourHh | `39` | 示例为第 3 小时、第 2 小时、第 1 小时、第 -1 小时、第 -2 小时 |
| HourFromStartHh | `79` | 示例是项目开始后的 -2、-1、1、2、3 小时。 |
| HourFromStartHhh | `78` | 示例为 H-2、H-1、H1、H2、H3 |
| HourFromStartHourHh | `38` | 示例为 -2 小时、-1 小时、1 小时、2 小时、3 小时 |
| MinuteHhMmAm | `33` | 例如上午 8:00、上午 8:01、上午 8:02。要求时间单位为 TimescaleMinutes. |
| MinuteMm | `34` | 示例为 0、1、2、...、59 分钟 |
| MinuteFromEndMinuteMm | `37` | 示例是从项目结束开始的第 181 分钟、第 180 分钟、...、第 1 分钟、第 -1 分钟。 |
| MinuteFromEndMm | `81` | 示例为 181、180、...、1、-1 |
| MinuteFromEndMmm | `80` | 例子是 M181, M180, ..., M1, M-1 |
| MinuteFromStartMinuteMm | `36` | 示例是 Minute -2, Minute -1, Minute 1, ... 从项目开始的第 180 分钟。 |
| MinuteFromStartMm | `83` | 示例为 -2、-1、1、...、180 |
| MinuteFromStartMmm | `82` | 示例为 M-2、M-1、M1、...、M180 |
| MonthM | `11` | 示例为 M、A、M、J、J。要求时间单位为 TimescaleMonths。 |
| MonthMm | `57` | 示例为 11、12、1、2 |
| MonthMmYy | `86` | 例如 3/10、4/10、5/10 |
| MonthMmYyy | `85` | 示例为 3 '10、4 '10、5 '10 |
| MonthMmm | `10` | 例如三月、四月、五月 |
| MonthMmmYyy | `8` | 示例为 10 年 3 月、10 年 4 月、10 年 5 月 |
| MonthMmmm | `9` | 例如三月、四月、五月 |
| MonthMmmmYyyy | `7` | 示例为 2010 年 3 月、2010 年 4 月、2010 年 5 月 |
| MonthFromEndMm | `59` | 示例是项目结束后的 2、1、-1、-2 个月。 |
| MonthFromEndMmm | `58` | 示例是 M2、M1、M-1、M-2 |
| MonthFromEndMonthMm | `45` | 示例为第 2 个月、第 1 个月、第 -1 个月、第 -2 个月 |
| MonthFromStartMm | `61` | 示例是项目开始后的 -2、-2、1、2 个月。 |
| MonthFromStartMmm | `60` | 示例为 M-2、M-1、M1、M2 |
| MonthFromStartMonthMm | `44` | 示例为月 -2、月 -1、月 1、月 2 |
| QuarterQ | `62` | 示例为 3、4、1。要求时间单位为 TimescaleQuarters。 |
| QuarterQq | `6` | 示例是 Q3、Q4、Q1 |
| QuarterQqYyy | `4` | 示例为 10 年第 3 季度、10 年第 4 季度、11 年第 1 季度 |
| QuarterQqqQuarter | `2` | 例如第三季度、第一季度 |
| QuarterQQyy | `51` | 例如 2010 年 3 季度、2010 年 4 季度、1Q11 |
| QuarterQtrQ | `5` | 示例是 Qtr3、Qtr4、Qtr1 |
| QuarterQtrQYyyy | `3` | 示例为 2010 年第 3 季度； 2010 年第四季度； 2011 年第一季度 |
| QuarterFromEndQ | `64` | 示例是距离项目结束 5、4、3、2、1、-1 个季度。 |
| QuarterFromEndQq | `63` | 示例是 Q5、Q4、Q3、Q2、Q1、Q-1 |
| QuarterFromEndQuarterQ | `47` | 示例为第 5 季度、第 4 季度、第 3 季度、第 2 季度、第 1 季度、第 -1 季度 |
| QuarterFromStartQ | `66` | 示例是项目开始后的 -5、-4、-3、-2、-1、1 个季度。 |
| QuarterFromStartQq | `65` | 示例为 Q-5、Q-4、Q-3、Q-2、Q-1、Q1 |
| QuarterFromStartQuarterQ | `46` | 示例为 -5 季度、-4 季度、-3 季度、-2 季度、-1 季度、1 季度 |
| ThirdsOfMonthsDd | `136` | 示例为 1、11、21、1。要求时间单位为 TimescaleThirdsOfMonths. |
| ThirdsOfMonthsDdd | `137` | 示例为 B、M、E、B |
| ThirdsOfMonthsDddd | `138` | 示例是开头、中间、结尾、开头 |
| ThirdsOfMonthsMmDd | `139` | 例子是 3/1. |
| ThirdsOfMonthsMmDdYy | `145` | 示例是 2010 年 3 月 1 日。 |
| ThirdsOfMonthsMmDdd | `140` | 示例为 3/B、3/M、3/E、4/B |
| ThirdsOfMonthsMmDddYy | `146` | 例子是 3/B/10. |
| ThirdsOfMonthsMmmDd | `142` | 示例为 3 月 1 日、3 月 11 日、3 月 21 日、4 月 1 日 |
| ThirdsOfMonthsMmmDdYy | `147` | 示例为 2010 年 3 月 1 日； 2010 年 3 月 11 日； 2010 年 3 月 21 日； 10 年 4 月 1 日 |
| ThirdsOfMonthsMmmDdd | `143` | 例如三月 B、三月 M、三月 E、四月 B |
| ThirdsOfMonthsMmmDddYy | `148` | 例子是 Mar B, '10;三月，'10；三月E，'10；四月 B '10 |
| ThirdsOfMonthsMmmmDd | `144` | 示例为 3 月 1 日、3 月 11 日、3 月 21 日、4 月 1 日 |
| ThirdsOfMonthsMmmmDdYyyy | `149` | 示例为 2010 年 3 月 1 日； 2010 年 3 月 11 日； 2010 年 3 月 21 日； 2010 年 4 月 1 日 |
| ThirdsOfMonthsMmmmDddd | `141` | 例如三月开始、三月中旬、三月结束、四月开始 |
| ThirdsOfMonthsMmmmDdddYyyy | `150` | 示例为 2010 年 3 月开始； 2010年3月中旬； 2010 年 3 月下旬； 2010 年 4 月开始 |
| WeekDddDd | `88` | 示例为 Sun 21、Sun 28、Sun 4。要求时间单位为 TimescaleWeeks。 |
| WeekDddMDd | `97` | 例如 Sun M 21、Sun M 28、Sun A 4 |
| WeekDddMmDd | `90` | 示例为 Sun 3/21、Sun 3/28、Sun 4/4 |
| WeekDddMmDdYy | `100` | 示例为 Sun 3/21/10、Sun 3/28/10、Sun 4/4/10 |
| WeekDddMmmDd | `93` | 例如，3 月 21 日星期日、3 月 28 日星期日、4 月 4 日星期日 |
| WeekDddMmmDdYyy | `101` | 例如，2010 年 3 月 21 日星期日； 10 年 3 月 28 日，星期日； 4 月 4 日，星期日，'10 |
| WeekDddMmmmDd | `96` | 例如，3 月 21 日星期日、3 月 28 日星期日、4 月 4 日星期日 |
| WeekDddMmmmDdYyy | `102` | 例如，2010 年 3 月 21 日星期日； 2010 年 3 月 28 日，星期日；周日 4 月 4 日，'10 |
| WeekDddWw | `103` | 例如太阳 12、太阳 13、太阳 14 |
| WeekDdiMDd | `98` | 示例是 Su M 21、Su M 28、Su A 4 |
| WeekDdiMmDd | `91` | 例如 Su 3/21。苏3/28，苏4/4 |
| WeekDdiMmmDd | `94` | 示例是 Su Mar 21、Su Mar 28、Su Apr 4 |
| WeekDiMDd | `99` | 示例为 SM 21、SM 28、SA 4 |
| WeekDiMmDd | `92` | 例如 S 3/21、S 3/28、S 4/4 |
| WeekDiMmmDd | `95` | 示例为 3 月 21 日、3 月 28 日、4 月 4 日 |
| WeekMDd | `89` | 示例是 M21、M28、A 4 |
| WeekMmDd | `17` | 例如 3/21、3/28、4/4 |
| WeekMmDdYy | `16` | 示例是“2010 年 3 月 21 日”。 |
| WeekMmmDd | `15` | 示例是 3 月 21 日、3 月 28 日、4 月 4 日 |
| WeekMmmDdYyy | `13` | 例如 2010 年 3 月 21 日； 2010 年 3 月 28 日； 4 月 4 日，'10 |
| WeekMmmmDd | `14` | 示例为 3 月 21 日、3 月 28 日、4 月 4 日 |
| WeekMmmmDdYyyy | `12` | 示例为 2010 年 3 月 21 日； 2010 年 3 月 28 日； 2010 年 4 月 4 日 |
| WeekDayOfMonthDd | `87` | 例如 21、28、4 |
| WeekFromEndWeekWw | `43` | 示例是项目结束后的第 2 周、第 1 周、第 -1 周。 |
| WeekFromEndWw | `68` | 示例为 2、1、-1 |
| WeekFromEndWww | `67` | 例如 W2、W1、W-1 |
| WeekFromStartWeekWw | `42` | 示例是项目开始后的第 -1 周、第 1 周、第 2 周。 |
| WeekFromStartWw | `70` | 示例为 -1、1、2 |
| WeekFromStartWww | `69` | 示例是 W-1、W1、W2 |
| WeekNumberDdWw | `104` | 示例为 1 12、1 13、1 14（第 12 周的第 1 天、第 13 周的第 1 天等） |
| WeekNumberWw | `50` | 示例为 12、13、14 |
| YearYy | `75` | 示例为 10、11、12。要求时间单位为 TimescaleYears。 |
| YearYyy | `1` | 示例为 '10、'11、'12 |
| YearYyyy | `0` | 示例为 2010、2011、2012 |
| YearFromEndYearYy | `49` | 示例是项目结束后的第 2 年、第 1 年、第 -1 年。 |
| YearFromEndYy | `72` | 示例为 2、1、-1 |
| YearFromEndYyy | `71` | 示例是 Y2、Y1、Y-1 |
| YearFromStartYearYy | `48` | 示例是项目开始后的第 -1 年、第 1 年、第 2 年。 |
| YearFromStartYy | `74` | 示例为 -1、1、2 |
| YearFromStartYyy | `73` | 示例是 Y-1、Y1、Y2 |

### 也可以看看

* 命名空间 [Aspose.Tasks.Visualization](../../aspose.tasks.visualization)
* 部件 [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
