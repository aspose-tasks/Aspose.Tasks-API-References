---
title: "日期标签"
second_title: "Aspose.Tasks for Java API 参考"
description: "指定时间轴中日期和时间标签的显示格式。"
type: docs
weight: 69
url: /zh/java/com.aspose.tasks/datelabel/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class DateLabel extends System.Enum
```

指定时间轴中日期和时间标签的显示格式。
## 字段

| 字段 | 描述 |
| --- | --- |
| [DayDdMmYyyy](#DayDdMmYyyy) | 示例为 19/07/2016。 |
| [DayDdd](#DayDdd) | 示例为 周一, 周二。 |
| [DayDddDd](#DayDddDd) | 示例为 周一 30, 周二 1 |
| [DayDddMDd](#DayDddMDd) | 示例为 周一 S 30, 周二 O 1 |
| [DayDddMmDd](#DayDddMmDd) | 示例为 周一 9/30, 周二 10/1 |
| [DayDddMmDdYy](#DayDddMmDdYy) | 示例为 周一 9/30/02, 周二 10/1/02 |
| [DayDddMmmDd](#DayDddMmmDd) | 示例为 周一 Sep 30, 周二 Oct 1 |
| [DayDddMmmDdYyy](#DayDddMmmDdYyy) | 示例为 周一 Sep 30 '02, 周二 Oct 1 '02 |
| [DayDddMmmmDd](#DayDddMmmmDd) | 示例为 周一 September 30, 周二 October 1 |
| [DayDddd](#DayDddd) | 示例为 星期二, 星期三。 |
| [DayDdi](#DayDdi) | 示例为 周一, 周二 |
| [DayDdiDd](#DayDdiDd) | 示例为 周一 30, 周二 1 |
| [DayDdiMDd](#DayDdiMDd) | 示例为 周一 S 30, 周二 O 1 |
| [DayDdiMmDd](#DayDdiMmDd) | 示例为 周一 9/30, 周二 10/1 |
| [DayDi](#DayDi) | 示例为 M, T |
| [DayDiDdNoSpace](#DayDiDdNoSpace) | 示例为 M30, T1 |
| [DayDiDdSpace](#DayDiDdSpace) | 示例为 M 30, T 1 |
| [DayDiMDd](#DayDiMDd) | 示例为 M S 30, T O 1 |
| [DayDiMmDd](#DayDiMmDd) | 示例为 M 9/30, T 10/1 |
| [DayFromEndDayDd](#DayFromEndDayDd) | 示例为 项目结束时的第 2 天, 第 1 天, 第 -1 天, 第 -2 天。 |
| [DayFromEndDd](#DayFromEndDd) | 示例为 2, 1, -1, -2 |
| [DayFromEndDdd](#DayFromEndDdd) | 示例为 D2, D1, D-1, D-2 |
| [DayFromStartDayDd](#DayFromStartDayDd) | 示例为 项目开始时的第 -2 天, 第 -1 天, 第 1 天, 第 2 天。 |
| [DayFromStartDd](#DayFromStartDd) | 示例为 -2, -1, 1, 2 |
| [DayFromStartDdd](#DayFromStartDdd) | 示例为 D-2, D-1, D1, D2 |
| [DayMDd](#DayMDd) | 示例为 S 30, O 1 |
| [DayMmDd](#DayMmDd) | 示例为 9/30, 10/1 |
| [DayMmDdYy](#DayMmDdYy) | 示例为 9/30/02, 10/1/02 |
| [DayMmmDd](#DayMmmDd) | 示例为 9月30日, 10月1日 |
| [DayMmmDdYyy](#DayMmmDdYyy) | 示例为 9月30日 '02, 10月10日 '02 |
| [DayOfMonthDd](#DayOfMonthDd) | 示例为 30, 1 |
| [DayOfYearDd](#DayOfYearDd) | 示例为 77, 78 |
| [DayOfYearDdYyy](#DayOfYearDdYyy) | 示例为 77 '10, 78 '10 |
| [DayOfYearDdYyyy](#DayOfYearDdYyyy) | 示例为 77 2010, 78 2010 |
| [HalfYearFromEndH](#HalfYearFromEndH) | 示例为 2, 1, -1, -2. |
| [HalfYearFromEndHalfH](#HalfYearFromEndHalfH) | 示例为 第2, 第1, 第-1, 第-2 |
| [HalfYearFromEndHh](#HalfYearFromEndHh) | 示例为 H2, H1, H-1, H-2 |
| [HalfYearFromStartH](#HalfYearFromStartH) | 示例为 -2, -1, 1, 2. |
| [HalfYearFromStartHalfH](#HalfYearFromStartHalfH) | 示例为 第-2, 第-1, 第1, 第2 |
| [HalfYearFromStartHh](#HalfYearFromStartHh) | 示例为 H-2, H-1, H1, H2 |
| [HalfYearH](#HalfYearH) | 示例为 1, 2. |
| [HalfYearHHyy](#HalfYearHHyy) | 示例为 1H10, 2H10 |
| [HalfYearHh](#HalfYearHh) | 示例为 H1, H2 |
| [HalfYearHhYyy](#HalfYearHhYyy) | 示例为 H1 '10, H2 '10 |
| [HalfYearHhhHalf](#HalfYearHhhHalf) | 示例为 第1半, 第2半 |
| [HalfYearHlfH](#HalfYearHlfH) | 示例为 第1, 第2 |
| [HalfYearHlfHYyyy](#HalfYearHlfHYyyy) | 示例为 第1, 2010; 第2, 2010 |
| [HourDddMmmDdHhAm](#HourDddMmmDdHhAm) | 示例为 周三 3月18日, 8 AM; 周三 3月18日, 9 AM. |
| [HourFromEndHh](#HourFromEndHh) | 示例为项目结束前的 3、2、1、-1、-2 小时。 |
| [HourFromEndHhh](#HourFromEndHhh) | 示例为 H3、H2、H1、H-1、H-2。 |
| [HourFromEndHourHh](#HourFromEndHourHh) | 示例为 第3小时、第2小时、第1小时、第-1小时、第-2小时。 |
| [HourFromStartHh](#HourFromStartHh) | 示例为项目开始后-2、-1、1、2、3 小时。 |
| [HourFromStartHhh](#HourFromStartHhh) | 示例为 H-2、H-1、H1、H2、H3。 |
| [HourFromStartHourHh](#HourFromStartHourHh) | 示例为 第-2小时、第-1小时、第1小时、第2小时、第3小时。 |
| [HourHh](#HourHh) | 示例为 8、9、10、11。 |
| [HourHhAm](#HourHhAm) | 示例为 8AM、9AM。 |
| [HourHhMmAm](#HourHhMmAm) | 示例为 8:00 AM、9:00 AM。 |
| [HourMmDdHhAm](#HourMmDdHhAm) | 示例为 3/18 8 AM、3/18 9 AM。 |
| [HourMmmDdHhAm](#HourMmmDdHhAm) | 示例为 Mar 18, 8 AM; Mar 18, 9 AM。 |
| [MinuteFromEndMinuteMm](#MinuteFromEndMinuteMm) | 示例为项目结束前的 Minute 181、Minute 180、...、Minute 1、Minute -1。 |
| [MinuteFromEndMm](#MinuteFromEndMm) | 示例为 181、180、...、1、-1。 |
| [MinuteFromEndMmm](#MinuteFromEndMmm) | 示例为 M181、M180、...、M1、M-1。 |
| [MinuteFromStartMinuteMm](#MinuteFromStartMinuteMm) | 示例为 Minute -2、Minute -1、Minute 1、...。 |
| [MinuteFromStartMm](#MinuteFromStartMm) | 示例为 -2、-1、1、...、180。 |
| [MinuteFromStartMmm](#MinuteFromStartMmm) | 示例为 M-2、M-1、M1、...、M180。 |
| [MinuteHhMmAm](#MinuteHhMmAm) | 示例为 8:00 AM、8:01 AM、8:02 AM。 |
| [MinuteMm](#MinuteMm) | 示例为 0、1、2、...、59 分钟。 |
| [MonthFromEndMm](#MonthFromEndMm) | 示例为项目结束前的 2、1、-1、-2 个月。 |
| [MonthFromEndMmm](#MonthFromEndMmm) | 示例为 M2、M1、M-1、M-2。 |
| [MonthFromEndMonthMm](#MonthFromEndMonthMm) | 示例为 Month 2、Month 1、Month -1、Month -2。 |
| [MonthFromStartMm](#MonthFromStartMm) | 示例为项目开始后-2、-2、1、2 个月。 |
| [MonthFromStartMmm](#MonthFromStartMmm) | 示例为 M-2、M-1、M1、M2。 |
| [MonthFromStartMonthMm](#MonthFromStartMonthMm) | 示例为 Month -2、Month -1、Month 1、Month 2。 |
| [MonthM](#MonthM) | 示例为 M, A, M, J, J. |
| [MonthMm](#MonthMm) | 示例为 11, 12, 1, 2 |
| [MonthMmYy](#MonthMmYy) | 示例为 3/10, 4/10, 5/10 |
| [MonthMmYyy](#MonthMmYyy) | 示例为 3 '10, 4 '10, 5 '10 |
| [MonthMmm](#MonthMmm) | 示例为 Mar, Apr, May |
| [MonthMmmYyy](#MonthMmmYyy) | 示例为 Mar '10, Apr '10, May '10 |
| [MonthMmmm](#MonthMmmm) | 示例为 March, April, May |
| [MonthMmmmYyyy](#MonthMmmmYyyy) | 示例为 March 2010, April 2010, May 2010 |
| [None](#None) | 未显示日期。 |
| [QuarterFromEndQ](#QuarterFromEndQ) | 示例为 项目结束后 5, 4, 3, 2, 1, -1 季度。 |
| [QuarterFromEndQq](#QuarterFromEndQq) | 示例为 Q5, Q4, Q3, Q2, Q1, Q-1 |
| [QuarterFromEndQuarterQ](#QuarterFromEndQuarterQ) | 示例为 第5季度, 第4季度, 第3季度, 第2季度, 第1季度, 第-1季度 |
| [QuarterFromStartQ](#QuarterFromStartQ) | 示例为 项目开始后 -5, -4, -3, -2, -1, 1 季度。 |
| [QuarterFromStartQq](#QuarterFromStartQq) | 示例为 Q-5, Q-4, Q-3, Q-2, Q-1, Q1 |
| [QuarterFromStartQuarterQ](#QuarterFromStartQuarterQ) | 示例为 第-5季度, 第-4季度, 第-3季度, 第-2季度, 第-1季度, 第1季度 |
| [QuarterQ](#QuarterQ) | 示例为 3, 4, 1. |
| [QuarterQQyy](#QuarterQQyy) | 示例为 3Q10, 4Q10, 1Q11 |
| [QuarterQq](#QuarterQq) | 示例为 Q3, Q4, Q1 |
| [QuarterQqYyy](#QuarterQqYyy) | 示例为 Q3 '10, Q4 '10, Q1 '11 |
| [QuarterQqqQuarter](#QuarterQqqQuarter) | 示例为 第3季度, 第1季度 |
| [QuarterQtrQ](#QuarterQtrQ) | 示例为 Qtr3, Qtr4, Qtr1 |
| [QuarterQtrQYyyy](#QuarterQtrQYyyy) | 示例为 Qtr3, 2010; Qtr4, 2010; Qtr1, 2011 |
| [ThirdsOfMonthsDd](#ThirdsOfMonthsDd) | 示例为 1, 11, 21, 1. |
| [ThirdsOfMonthsDdd](#ThirdsOfMonthsDdd) | 示例为 B, M, E, B |
| [ThirdsOfMonthsDddd](#ThirdsOfMonthsDddd) | 示例为 开始, 中间, 结束, 开始 |
| [ThirdsOfMonthsMmDd](#ThirdsOfMonthsMmDd) | 示例是 3/1。 |
| [ThirdsOfMonthsMmDdYy](#ThirdsOfMonthsMmDdYy) | 示例是 3/1/10。 |
| [ThirdsOfMonthsMmDdd](#ThirdsOfMonthsMmDdd) | 示例是 3/B、3/M、3/E、4/B |
| [ThirdsOfMonthsMmDddYy](#ThirdsOfMonthsMmDddYy) | 示例是 3/B/10。 |
| [ThirdsOfMonthsMmmDd](#ThirdsOfMonthsMmmDd) | 示例是 3月 1、3月 11、3月 21、4月 1 |
| [ThirdsOfMonthsMmmDdYy](#ThirdsOfMonthsMmmDdYy) | 示例是 3月 1、'10；3月 11、'10；3月 21、'10；4月 1、10 |
| [ThirdsOfMonthsMmmDdd](#ThirdsOfMonthsMmmDdd) | 示例是 3月 B、3月 M、3月 E、4月 B |
| [ThirdsOfMonthsMmmDddYy](#ThirdsOfMonthsMmmDddYy) | 示例是 3月 B、'10；3月 M、'10；3月 E、'10；4月 B '10 |
| [ThirdsOfMonthsMmmmDd](#ThirdsOfMonthsMmmmDd) | 示例是 三月 1、三月 11、三月 21、四月 1 |
| [ThirdsOfMonthsMmmmDdYyyy](#ThirdsOfMonthsMmmmDdYyyy) | 示例是 三月 1、2010；三月 11、2010；三月 21、2010；四月 1、2010 |
| [ThirdsOfMonthsMmmmDddd](#ThirdsOfMonthsMmmmDddd) | 示例是 三月 开始、三月 中部、三月 结束、四月 开始 |
| [ThirdsOfMonthsMmmmDdddYyyy](#ThirdsOfMonthsMmmmDdddYyyy) | 示例是 三月 开始、2010；三月 中部、2010；三月 结束、2010；四月 开始、2010 |
| [WeekDayOfMonthDd](#WeekDayOfMonthDd) | 示例是 21、28、4 |
| [WeekDddDd](#WeekDddDd) | 示例是 星期日 21、星期日 28、星期日 4。 |
| [WeekDddMDd](#WeekDddMDd) | 示例是 星期日 M 21、星期日 M 28、星期日 A 4 |
| [WeekDddMmDd](#WeekDddMmDd) | 示例是 星期日 3/21、星期日 3/28、星期日 4/4 |
| [WeekDddMmDdYy](#WeekDddMmDdYy) | 示例是 星期日 3/21/10、星期日 3/28/10、星期日 4/4/10 |
| [WeekDddMmmDd](#WeekDddMmmDd) | 示例是 星期日 3月 21、星期日 3月 28、星期日 4月 4 |
| [WeekDddMmmDdYyy](#WeekDddMmmDdYyy) | 示例是 星期日 3月 21、'10；星期日 3月 28、'10；星期日 4月 4、'10 |
| [WeekDddMmmmDd](#WeekDddMmmmDd) | 示例是 星期日 3月 21、星期日 三月 28、星期日 4月 4 |
| [WeekDddMmmmDdYyy](#WeekDddMmmmDdYyy) | 示例是 星期日 三月 21、'10；星期日 三月 28、'10；星期日 四月 4、'10 |
| [WeekDddWw](#WeekDddWw) | 示例是 星期日 12、星期日 13、星期日 14 |
| [WeekDdiMDd](#WeekDdiMDd) | 示例是 星期日 M 21、星期日 M 28、星期日 A 4 |
| [WeekDdiMmDd](#WeekDdiMmDd) | 示例是 星期日 3/21。 |
| [WeekDdiMmmDd](#WeekDdiMmmDd) | 示例是 星期日 3月 21、星期日 3月 28、星期日 4月 4 |
| [WeekDiMDd](#WeekDiMDd) | 示例为 S M 21, S M 28, S A 4 |
| [WeekDiMmDd](#WeekDiMmDd) | 示例为 S 3/21, S 3/28, S 4/4 |
| [WeekDiMmmDd](#WeekDiMmmDd) | 示例为 S Mar 21, S Mar 28, S Apr 4 |
| [WeekFromEndWeekWw](#WeekFromEndWeekWw) | 示例为项目结束时的 Week 2, Week 1, Week -1。 |
| [WeekFromEndWw](#WeekFromEndWw) | 示例为 2, 1, -1 |
| [WeekFromEndWww](#WeekFromEndWww) | 示例为 W2, W1, W-1 |
| [WeekFromStartWeekWw](#WeekFromStartWeekWw) | 示例为项目开始时的 Week -1, Week 1, Week 2。 |
| [WeekFromStartWw](#WeekFromStartWw) | 示例为 -1, 1, 2 |
| [WeekFromStartWww](#WeekFromStartWww) | 示例为 W-1, W1, W2 |
| [WeekMDd](#WeekMDd) | 示例为 M21, M28, A 4 |
| [WeekMmDd](#WeekMmDd) | 示例为 3/21, 3/28, 4/4 |
| [WeekMmDdYy](#WeekMmDdYy) | 示例为 '3/21/10'。 |
| [WeekMmmDd](#WeekMmmDd) | 示例为 Mar 21, Mar 28, Apr 4 |
| [WeekMmmDdYyy](#WeekMmmDdYyy) | 示例为 Mar 21, '10; Mar 28, '10; Apr 4, '10 |
| [WeekMmmmDd](#WeekMmmmDd) | 示例为 March 21, March 28, April 4 |
| [WeekMmmmDdYyyy](#WeekMmmmDdYyyy) | 示例为 March 21, 2010; March 28, 2010; April 4, 2010 |
| [WeekNumberDdWw](#WeekNumberDdWw) | 示例为 1 12, 1 13, 1 14（第 12 周的第 1 天，第 13 周的第 1 天，依此类推） |
| [WeekNumberWw](#WeekNumberWw) | 示例为 12, 13, 14 |
| [YearFromEndYearYy](#YearFromEndYearYy) | 示例为项目结束时的 Year 2, Year 1, Year -1。 |
| [YearFromEndYy](#YearFromEndYy) | 示例为 2, 1, -1 |
| [YearFromEndYyy](#YearFromEndYyy) | 示例为 Y2, Y1, Y-1 |
| [YearFromStartYearYy](#YearFromStartYearYy) | 示例为项目开始时的 Year -1, Year 1, Year 2。 |
| [YearFromStartYy](#YearFromStartYy) | 示例为 -1, 1, 2 |
| [YearFromStartYyy](#YearFromStartYyy) | 示例为 Y-1, Y1, Y2 |
| [YearYy](#YearYy) | 示例为 10, 11, 12。 |
| [YearYyy](#YearYyy) | 示例为 '10, '11, '12 |
| [YearYyyy](#YearYyyy) | 示例为 2010, 2011, 2012 |
### DayDdMmYyyy {#DayDdMmYyyy}
```
public static final int DayDdMmYyyy
```


示例为 19/07/2016。

### DayDdd {#DayDdd}
```
public static final int DayDdd
```


示例为 周一, 周二。

### DayDddDd {#DayDddDd}
```
public static final int DayDddDd
```


示例为 周一 30, 周二 1

### DayDddMDd {#DayDddMDd}
```
public static final int DayDddMDd
```


示例为 周一 S 30, 周二 O 1

### DayDddMmDd {#DayDddMmDd}
```
public static final int DayDddMmDd
```


示例为 周一 9/30, 周二 10/1

### DayDddMmDdYy {#DayDddMmDdYy}
```
public static final int DayDddMmDdYy
```


示例为 周一 9/30/02, 周二 10/1/02

### DayDddMmmDd {#DayDddMmmDd}
```
public static final int DayDddMmmDd
```


示例为 周一 Sep 30, 周二 Oct 1

### DayDddMmmDdYyy {#DayDddMmmDdYyy}
```
public static final int DayDddMmmDdYyy
```


示例为 周一 Sep 30 '02, 周二 Oct 1 '02

### DayDddMmmmDd {#DayDddMmmmDd}
```
public static final int DayDddMmmmDd
```


示例为 周一 September 30, 周二 October 1

### DayDddd {#DayDddd}
```
public static final int DayDddd
```


示例为 星期二, 星期三。

### DayDdi {#DayDdi}
```
public static final int DayDdi
```


示例为 周一, 周二

### DayDdiDd {#DayDdiDd}
```
public static final int DayDdiDd
```


示例为 周一 30, 周二 1

### DayDdiMDd {#DayDdiMDd}
```
public static final int DayDdiMDd
```


示例为 周一 S 30, 周二 O 1

### DayDdiMmDd {#DayDdiMmDd}
```
public static final int DayDdiMmDd
```


示例为 周一 9/30, 周二 10/1

### DayDi {#DayDi}
```
public static final int DayDi
```


示例为 M, T

### DayDiDdNoSpace {#DayDiDdNoSpace}
```
public static final int DayDiDdNoSpace
```


示例为 M30, T1

### DayDiDdSpace {#DayDiDdSpace}
```
public static final int DayDiDdSpace
```


示例为 M 30, T 1

### DayDiMDd {#DayDiMDd}
```
public static final int DayDiMDd
```


示例为 M S 30, T O 1

### DayDiMmDd {#DayDiMmDd}
```
public static final int DayDiMmDd
```


示例为 M 9/30, T 10/1

### DayFromEndDayDd {#DayFromEndDayDd}
```
public static final int DayFromEndDayDd
```


示例为 项目结束时的第 2 天, 第 1 天, 第 -1 天, 第 -2 天。

### DayFromEndDd {#DayFromEndDd}
```
public static final int DayFromEndDd
```


示例为 2, 1, -1, -2

### DayFromEndDdd {#DayFromEndDdd}
```
public static final int DayFromEndDdd
```


示例为 D2, D1, D-1, D-2

### DayFromStartDayDd {#DayFromStartDayDd}
```
public static final int DayFromStartDayDd
```


示例为 项目开始时的第 -2 天, 第 -1 天, 第 1 天, 第 2 天。

### DayFromStartDd {#DayFromStartDd}
```
public static final int DayFromStartDd
```


示例为 -2, -1, 1, 2

### DayFromStartDdd {#DayFromStartDdd}
```
public static final int DayFromStartDdd
```


示例为 D-2, D-1, D1, D2

### DayMDd {#DayMDd}
```
public static final int DayMDd
```


示例为 S 30, O 1

### DayMmDd {#DayMmDd}
```
public static final int DayMmDd
```


示例为 9/30, 10/1

### DayMmDdYy {#DayMmDdYy}
```
public static final int DayMmDdYy
```


示例为 9/30/02, 10/1/02

### DayMmmDd {#DayMmmDd}
```
public static final int DayMmmDd
```


示例为 9月30日, 10月1日

### DayMmmDdYyy {#DayMmmDdYyy}
```
public static final int DayMmmDdYyy
```


示例为 9月30日 '02, 10月10日 '02

### DayOfMonthDd {#DayOfMonthDd}
```
public static final int DayOfMonthDd
```


示例为 30, 1

### DayOfYearDd {#DayOfYearDd}
```
public static final int DayOfYearDd
```


示例为 77, 78

### DayOfYearDdYyy {#DayOfYearDdYyy}
```
public static final int DayOfYearDdYyy
```


示例为 77 '10, 78 '10

### DayOfYearDdYyyy {#DayOfYearDdYyyy}
```
public static final int DayOfYearDdYyyy
```


示例为 77 2010, 78 2010

### HalfYearFromEndH {#HalfYearFromEndH}
```
public static final int HalfYearFromEndH
```


示例为 2、1、-1、-2。项目结束日期起的半年。

### HalfYearFromEndHalfH {#HalfYearFromEndHalfH}
```
public static final int HalfYearFromEndHalfH
```


示例为 第2, 第1, 第-1, 第-2

### HalfYearFromEndHh {#HalfYearFromEndHh}
```
public static final int HalfYearFromEndHh
```


示例为 H2, H1, H-1, H-2

### HalfYearFromStartH {#HalfYearFromStartH}
```
public static final int HalfYearFromStartH
```


示例为 -2、-1、1、2。项目开始日期起的半年。

### HalfYearFromStartHalfH {#HalfYearFromStartHalfH}
```
public static final int HalfYearFromStartHalfH
```


示例为 第-2, 第-1, 第1, 第2

### HalfYearFromStartHh {#HalfYearFromStartHh}
```
public static final int HalfYearFromStartHh
```


示例为 H-2, H-1, H1, H2

### HalfYearH {#HalfYearH}
```
public static final int HalfYearH
```


示例为 1、2。要求时间单位为 TimescaleHalfYears。

### HalfYearHHyy {#HalfYearHHyy}
```
public static final int HalfYearHHyy
```


示例为 1H10, 2H10

### HalfYearHh {#HalfYearHh}
```
public static final int HalfYearHh
```


示例为 H1, H2

### HalfYearHhYyy {#HalfYearHhYyy}
```
public static final int HalfYearHhYyy
```


示例为 H1 '10, H2 '10

### HalfYearHhhHalf {#HalfYearHhhHalf}
```
public static final int HalfYearHhhHalf
```


示例为 第1半, 第2半

### HalfYearHlfH {#HalfYearHlfH}
```
public static final int HalfYearHlfH
```


示例为 第1, 第2

### HalfYearHlfHYyyy {#HalfYearHlfHYyyy}
```
public static final int HalfYearHlfHYyyy
```


示例为 第1, 2010; 第2, 2010

### HourDddMmmDdHhAm {#HourDddMmmDdHhAm}
```
public static final int HourDddMmmDdHhAm
```


示例为 Wed Mar 18，上午 8 点；Wed Mar 18，上午 9 点。要求时间单位为 TimescaleHours。

### HourFromEndHh {#HourFromEndHh}
```
public static final int HourFromEndHh
```


示例为项目结束前的 3、2、1、-1、-2 小时。

### HourFromEndHhh {#HourFromEndHhh}
```
public static final int HourFromEndHhh
```


示例为 H3、H2、H1、H-1、H-2。

### HourFromEndHourHh {#HourFromEndHourHh}
```
public static final int HourFromEndHourHh
```


示例为 第3小时、第2小时、第1小时、第-1小时、第-2小时。

### HourFromStartHh {#HourFromStartHh}
```
public static final int HourFromStartHh
```


示例为项目开始后-2、-1、1、2、3 小时。

### HourFromStartHhh {#HourFromStartHhh}
```
public static final int HourFromStartHhh
```


示例为 H-2、H-1、H1、H2、H3。

### HourFromStartHourHh {#HourFromStartHourHh}
```
public static final int HourFromStartHourHh
```


示例为 第-2小时、第-1小时、第1小时、第2小时、第3小时。

### HourHh {#HourHh}
```
public static final int HourHh
```


示例为 8、9、10、11。

### HourHhAm {#HourHhAm}
```
public static final int HourHhAm
```


示例为 8AM、9AM。

### HourHhMmAm {#HourHhMmAm}
```
public static final int HourHhMmAm
```


示例为 8:00 AM、9:00 AM。

### HourMmDdHhAm {#HourMmDdHhAm}
```
public static final int HourMmDdHhAm
```


示例为 3/18 8 AM、3/18 9 AM。

### HourMmmDdHhAm {#HourMmmDdHhAm}
```
public static final int HourMmmDdHhAm
```


示例为 Mar 18, 8 AM; Mar 18, 9 AM。

### MinuteFromEndMinuteMm {#MinuteFromEndMinuteMm}
```
public static final int MinuteFromEndMinuteMm
```


示例为项目结束前的 Minute 181、Minute 180、...、Minute 1、Minute -1。

### MinuteFromEndMm {#MinuteFromEndMm}
```
public static final int MinuteFromEndMm
```


示例为 181、180、...、1、-1。

### MinuteFromEndMmm {#MinuteFromEndMmm}
```
public static final int MinuteFromEndMmm
```


示例为 M181、M180、...、M1、M-1。

### MinuteFromStartMinuteMm {#MinuteFromStartMinuteMm}
```
public static final int MinuteFromStartMinuteMm
```


示例为 Minute -2、Minute -1、Minute 1、... Minute 180（项目开始时）。

### MinuteFromStartMm {#MinuteFromStartMm}
```
public static final int MinuteFromStartMm
```


示例为 -2、-1、1、...、180。

### MinuteFromStartMmm {#MinuteFromStartMmm}
```
public static final int MinuteFromStartMmm
```


示例为 M-2、M-1、M1、...、M180。

### MinuteHhMmAm {#MinuteHhMmAm}
```
public static final int MinuteHhMmAm
```


示例为 8:00 AM、8:01 AM、8:02 AM。要求时间单位为 TimescaleMinutes。

### MinuteMm {#MinuteMm}
```
public static final int MinuteMm
```


示例为 0、1、2、...、59 分钟。

### MonthFromEndMm {#MonthFromEndMm}
```
public static final int MonthFromEndMm
```


示例为项目结束前的 2、1、-1、-2 个月。

### MonthFromEndMmm {#MonthFromEndMmm}
```
public static final int MonthFromEndMmm
```


示例为 M2、M1、M-1、M-2。

### MonthFromEndMonthMm {#MonthFromEndMonthMm}
```
public static final int MonthFromEndMonthMm
```


示例为 Month 2、Month 1、Month -1、Month -2。

### MonthFromStartMm {#MonthFromStartMm}
```
public static final int MonthFromStartMm
```


示例为项目开始后-2、-2、1、2 个月。

### MonthFromStartMmm {#MonthFromStartMmm}
```
public static final int MonthFromStartMmm
```


示例为 M-2、M-1、M1、M2。

### MonthFromStartMonthMm {#MonthFromStartMonthMm}
```
public static final int MonthFromStartMonthMm
```


示例为 Month -2、Month -1、Month 1、Month 2。

### MonthM {#MonthM}
```
public static final int MonthM
```


示例为 M、A、M、J、J。要求时间单位为 TimescaleMonths。

### MonthMm {#MonthMm}
```
public static final int MonthMm
```


示例为 11, 12, 1, 2

### MonthMmYy {#MonthMmYy}
```
public static final int MonthMmYy
```


示例为 3/10, 4/10, 5/10

### MonthMmYyy {#MonthMmYyy}
```
public static final int MonthMmYyy
```


示例为 3 '10, 4 '10, 5 '10

### MonthMmm {#MonthMmm}
```
public static final int MonthMmm
```


示例为 Mar, Apr, May

### MonthMmmYyy {#MonthMmmYyy}
```
public static final int MonthMmmYyy
```


示例为 Mar '10, Apr '10, May '10

### MonthMmmm {#MonthMmmm}
```
public static final int MonthMmmm
```


示例为 March, April, May

### MonthMmmmYyyy {#MonthMmmmYyyy}
```
public static final int MonthMmmmYyyy
```


示例为 March 2010, April 2010, May 2010

### None {#None}
```
public static final int None
```


未显示日期。

### QuarterFromEndQ {#QuarterFromEndQ}
```
public static final int QuarterFromEndQ
```


示例为 项目结束后 5, 4, 3, 2, 1, -1 季度。

### QuarterFromEndQq {#QuarterFromEndQq}
```
public static final int QuarterFromEndQq
```


示例为 Q5, Q4, Q3, Q2, Q1, Q-1

### QuarterFromEndQuarterQ {#QuarterFromEndQuarterQ}
```
public static final int QuarterFromEndQuarterQ
```


示例为 第5季度, 第4季度, 第3季度, 第2季度, 第1季度, 第-1季度

### QuarterFromStartQ {#QuarterFromStartQ}
```
public static final int QuarterFromStartQ
```


示例为 项目开始后 -5, -4, -3, -2, -1, 1 季度。

### QuarterFromStartQq {#QuarterFromStartQq}
```
public static final int QuarterFromStartQq
```


示例为 Q-5, Q-4, Q-3, Q-2, Q-1, Q1

### QuarterFromStartQuarterQ {#QuarterFromStartQuarterQ}
```
public static final int QuarterFromStartQuarterQ
```


示例为 第-5季度, 第-4季度, 第-3季度, 第-2季度, 第-1季度, 第1季度

### QuarterQ {#QuarterQ}
```
public static final int QuarterQ
```


示例为 3、4、1。要求时间单位为 TimescaleQuarters。

### QuarterQQyy {#QuarterQQyy}
```
public static final int QuarterQQyy
```


示例为 3Q10, 4Q10, 1Q11

### QuarterQq {#QuarterQq}
```
public static final int QuarterQq
```


示例为 Q3, Q4, Q1

### QuarterQqYyy {#QuarterQqYyy}
```
public static final int QuarterQqYyy
```


示例为 Q3 '10, Q4 '10, Q1 '11

### QuarterQqqQuarter {#QuarterQqqQuarter}
```
public static final int QuarterQqqQuarter
```


示例为 第3季度, 第1季度

### QuarterQtrQ {#QuarterQtrQ}
```
public static final int QuarterQtrQ
```


示例为 Qtr3, Qtr4, Qtr1

### QuarterQtrQYyyy {#QuarterQtrQYyyy}
```
public static final int QuarterQtrQYyyy
```


示例为 Qtr3, 2010; Qtr4, 2010; Qtr1, 2011

### ThirdsOfMonthsDd {#ThirdsOfMonthsDd}
```
public static final int ThirdsOfMonthsDd
```


示例为 1、11、21、1。要求时间单位为 TimescaleThirdsOfMonths。

### ThirdsOfMonthsDdd {#ThirdsOfMonthsDdd}
```
public static final int ThirdsOfMonthsDdd
```


示例为 B, M, E, B

### ThirdsOfMonthsDddd {#ThirdsOfMonthsDddd}
```
public static final int ThirdsOfMonthsDddd
```


示例为 开始, 中间, 结束, 开始

### ThirdsOfMonthsMmDd {#ThirdsOfMonthsMmDd}
```
public static final int ThirdsOfMonthsMmDd
```


示例是 3/1。

### ThirdsOfMonthsMmDdYy {#ThirdsOfMonthsMmDdYy}
```
public static final int ThirdsOfMonthsMmDdYy
```


示例是 3/1/10。

### ThirdsOfMonthsMmDdd {#ThirdsOfMonthsMmDdd}
```
public static final int ThirdsOfMonthsMmDdd
```


示例是 3/B、3/M、3/E、4/B

### ThirdsOfMonthsMmDddYy {#ThirdsOfMonthsMmDddYy}
```
public static final int ThirdsOfMonthsMmDddYy
```


示例是 3/B/10。

### ThirdsOfMonthsMmmDd {#ThirdsOfMonthsMmmDd}
```
public static final int ThirdsOfMonthsMmmDd
```


示例是 3月 1、3月 11、3月 21、4月 1

### ThirdsOfMonthsMmmDdYy {#ThirdsOfMonthsMmmDdYy}
```
public static final int ThirdsOfMonthsMmmDdYy
```


示例是 3月 1、'10；3月 11、'10；3月 21、'10；4月 1、10

### ThirdsOfMonthsMmmDdd {#ThirdsOfMonthsMmmDdd}
```
public static final int ThirdsOfMonthsMmmDdd
```


示例是 3月 B、3月 M、3月 E、4月 B

### ThirdsOfMonthsMmmDddYy {#ThirdsOfMonthsMmmDddYy}
```
public static final int ThirdsOfMonthsMmmDddYy
```


示例是 3月 B、'10；3月 M、'10；3月 E、'10；4月 B '10

### ThirdsOfMonthsMmmmDd {#ThirdsOfMonthsMmmmDd}
```
public static final int ThirdsOfMonthsMmmmDd
```


示例是 三月 1、三月 11、三月 21、四月 1

### ThirdsOfMonthsMmmmDdYyyy {#ThirdsOfMonthsMmmmDdYyyy}
```
public static final int ThirdsOfMonthsMmmmDdYyyy
```


示例是 三月 1、2010；三月 11、2010；三月 21、2010；四月 1、2010

### ThirdsOfMonthsMmmmDddd {#ThirdsOfMonthsMmmmDddd}
```
public static final int ThirdsOfMonthsMmmmDddd
```


示例是 三月 开始、三月 中部、三月 结束、四月 开始

### ThirdsOfMonthsMmmmDdddYyyy {#ThirdsOfMonthsMmmmDdddYyyy}
```
public static final int ThirdsOfMonthsMmmmDdddYyyy
```


示例是 三月 开始、2010；三月 中部、2010；三月 结束、2010；四月 开始、2010

### WeekDayOfMonthDd {#WeekDayOfMonthDd}
```
public static final int WeekDayOfMonthDd
```


示例是 21、28、4

### WeekDddDd {#WeekDddDd}
```
public static final int WeekDddDd
```


示例为 Sun 21、Sun 28、Sun 4。要求时间单位为 TimescaleWeeks。

### WeekDddMDd {#WeekDddMDd}
```
public static final int WeekDddMDd
```


示例是 星期日 M 21、星期日 M 28、星期日 A 4

### WeekDddMmDd {#WeekDddMmDd}
```
public static final int WeekDddMmDd
```


示例是 星期日 3/21、星期日 3/28、星期日 4/4

### WeekDddMmDdYy {#WeekDddMmDdYy}
```
public static final int WeekDddMmDdYy
```


示例是 星期日 3/21/10、星期日 3/28/10、星期日 4/4/10

### WeekDddMmmDd {#WeekDddMmmDd}
```
public static final int WeekDddMmmDd
```


示例是 星期日 3月 21、星期日 3月 28、星期日 4月 4

### WeekDddMmmDdYyy {#WeekDddMmmDdYyy}
```
public static final int WeekDddMmmDdYyy
```


示例是 星期日 3月 21、'10；星期日 3月 28、'10；星期日 4月 4、'10

### WeekDddMmmmDd {#WeekDddMmmmDd}
```
public static final int WeekDddMmmmDd
```


示例是 星期日 3月 21、星期日 三月 28、星期日 4月 4

### WeekDddMmmmDdYyy {#WeekDddMmmmDdYyy}
```
public static final int WeekDddMmmmDdYyy
```


示例是 星期日 三月 21、'10；星期日 三月 28、'10；星期日 四月 4、'10

### WeekDddWw {#WeekDddWw}
```
public static final int WeekDddWw
```


示例是 星期日 12、星期日 13、星期日 14

### WeekDdiMDd {#WeekDdiMDd}
```
public static final int WeekDdiMDd
```


示例是 星期日 M 21、星期日 M 28、星期日 A 4

### WeekDdiMmDd {#WeekDdiMmDd}
```
public static final int WeekDdiMmDd
```


示例为 Su 3/21、Su 3/28、Su 4/4

### WeekDdiMmmDd {#WeekDdiMmmDd}
```
public static final int WeekDdiMmmDd
```


示例是 星期日 3月 21、星期日 3月 28、星期日 4月 4

### WeekDiMDd {#WeekDiMDd}
```
public static final int WeekDiMDd
```


示例为 S M 21, S M 28, S A 4

### WeekDiMmDd {#WeekDiMmDd}
```
public static final int WeekDiMmDd
```


示例为 S 3/21, S 3/28, S 4/4

### WeekDiMmmDd {#WeekDiMmmDd}
```
public static final int WeekDiMmmDd
```


示例为 S Mar 21, S Mar 28, S Apr 4

### WeekFromEndWeekWw {#WeekFromEndWeekWw}
```
public static final int WeekFromEndWeekWw
```


示例为项目结束时的 Week 2, Week 1, Week -1。

### WeekFromEndWw {#WeekFromEndWw}
```
public static final int WeekFromEndWw
```


示例为 2, 1, -1

### WeekFromEndWww {#WeekFromEndWww}
```
public static final int WeekFromEndWww
```


示例为 W2, W1, W-1

### WeekFromStartWeekWw {#WeekFromStartWeekWw}
```
public static final int WeekFromStartWeekWw
```


示例为项目开始时的 Week -1, Week 1, Week 2。

### WeekFromStartWw {#WeekFromStartWw}
```
public static final int WeekFromStartWw
```


示例为 -1, 1, 2

### WeekFromStartWww {#WeekFromStartWww}
```
public static final int WeekFromStartWww
```


示例为 W-1, W1, W2

### WeekMDd {#WeekMDd}
```
public static final int WeekMDd
```


示例为 M21, M28, A 4

### WeekMmDd {#WeekMmDd}
```
public static final int WeekMmDd
```


示例为 3/21, 3/28, 4/4

### WeekMmDdYy {#WeekMmDdYy}
```
public static final int WeekMmDdYy
```


示例为 '3/21/10'。

### WeekMmmDd {#WeekMmmDd}
```
public static final int WeekMmmDd
```


示例为 Mar 21, Mar 28, Apr 4

### WeekMmmDdYyy {#WeekMmmDdYyy}
```
public static final int WeekMmmDdYyy
```


示例为 Mar 21, '10; Mar 28, '10; Apr 4, '10

### WeekMmmmDd {#WeekMmmmDd}
```
public static final int WeekMmmmDd
```


示例为 March 21, March 28, April 4

### WeekMmmmDdYyyy {#WeekMmmmDdYyyy}
```
public static final int WeekMmmmDdYyyy
```


示例为 March 21, 2010; March 28, 2010; April 4, 2010

### WeekNumberDdWw {#WeekNumberDdWw}
```
public static final int WeekNumberDdWw
```


示例为 1 12, 1 13, 1 14（第 12 周的第 1 天，第 13 周的第 1 天，依此类推）

### WeekNumberWw {#WeekNumberWw}
```
public static final int WeekNumberWw
```


示例为 12, 13, 14

### YearFromEndYearYy {#YearFromEndYearYy}
```
public static final int YearFromEndYearYy
```


示例为项目结束时的 Year 2, Year 1, Year -1。

### YearFromEndYy {#YearFromEndYy}
```
public static final int YearFromEndYy
```


示例为 2, 1, -1

### YearFromEndYyy {#YearFromEndYyy}
```
public static final int YearFromEndYyy
```


示例为 Y2, Y1, Y-1

### YearFromStartYearYy {#YearFromStartYearYy}
```
public static final int YearFromStartYearYy
```


示例为项目开始时的 Year -1, Year 1, Year 2。

### YearFromStartYy {#YearFromStartYy}
```
public static final int YearFromStartYy
```


示例为 -1, 1, 2

### YearFromStartYyy {#YearFromStartYyy}
```
public static final int YearFromStartYyy
```


示例为 Y-1, Y1, Y2

### YearYy {#YearYy}
```
public static final int YearYy
```


示例为 10、11、12。要求时间单位为 TimescaleYears。

### YearYyy {#YearYyy}
```
public static final int YearYyy
```


示例为 '10, '11, '12

### YearYyyy {#YearYyyy}
```
public static final int YearYyyy
```


示例为 2010, 2011, 2012

