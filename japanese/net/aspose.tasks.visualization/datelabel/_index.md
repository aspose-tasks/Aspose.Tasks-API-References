---
title: DateLabel
second_title: Aspose.Tasks for .NET API リファレンス
description: タイムスケールの日付と時刻のラベルの表示形式を指定します
type: docs
weight: 2650
url: /ja/net/aspose.tasks.visualization/datelabel/
---
## DateLabel enumeration

タイムスケールの日付と時刻のラベルの表示形式を指定します。

```csharp
public enum DateLabel
```

### 値

| 名前 | 価値 | 説明 |
| --- | --- | --- |
| None | `35` | 日付は表示されません。 |
| DayDdd | `19` | 例は月曜日、火曜日です。 |
| DayDddDd | `105` | 例は月 30、火 1 です。 |
| DayDddMDd | `112` | 例は、Mon S 30、Tue O 1 です。 |
| DayDddMmDd | `108` | 例は月 9/30、火 10/1 |
| DayDddMmDdYy | `52` | 例は、Mon 9/30/02、Tue 10/1/02 です。 |
| DayDddMmmDd | `23` | 例: 月 9 月 30 日、火 10 月 1 |
| DayDddMmmDdYyy | `22` | 例は、Mon Sep 30 '02、Tue Oct 1 '02 です。 |
| DayDddMmmmDd | `111` | 例: 9 月 30 日月曜日、10 月 1 日火曜日 |
| DayDddd | `18` | 例は火曜日、水曜日です。 |
| DayDdi | `119` | 例は Mo、Tu |
| DayDdiDd | `106` | 例は Mo 30、Tu 1 |
| DayDdiMDd | `113` | 例は Mo S 30、Tu O 1 |
| DayDdiMmDd | `109` | 例は Mo 9/30、Tu 10/1 です。 |
| DayDi | `20` | 例は M、T です。 |
| DayDiDdSpace | `107` | 例は M 30、T 1 です。 |
| DayDiMDd | `114` | 例は MS 30、TO 1 です。 |
| DayDiMmDd | `110` | 例は M 9/30、T 10/1 です。 |
| DayDiDdNoSpace | `121` | 例は M30、T1 です。 |
| DayMDd | `115` | 例は S 30、O 1 です。 |
| DayMmDd | `27` | 例は 9/30、10/1 です。 |
| DayMmDdYy | `26` | 例は 9/30/02、10/1/02 です。 |
| DayMmmDd | `25` | 例は 9 月 30 日、10 月 1 日です |
| DayMmmDdYyy | `24` | 例は、2002 年 9 月 30 日、2002 年 10 月 10 日です |
| DayFromEndDayDd | `41` | 例は、プロジェクト終了から 2 日目、1 日目、-1 日目、-2 日目です。 |
| DayFromEndDd | `54` | 例は 2、1、-1、-2 です。 |
| DayFromEndDdd | `53` | 例は、D2、D1、D-1、D-2 です。 |
| DayFromStartDayDd | `40` | 例としては、プロジェクト開始から -2 日目、-1 日目、1 日目、2 日目です。 |
| DayFromStartDd | `56` | 例は -2、-1、1、2 です。 |
| DayFromStartDdd | `55` | 例は、D-2、D-1、D1、D2 です。 |
| DayOfMonthDd | `21` | 例は 30、1 |
| DayOfYearDd | `118` | 例は 77、78 です。 |
| DayOfYearDdYyy | `116` | 例は 77 '10、78 '10 です。 |
| DayOfYearDdYyyy | `117` | 例は 77 2010、78 2010 です。 |
| DayDdMmYyyy | `256` | 例は 19/07/2016 です。 |
| HalfYearH | `128` | 例は 1、2 です。時間単位は TimescaleHalfYears である必要があります。 |
| HalfYearHh | `127` | 例は H1、H2 です。 |
| HalfYearHhYyy | `126` | 例: H1 '10、H2 '10 |
| HalfYearHhhHalf | `123` | 例は前半、後半です |
| HalfYearHHyy | `129` | 例は 1H10、2H10 です。 |
| HalfYearHlfH | `125` | 例はハーフ 1、ハーフ 2 です。 |
| HalfYearHlfHYyyy | `124` | 例は、2010 年半期 1 日です。 2010年上半期 |
| HalfYearFromEndH | `135` | 例は 2、1、-1、-2 です。プロジェクト終了日から半年. |
| HalfYearFromEndHalfH | `133` | 例は、Half 2、Half 1、Half -1、Half -2 です。 |
| HalfYearFromEndHh | `134` | 例は、H2、H1、H-1、H-2 です。 |
| HalfYearFromStartH | `132` | 例: -2、-1、1、2。プロジェクト開始日から半年。 |
| HalfYearFromStartHalfH | `130` | 例は、Half -2、Half -1、Half 1、Half 2 です。 |
| HalfYearFromStartHh | `131` | 例は、H-2、H-1、H1、H2 です。 |
| HourDddMmmDdHhAm | `28` | 例は、3 月 18 日水曜日、午前 8 時です。 3 月 18 日水曜日、午前 9 時。時間単位は TimescaleHours. である必要があります |
| HourHh | `32` | 例は 8、9、10、11 です。 |
| HourHhMmAm | `30` | 例: 午前 8:00、午前 9:00 |
| HourHhAm | `31` | 例は午前 8 時、午前 9 時 |
| HourMmDdHhAm | `120` | 例: 3/18 8 AM、3/18 9 AM |
| HourMmmDdHhAm | `29` | 例は、3 月 18 日午前 8 時です。 3月18日午前9時 |
| HourFromEndHh | `77` | 例は、プロジェクト終了から 3、2、1、-1、-2 時間です。 |
| HourFromEndHhh | `76` | 例は、H3、H2、H1、H-1、H-2 です。 |
| HourFromEndHourHh | `39` | 例: 3 時間、2 時間、1 時間、-1 時間、-2 時間 |
| HourFromStartHh | `79` | 例は、プロジェクト開始から -2、-1、1、2、3 時間です。 |
| HourFromStartHhh | `78` | 例は、H-2、H-1、H1、H2、H3 です。 |
| HourFromStartHourHh | `38` | 例: -2 時間、-1 時間、1 時間、2 時間、3 時間 |
| MinuteHhMmAm | `33` | 例は、午前 8:00、午前 8:01、午前 8:02 です。時間単位は TimescaleMinutes. である必要があります |
| MinuteMm | `34` | 例は 0、1、2、...、59 分です |
| MinuteFromEndMinuteMm | `37` | 例は、プロジェクト終了から 181 分、180 分、...、1 分、-1 分です。 |
| MinuteFromEndMm | `81` | 例は 181、180、...、1、-1 です。 |
| MinuteFromEndMmm | `80` | 例は、M181、M180、...、M1、M-1 です。 |
| MinuteFromStartMinuteMm | `36` | 例は -2 分、-1 分、1 分、... プロジェクト開始から 180 分です。 |
| MinuteFromStartMm | `83` | 例は -2、-1、1、...、180 です。 |
| MinuteFromStartMmm | `82` | 例は、M-2、M-1、M1、...、M180 です。 |
| MonthM | `11` | 例は M、A、M、J、J です。時間単位は TimescaleMonths. である必要があります。 |
| MonthMm | `57` | 例は 11、12、1、2 です。 |
| MonthMmYy | `86` | 例は 3/10、4/10、5/10 です。 |
| MonthMmYyy | `85` | 例は 3 '10、4 '10、5 '10 です。 |
| MonthMmm | `10` | 例は 3 月、4 月、5 月です |
| MonthMmmYyy | `8` | 例: Mar '10、Apr '10、May '10 |
| MonthMmmm | `9` | 例は 3 月、4 月、5 月です |
| MonthMmmmYyyy | `7` | 例は 2010 年 3 月、2010 年 4 月、2010 年 5 月です |
| MonthFromEndMm | `59` | 例は、プロジェクト終了から 2、1、-1、-2 か月です。 |
| MonthFromEndMmm | `58` | 例は、M2、M1、M-1、M-2 です。 |
| MonthFromEndMonthMm | `45` | 例は月 2、月 1、月 -1、月 -2 です。 |
| MonthFromStartMm | `61` | 例は、プロジェクト開始から -2、-2、1、2 か月です。 |
| MonthFromStartMmm | `60` | 例は、M-2、M-1、M1、M2 です。 |
| MonthFromStartMonthMm | `44` | 例は、Month -2、Month -1、Month 1、Month 2 です。 |
| QuarterQ | `62` | 例は 3、4、1 です。時間単位は TimescaleQuarters. である必要があります。 |
| QuarterQq | `6` | 例は Q3、Q4、Q1 です。 |
| QuarterQqYyy | `4` | 例: Q3 '10、Q4 '10、Q1 '11 |
| QuarterQqqQuarter | `2` | 例は第 3 四半期、第 1 四半期です |
| QuarterQQyy | `51` | 例は 3Q10、4Q10、1Q11 です。 |
| QuarterQtrQ | `5` | 例は、Qtr3、Qtr4、Qtr1 です。 |
| QuarterQtrQYyyy | `3` | 例は、2010 年第 3 四半期です。 2010 年第 4 四半期。 2011 年第 1 四半期 |
| QuarterFromEndQ | `64` | 例は、プロジェクト終了から 5、4、3、2、1、-1 四半期です。 |
| QuarterFromEndQq | `63` | 例は Q5、Q4、Q3、Q2、Q1、Q-1 です。 |
| QuarterFromEndQuarterQ | `47` | 例は、Quarter 5、Quarter 4、Quarter 3、Quarter 2、Quarter 1、Quarter -1 です。 |
| QuarterFromStartQ | `66` | 例は、プロジェクト開始から -5、-4、-3、-2、-1、1 四半期です。 |
| QuarterFromStartQq | `65` | 例は、Q-5、Q-4、Q-3、Q-2、Q-1、Q1 です。 |
| QuarterFromStartQuarterQ | `46` | 例は、Quarter -5、Quarter -4、Quarter -3、Quarter -2、Quarter -1、Quarter 1 です。 |
| ThirdsOfMonthsDd | `136` | 例は 1、11、21、1 です。時間単位は TimescaleThirdsOfMonths である必要があります。 |
| ThirdsOfMonthsDdd | `137` | 例は B、M、E、B です。 |
| ThirdsOfMonthsDddd | `138` | 例は、Beginning、Middle、End、Beginning です。 |
| ThirdsOfMonthsMmDd | `139` | 例は 3/1. |
| ThirdsOfMonthsMmDdYy | `145` | 例は 3/1/10 です。 |
| ThirdsOfMonthsMmDdd | `140` | 例は 3/B、3/M、3/E、4/B です。 |
| ThirdsOfMonthsMmDddYy | `146` | 例は 3/B/10 です。 |
| ThirdsOfMonthsMmmDd | `142` | 例は、3 月 1 日、3 月 11 日、3 月 21 日、4 月 1 です。 |
| ThirdsOfMonthsMmmDdYy | `147` | 例は、'10 年 3 月 1 日です。 2010 年 3 月 11 日; 2010 年 3 月 21 日; 10/04/01 |
| ThirdsOfMonthsMmmDdd | `143` | 例: 3 月 B、3 月 M、3 月 E、4 月 B |
| ThirdsOfMonthsMmmDddYy | `148` | 例は、2010 年 3 月 B です。 2010 年 3 月 M。 2010 年 3 月 E; 4 月 B '10 |
| ThirdsOfMonthsMmmmDd | `144` | 例: 3 月 1 日、3 月 11 日、3 月 21 日、4 月 1 日 |
| ThirdsOfMonthsMmmmDdYyyy | `149` | 例は 2010 年 3 月 1 日です。 2010 年 3 月 11 日。 2010 年 3 月 21 日。 2010 年 4 月 1 日 |
| ThirdsOfMonthsMmmmDddd | `141` | 例: 3 月上旬、3 月中旬、3 月下旬、4 月上旬 |
| ThirdsOfMonthsMmmmDdddYyyy | `150` | 例は 2010 年 3 月初めです。 2010 年 3 月中旬。 2010 年 3 月末。 2010年4月上旬 |
| WeekDddDd | `88` | 例は Sun 21、Sun 28、Sun 4 です。時間単位は TimescaleWeeks. である必要があります。 |
| WeekDddMDd | `97` | 例は、Sun M 21、Sun M 28、Sun A 4 です。 |
| WeekDddMmDd | `90` | 例は、Sun 3/21、Sun 3/28、Sun 4/4 です。 |
| WeekDddMmDdYy | `100` | 例は Sun 3/21/10、Sun 3/28/10、Sun 4/4/10 です。 |
| WeekDddMmmDd | `93` | 例: 3 月 21 日 (日)、3 月 28 日 (日)、4 月 4 日 (日) |
| WeekDddMmmDdYyy | `101` | 例は Sun Mar 21, '10; 2010 年 3 月 28 日（日） '10/04/04(日) |
| WeekDddMmmmDd | `96` | 例: 3 月 21 日 (日)、3 月 28 日 (日)、4 月 4 日 (日) |
| WeekDddMmmmDdYyy | `102` | 例は Sun March 21, '10; 2010年3月28日（日） '10/04/04(日) |
| WeekDddWw | `103` | 例は Sun 12、Sun 13、Sun 14 です。 |
| WeekDdiMDd | `98` | 例は、Su M 21、Su M 28、Su A 4 です。 |
| WeekDdiMmDd | `91` | 例は Su 3/21 です。す 3/28、す 4/4 |
| WeekDdiMmmDd | `94` | 例: Su Mar 21、Su Mar 28、Su Apr 4 |
| WeekDiMDd | `99` | 例は、SM 21、SM 28、SA 4 です。 |
| WeekDiMmDd | `92` | 例は S 3/21、S 3/28、S 4/4 です。 |
| WeekDiMmmDd | `95` | 例: S Mar 21、S Mar 28、S Apr 4 |
| WeekMDd | `89` | 例は、M21、M28、A 4 です。 |
| WeekMmDd | `17` | 例は 3/21、3/28、4/4 です。 |
| WeekMmDdYy | `16` | 例は「3/21/10」. |
| WeekMmmDd | `15` | 例は、3 月 21 日、3 月 28 日、4 月 4 です。 |
| WeekMmmDdYyy | `13` | 例は、'10 年 3 月 21 日です。 2010 年 3 月 28 日; '10/04/04 |
| WeekMmmmDd | `14` | 例は 3 月 21 日、3 月 28 日、4 月 4 日です |
| WeekMmmmDdYyyy | `12` | 例は 2010 年 3 月 21 日です。 2010 年 3 月 28 日。 2010 年 4 月 4 日 |
| WeekDayOfMonthDd | `87` | 例は 21、28、4 です。 |
| WeekFromEndWeekWw | `43` | 例は、プロジェクト終了から 2 週目、1 週目、-1 週目です。 |
| WeekFromEndWw | `68` | 例は 2、1、-1 です。 |
| WeekFromEndWww | `67` | 例は、W2、W1、W-1 です。 |
| WeekFromStartWeekWw | `42` | 例は、プロジェクト開始から週 -1、週 1、週 2 です。 |
| WeekFromStartWw | `70` | 例は -1、1、2 です。 |
| WeekFromStartWww | `69` | 例は、W-1、W1、W2 です。 |
| WeekNumberDdWw | `104` | 例は、1 12、1 13、1 14 (第 12 週の第 1 日、第 13 週の第 1 日など) です。 |
| WeekNumberWw | `50` | 例は 12、13、14 です。 |
| YearYy | `75` | 例は 10、11、12 です。時間単位は TimescaleYears. である必要があります。 |
| YearYyy | `1` | 例: '10、'11、'12 |
| YearYyyy | `0` | 例は 2010、2011、2012 です。 |
| YearFromEndYearYy | `49` | 例は、プロジェクト終了から 2 年目、1 年目、-1 年目です。 |
| YearFromEndYy | `72` | 例は 2、1、-1 です。 |
| YearFromEndYyy | `71` | 例は Y2、Y1、Y-1 です。 |
| YearFromStartYearYy | `48` | 例は、プロジェクト開始から -1 年、1 年、2 年です。 |
| YearFromStartYy | `74` | 例は -1、1、2 です。 |
| YearFromStartYyy | `73` | 例は Y-1、Y1、Y2 です。 |

### 関連項目

* 名前空間 [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* 組み立て [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
