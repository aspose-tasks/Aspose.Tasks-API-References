---
title: Enum DateLabel
second_title: Aspose.Tasks for .NET API 参考
description: Aspose.Tasks.Visualization.DateLabel 枚举. 指定时间刻度中日期和时间标签的显示格式
type: docs
weight: 2650
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
| None | `35` | 没有显示日期。 |
| DayDdd | `19` | 例如周一、周二。 |
| DayDddDd | `105` | 例如星期一 30，星期二 1 |
| DayDddMDd | `112` | 例子是星期一 S 30，星期二 O 1 |
| DayDddMmDd | `108` | 例如 9 月 30 日星期一、10 月 1 日星期二 |
| DayDddMmDdYy | `52` | 例如 Mon 9/30/02, Tue 10/1/02 |
| DayDddMmmDd | `23` | 例如 9 月 30 日星期一、10 月 1 日星期二 |
| DayDddMmmDdYyy | `22` | 例子是 Mon Sep 30 '02, Tue Oct 1 '02 |
| DayDddMmmmDd | `111` | 例如 9 月 30 日星期一、10 月 1 日星期二 |
| DayDddd | `18` | 例如星期二、星期三。 |
| DayDdi | `119` | 例子有 Mo, Tu |
| DayDdiDd | `106` | 示例为 Mo 30、Tu 1 |
| DayDdiMDd | `113` | 例子是 Mo S 30，Tu O 1 |
| DayDdiMmDd | `109` | 示例为 Mo 9/30、Tu 10/1 |
| DayDi | `20` | 例子有 M, T |
| DayDiDdSpace | `107` | 例如 M 30，T 1 |
| DayDiMDd | `114` | 例如 MS 30，TO 1 |
| DayDiMmDd | `110` | 例如 M 9/30、T 10/1 |
| DayDiDdNoSpace | `121` | 例如 M30、T1 |
| DayMDd | `115` | 例如 S 30、O 1 |
| DayMmDd | `27` | 示例为 9/30、10/1 |
| DayMmDdYy | `26` | 例如 9/30/02、10/1/02 |
| DayMmmDd | `25` | 例如 9 月 30 日、10 月 1 日 |
| DayMmmDdYyy | `24` | 例子是 Sep 30 '02, Oct 10 '02 |
| DayFromEndDayDd | `41` | 示例是项目结束后的第 2 天、第 1 天、第 -1 天、第 -2 天。 |
| DayFromEndDd | `54` | 示例为 2、1、-1、-2 |
| DayFromEndDdd | `53` | 示例为 D2、D1、D-1、D-2 |
| DayFromStartDayDd | `40` | 示例是项目开始后的第 -2 天、第 -1 天、第 1 天、第 2 天。 |
| DayFromStartDd | `56` | 示例为 -2、-1、1、2 |
| DayFromStartDdd | `55` | 例如 D-2、D-1、D1、D2 |
| DayOfMonthDd | `21` | 例子是 30, 1 |
| DayOfYearDd | `118` | 例子是 77, 78 |
| DayOfYearDdYyy | `116` | 例子是 77 '10, 78 '10 |
| DayOfYearDdYyyy | `117` | 示例为 77 2010、78 2010 |
| DayDdMmYyyy | `256` | 例子是 19/07/2016. |
| HalfYearH | `128` | 例子是1、2。要求时间单位是TimescaleHalfYears. |
| HalfYearHh | `127` | 示例为 H1、H2 |
| HalfYearHhYyy | `126` | 例子是 H1 '10, H2 '10 |
| HalfYearHhhHalf | `123` | 例子是 1st Half, 2d Half |
| HalfYearHHyy | `129` | 示例为 1H10、2H10 |
| HalfYearHlfH | `125` | 示例是 Half 1，Half 2 |
| HalfYearHlfHYyyy | `124` | 示例是 2010 年第 1 场；下半场 2, 2010 |
| HalfYearFromEndH | `135` | 示例为 2、1、-1、-2。从项目结束日期起半年。 |
| HalfYearFromEndHalfH | `133` | 例子是一半 2，一半 1，一半 -1，一半 -2 |
| HalfYearFromEndHh | `134` | 例如 H2、H1、H-1、H-2 |
| HalfYearFromStartH | `132` | 示例为 -2、-1、1、2。从项目开始日期算起半年。 |
| HalfYearFromStartHalfH | `130` | 示例为 Half -2、Half -1、Half 1、Half 2 |
| HalfYearFromStartHh | `131` | 示例为 H-2、H-1、H1、H2 |
| HourDddMmmDdHhAm | `28` | 例如 3 月 18 日星期三上午 8 点； 3 月 18 日，星期三，上午 9 点。要求时间单位为TimescaleHours. |
| HourHh | `32` | 示例为 8、9、10、11 |
| HourHhMmAm | `30` | 示例为上午 8:00、上午 9:00 |
| HourHhAm | `31` | 例如上午 8 点、上午 9 点 |
| HourMmDdHhAm | `120` | 例子是 3/18 8 AM, 3/18 9 AM |
| HourMmmDdHhAm | `29` | 例如 3 月 18 日上午 8 点； 3 月 18 日上午 9 点 |
| HourFromEndHh | `77` | 示例是项目结束后的 3、2、1、-1、-2 小时。 |
| HourFromEndHhh | `76` | 例如 H3、H2、H1、H-1、H-2 |
| HourFromEndHourHh | `39` | 示例是小时 3、小时 2、小时 1、小时 -1、小时 -2 |
| HourFromStartHh | `79` | 示例是项目开始后的 -2、-1、1、2、3 小时。 |
| HourFromStartHhh | `78` | 示例为 H-2、H-1、H1、H2、H3 |
| HourFromStartHourHh | `38` | 示例为小时 -2、小时 -1、小时 1、小时 2、小时 3 |
| MinuteHhMmAm | `33` | 例如 8:00 AM、8:01 AM、8:02 AM。要求时间单位为TimescaleMinutes. |
| MinuteMm | `34` | 例子是 0, 1, 2, ..., 59 minutes |
| MinuteFromEndMinuteMm | `37` | 例如项目结束后的第 181 分钟、第 180 分钟、...、第 1 分钟、第 -1 分钟。 |
| MinuteFromEndMm | `81` | 例子是 181, 180, ..., 1, -1 |
| MinuteFromEndMmm | `80` | 例如 M181、M180、...、M1、M-1 |
| MinuteFromStartMinuteMm | `36` | 示例是 -2 分钟、-1 分钟、1 分钟...项目开始后的第 180 分钟。 |
| MinuteFromStartMm | `83` | 示例为 -2、-1、1、...、180 |
| MinuteFromStartMmm | `82` | 例如 M-2、M-1、M1、...、M180 |
| MonthM | `11` | 例子有M,A,M,J,J。要求时间单位为TimescaleMonths. |
| MonthMm | `57` | 示例为 11、12、1、2 |
| MonthMmYy | `86` | 示例为 3/10、4/10、5/10 |
| MonthMmYyy | `85` | 示例为 3 '10、4 '10、5 '10 |
| MonthMmm | `10` | 例如三月、四月、五月 |
| MonthMmmYyy | `8` | 例子是 Mar '10, Apr '10, May '10 |
| MonthMmmm | `9` | 例如三月、四月、五月 |
| MonthMmmmYyyy | `7` | 例如 2010 年 3 月、2010 年 4 月、2010 年 5 月 |
| MonthFromEndMm | `59` | 示例是项目结束后的 2、1、-1、-2 个月。 |
| MonthFromEndMmm | `58` | 例如 M2、M1、M-1、M-2 |
| MonthFromEndMonthMm | `45` | 例如第 2 个月、第 1 个月、第 -1 个月、第 -2 个月 |
| MonthFromStartMm | `61` | 示例是项目开始后的 -2、-2、1、2 个月。 |
| MonthFromStartMmm | `60` | 例如 M-2、M-1、M1、M2 |
| MonthFromStartMonthMm | `44` | 示例是 -2 月、-1 月、1 月、2 月 |
| QuarterQ | `62` | 例子是3, 4, 1。要求时间单位是TimescaleQuarters. |
| QuarterQq | `6` | 例如 Q3、Q4、Q1 |
| QuarterQqYyy | `4` | 示例为 Q3 '10、Q4 '10、Q1 '11 |
| QuarterQqqQuarter | `2` | 例如第三季度、第一季度 |
| QuarterQQyy | `51` | 例如 3Q10、4Q10、1Q11 |
| QuarterQtrQ | `5` | 示例为 Qtr3、Qtr4、Qtr1 |
| QuarterQtrQYyyy | `3` | 例如 2010 年第三季度； 2010 年第四季度； 2011 年第一季度 |
| QuarterFromEndQ | `64` | 示例是项目结束后的第 5、4、3、2、1、-1 个季度。 |
| QuarterFromEndQq | `63` | 示例为 Q5、Q4、Q3、Q2、Q1、Q-1 |
| QuarterFromEndQuarterQ | `47` | 例如第 5 季度、第 4 季度、第 3 季度、第 2 季度、第 1 季度、第 -1 |
| QuarterFromStartQ | `66` | 示例为 -5、-4、-3、-2、-1、项目开始后 1 个季度。 |
| QuarterFromStartQq | `65` | 示例为 Q-5、Q-4、Q-3、Q-2、Q-1、Q1 |
| QuarterFromStartQuarterQ | `46` | 示例是第 -5 季度、第 -4 季度、第 -3 季度、第 -2 季度、第 -1 季度、第 1 季度 |
| ThirdsOfMonthsDd | `136` | 例子是1, 11, 21, 1。要求时间单位是TimescaleThirdsOfMonths. |
| ThirdsOfMonthsDdd | `137` | 示例为 B、M、E、B |
| ThirdsOfMonthsDddd | `138` | 示例为 Beginning、Middle、End、Beginning |
| ThirdsOfMonthsMmDd | `139` | 例子是 3/1. |
| ThirdsOfMonthsMmDdYy | `145` | 示例是 3/1/10. |
| ThirdsOfMonthsMmDdd | `140` | 示例为 3/B、3/M、3/E、4/B |
| ThirdsOfMonthsMmDddYy | `146` | 例子是 3/B/10. |
| ThirdsOfMonthsMmmDd | `142` | 例如 3 月 1 日、3 月 11 日、3 月 21 日、4 月 1 日 |
| ThirdsOfMonthsMmmDdYy | `147` | 例子是 2010 年 3 月 1 日； 2010 年 3 月 11 日； 2010 年 3 月 21 日； 4 月 1 日，10 |
| ThirdsOfMonthsMmmDdd | `143` | 例如 Mar B、Mar M、Mar E、Apr B |
| ThirdsOfMonthsMmmDddYy | `148` | 例子是 Mar B, '10;三月男，'10;三月 E，'10; Apr B '10 |
| ThirdsOfMonthsMmmmDd | `144` | 例如 3 月 1 日、3 月 11 日、3 月 21 日、4 月 1 日 |
| ThirdsOfMonthsMmmmDdYyyy | `149` | 例子是 2010 年 3 月 1 日； 2010 年 3 月 11 日； 2010 年 3 月 21 日； 2010 年 4 月 1 日 |
| ThirdsOfMonthsMmmmDddd | `141` | 示例是三月初、三月中旬、三月末、四月初 |
| ThirdsOfMonthsMmmmDdddYyyy | `150` | 例子是 2010 年三月初； 2010年3月中旬； 2010 年 3 月底；四月初，2010 |
| WeekDddDd | `88` | 例如Sun 21, Sun 28, Sun 4。要求时间单位为TimescaleWeeks. |
| WeekDddMDd | `97` | 例如 Sun M 21、Sun M 28、Sun A 4 |
| WeekDddMmDd | `90` | 例如 Sun 3/21、Sun 3/28、Sun 4/4 |
| WeekDddMmDdYy | `100` | 例如 Sun 3/21/10、Sun 3/28/10、Sun 4/4/10 |
| WeekDddMmmDd | `93` | 例如 3 月 21 日星期日、3 月 28 日星期日、4 月 4 日星期日 |
| WeekDddMmmDdYyy | `101` | 例子是 Sun Mar 21, '10; 10 年 3 月 28 日，星期日； 4 月 4 日星期日，'10 |
| WeekDddMmmmDd | `96` | 例如 3 月 21 日星期日、3 月 28 日星期日、4 月 4 日星期日 |
| WeekDddMmmmDdYyy | `102` | 示例是 2010 年 3 月 21 日星期日； 10 年 3 月 28 日，星期日； 4 月 4 日星期日，'10 |
| WeekDddWw | `103` | 例如 Sun 12、Sun 13、Sun 14 |
| WeekDdiMDd | `98` | 示例为 Su M 21、Su M 28、Su A 4 |
| WeekDdiMmDd | `91` | 例子是 Su 3/21。苏 3/28，苏 4/4 |
| WeekDdiMmmDd | `94` | 例如 Su Mar 21, Su Mar 28, Su Apr 4 |
| WeekDiMDd | `99` | 例如 SM 21、SM 28、SA 4 |
| WeekDiMmDd | `92` | 例如 S 3/21、S 3/28、S 4/4 |
| WeekDiMmmDd | `95` | 例子是 S Mar 21, S Mar 28, S Apr 4 |
| WeekMDd | `89` | 例如 M21、M28、A 4 |
| WeekMmDd | `17` | 示例为 3/21、3/28、4/4 |
| WeekMmDdYy | `16` | 例子是 '3/21/10'. |
| WeekMmmDd | `15` | 例如 3 月 21 日、3 月 28 日、4 月 4 日 |
| WeekMmmDdYyy | `13` | 例子是 2010 年 3 月 21 日； 10 年 3 月 28 日； 4 月 4 日，'10 |
| WeekMmmmDd | `14` | 例如 3 月 21 日、3 月 28 日、4 月 4 日 |
| WeekMmmmDdYyyy | `12` | 例如 2010 年 3 月 21 日； 2010 年 3 月 28 日； 2010 年 4 月 4 日 |
| WeekDayOfMonthDd | `87` | 示例为 21、28、4 |
| WeekFromEndWeekWw | `43` | 示例是项目结束后的第 2 周、第 1 周、第 -1 周。 |
| WeekFromEndWw | `68` | 示例为 2、1、-1 |
| WeekFromEndWww | `67` | 示例为 W2、W1、W-1 |
| WeekFromStartWeekWw | `42` | 示例是项目开始的第 -1 周、第 1 周、第 2 周。 |
| WeekFromStartWw | `70` | 示例为 -1、1、2 |
| WeekFromStartWww | `69` | 示例为 W-1、W1、W2 |
| WeekNumberDdWw | `104` | 示例为 1 12、1 13、1 14（第 12 周的第 1 天、第 13 周的第 1 天，等等） |
| WeekNumberWw | `50` | 示例为 12、13、14 |
| YearYy | `75` | 例子是10, 11, 12。要求时间单位是TimescaleYears. |
| YearYyy | `1` | 示例为 '10、'11、'12 |
| YearYyyy | `0` | 例如 2010、2011、2012 |
| YearFromEndYearYy | `49` | 示例是项目结束后的第 2 年、第 1 年、第 -1 年。 |
| YearFromEndYy | `72` | 示例为 2、1、-1 |
| YearFromEndYyy | `71` | 示例为 Y2、Y1、Y-1 |
| YearFromStartYearYy | `48` | 示例是从项目开始的第 -1 年、第 1 年、第 2 年。 |
| YearFromStartYy | `74` | 示例为 -1、1、2 |
| YearFromStartYyy | `73` | 示例为 Y-1、Y1、Y2 |

### 也可以看看

* 命名空间 [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* 部件 [Aspose.Tasks](../../)


