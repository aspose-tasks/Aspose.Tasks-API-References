---
title: DateLabel
second_title: Aspose.Tasks for Java API Reference
description: Specifies the display format for date and time labels in a timescale.
type: docs
weight: 69
url: /java/com.aspose.tasks/datelabel/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class DateLabel extends System.Enum
```

Specifies the display format for date and time labels in a timescale.
## Fields

| Field | Description |
| --- | --- |
| [DayDdMmYyyy](#DayDdMmYyyy) | Example is 19/07/2016. |
| [DayDdd](#DayDdd) | Examples are Mon, Tue. |
| [DayDddDd](#DayDddDd) | Examples are Mon 30, Tue 1 |
| [DayDddMDd](#DayDddMDd) | Examples are Mon S 30, Tue O 1 |
| [DayDddMmDd](#DayDddMmDd) | Examples are Mon 9/30, Tue 10/1 |
| [DayDddMmDdYy](#DayDddMmDdYy) | Examples are Mon 9/30/02, Tue 10/1/02 |
| [DayDddMmmDd](#DayDddMmmDd) | Examples are Mon Sep 30, Tue Oct 1 |
| [DayDddMmmDdYyy](#DayDddMmmDdYyy) | Examples are Mon Sep 30 '02, Tue Oct 1 '02 |
| [DayDddMmmmDd](#DayDddMmmmDd) | Examples are Mon September 30, Tue October 1 |
| [DayDddd](#DayDddd) | Examples are Tuesday, Wednesday. |
| [DayDdi](#DayDdi) | Examples are Mo, Tu |
| [DayDdiDd](#DayDdiDd) | Examples are Mo 30, Tu 1 |
| [DayDdiMDd](#DayDdiMDd) | Examples are Mo S 30, Tu O 1 |
| [DayDdiMmDd](#DayDdiMmDd) | Examples are Mo 9/30, Tu 10/1 |
| [DayDi](#DayDi) | Examples are M, T |
| [DayDiDdNoSpace](#DayDiDdNoSpace) | Examples are M30, T1 |
| [DayDiDdSpace](#DayDiDdSpace) | Examples are M 30, T 1 |
| [DayDiMDd](#DayDiMDd) | Examples are M S 30, T O 1 |
| [DayDiMmDd](#DayDiMmDd) | Examples are M 9/30, T 10/1 |
| [DayFromEndDayDd](#DayFromEndDayDd) | Examples are Day 2, Day 1, Day -1, Day -2 from the project end. |
| [DayFromEndDd](#DayFromEndDd) | Examples are 2, 1, -1, -2 |
| [DayFromEndDdd](#DayFromEndDdd) | Examples are D2, D1, D-1, D-2 |
| [DayFromStartDayDd](#DayFromStartDayDd) | Examples are Day -2, Day -1, Day 1, Day 2 from the project start. |
| [DayFromStartDd](#DayFromStartDd) | Examples are -2, -1, 1, 2 |
| [DayFromStartDdd](#DayFromStartDdd) | Examples are D-2, D-1, D1, D2 |
| [DayMDd](#DayMDd) | Examples are S 30, O 1 |
| [DayMmDd](#DayMmDd) | Examples are 9/30, 10/1 |
| [DayMmDdYy](#DayMmDdYy) | Examples are 9/30/02, 10/1/02 |
| [DayMmmDd](#DayMmmDd) | Examples are Sep 30, Oct 1 |
| [DayMmmDdYyy](#DayMmmDdYyy) | Examples are Sep 30 '02, Oct 10 '02 |
| [DayOfMonthDd](#DayOfMonthDd) | Examples are 30, 1 |
| [DayOfYearDd](#DayOfYearDd) | Examples are 77, 78 |
| [DayOfYearDdYyy](#DayOfYearDdYyy) | Examples are 77 '10, 78 '10 |
| [DayOfYearDdYyyy](#DayOfYearDdYyyy) | Examples are 77 2010, 78 2010 |
| [HalfYearFromEndH](#HalfYearFromEndH) | Examples are 2, 1, -1, -2. |
| [HalfYearFromEndHalfH](#HalfYearFromEndHalfH) | Examples are Half 2, Half 1, Half -1, Half -2 |
| [HalfYearFromEndHh](#HalfYearFromEndHh) | Examples are H2, H1, H-1, H-2 |
| [HalfYearFromStartH](#HalfYearFromStartH) | Examples are -2, -1, 1, 2. |
| [HalfYearFromStartHalfH](#HalfYearFromStartHalfH) | Examples are Half -2, Half -1, Half 1, Half 2 |
| [HalfYearFromStartHh](#HalfYearFromStartHh) | Examples are H-2, H-1, H1, H2 |
| [HalfYearH](#HalfYearH) | Examples are 1, 2. |
| [HalfYearHHyy](#HalfYearHHyy) | Examples are 1H10, 2H10 |
| [HalfYearHh](#HalfYearHh) | Examples are H1, H2 |
| [HalfYearHhYyy](#HalfYearHhYyy) | Examples are H1 '10, H2 '10 |
| [HalfYearHhhHalf](#HalfYearHhhHalf) | Examples are 1st Half, 2d Half |
| [HalfYearHlfH](#HalfYearHlfH) | Examples are Half 1, Half 2 |
| [HalfYearHlfHYyyy](#HalfYearHlfHYyyy) | Examples are Half 1, 2010; Half 2, 2010 |
| [HourDddMmmDdHhAm](#HourDddMmmDdHhAm) | Examples are Wed Mar 18, 8 AM; Wed Mar 18, 9 AM. |
| [HourFromEndHh](#HourFromEndHh) | Examples are 3, 2, 1, -1, -2 hours from the project end. |
| [HourFromEndHhh](#HourFromEndHhh) | Examples are H3, H2, H1, H-1, H-2 |
| [HourFromEndHourHh](#HourFromEndHourHh) | Examples are Hour 3, Hour 2, Hour 1, Hour -1, Hour -2 |
| [HourFromStartHh](#HourFromStartHh) | Examples are -2, -1, 1, 2, 3 hours from the project start. |
| [HourFromStartHhh](#HourFromStartHhh) | Examples are H-2, H-1, H1, H2, H3 |
| [HourFromStartHourHh](#HourFromStartHourHh) | Examples are Hour -2, Hour -1, Hour 1, Hour 2, Hour 3 |
| [HourHh](#HourHh) | Examples are 8, 9, 10, 11 |
| [HourHhAm](#HourHhAm) | Examples are 8AM, 9AM |
| [HourHhMmAm](#HourHhMmAm) | Examples are 8:00 AM, 9:00 AM |
| [HourMmDdHhAm](#HourMmDdHhAm) | Examples are 3/18 8 AM, 3/18 9 AM |
| [HourMmmDdHhAm](#HourMmmDdHhAm) | Examples are Mar 18, 8 AM; Mar 18, 9 AM |
| [MinuteFromEndMinuteMm](#MinuteFromEndMinuteMm) | Examples are Minute 181, Minute 180, ..., Minute 1, Minute -1 from the project end. |
| [MinuteFromEndMm](#MinuteFromEndMm) | Examples are 181, 180, ..., 1, -1 |
| [MinuteFromEndMmm](#MinuteFromEndMmm) | Examples are M181, M180, ..., M1, M-1 |
| [MinuteFromStartMinuteMm](#MinuteFromStartMinuteMm) | Examples are Minute -2, Minute -1, Minute 1, ... |
| [MinuteFromStartMm](#MinuteFromStartMm) | Examples are -2, -1, 1, ..., 180 |
| [MinuteFromStartMmm](#MinuteFromStartMmm) | Examples are M-2, M-1, M1, ..., M180 |
| [MinuteHhMmAm](#MinuteHhMmAm) | Examples are 8:00 AM, 8:01 AM, 8:02 AM. |
| [MinuteMm](#MinuteMm) | Examples are 0, 1, 2, ..., 59 minutes |
| [MonthFromEndMm](#MonthFromEndMm) | Examples are 2, 1, -1, -2 months from the project end. |
| [MonthFromEndMmm](#MonthFromEndMmm) | Examples are M2, M1, M-1, M-2 |
| [MonthFromEndMonthMm](#MonthFromEndMonthMm) | Examples are Month 2, Month 1, Month -1, Month -2 |
| [MonthFromStartMm](#MonthFromStartMm) | Examples are -2, -2, 1, 2 months from the project start. |
| [MonthFromStartMmm](#MonthFromStartMmm) | Examples are M-2, M-1, M1, M2 |
| [MonthFromStartMonthMm](#MonthFromStartMonthMm) | Examples are Month -2, Month -1, Month 1, Month 2 |
| [MonthM](#MonthM) | Examples are M, A, M, J, J. |
| [MonthMm](#MonthMm) | Examples are 11, 12, 1, 2 |
| [MonthMmYy](#MonthMmYy) | Examples are 3/10, 4/10, 5/10 |
| [MonthMmYyy](#MonthMmYyy) | Examples are 3 '10, 4 '10, 5 '10 |
| [MonthMmm](#MonthMmm) | Examples are Mar, Apr, May |
| [MonthMmmYyy](#MonthMmmYyy) | Examples are Mar '10, Apr '10, May '10 |
| [MonthMmmm](#MonthMmmm) | Examples are March, April, May |
| [MonthMmmmYyyy](#MonthMmmmYyyy) | Examples are March 2010, April 2010, May 2010 |
| [None](#None) | No date is displayed. |
| [QuarterFromEndQ](#QuarterFromEndQ) | Examples are 5, 4, 3, 2, 1, -1 quarters from the project end. |
| [QuarterFromEndQq](#QuarterFromEndQq) | Examples are Q5, Q4, Q3, Q2, Q1, Q-1 |
| [QuarterFromEndQuarterQ](#QuarterFromEndQuarterQ) | Examples are Quarter 5, Quarter 4, Quarter 3, Quarter 2, Quarter 1, Quarter -1 |
| [QuarterFromStartQ](#QuarterFromStartQ) | Examples are -5, -4, -3, -2, -1, 1 quarters from the project start. |
| [QuarterFromStartQq](#QuarterFromStartQq) | Examples are Q-5, Q-4, Q-3, Q-2, Q-1, Q1 |
| [QuarterFromStartQuarterQ](#QuarterFromStartQuarterQ) | Examples are Quarter -5, Quarter -4, Quarter -3, Quarter -2, Quarter -1, Quarter 1 |
| [QuarterQ](#QuarterQ) | Examples are 3, 4, 1. |
| [QuarterQQyy](#QuarterQQyy) | Examples are 3Q10, 4Q10, 1Q11 |
| [QuarterQq](#QuarterQq) | Examples are Q3, Q4, Q1 |
| [QuarterQqYyy](#QuarterQqYyy) | Examples are Q3 '10, Q4 '10, Q1 '11 |
| [QuarterQqqQuarter](#QuarterQqqQuarter) | Examples are 3rd Quarter, 1st Quarter |
| [QuarterQtrQ](#QuarterQtrQ) | Examples are Qtr3, Qtr4, Qtr1 |
| [QuarterQtrQYyyy](#QuarterQtrQYyyy) | Examples are Qtr3, 2010; Qtr4, 2010; Qtr1, 2011 |
| [ThirdsOfMonthsDd](#ThirdsOfMonthsDd) | Examples are 1, 11, 21, 1. |
| [ThirdsOfMonthsDdd](#ThirdsOfMonthsDdd) | Examples are B, M, E, B |
| [ThirdsOfMonthsDddd](#ThirdsOfMonthsDddd) | Examples are Beginning, Middle, End, Beginning |
| [ThirdsOfMonthsMmDd](#ThirdsOfMonthsMmDd) | Example is 3/1. |
| [ThirdsOfMonthsMmDdYy](#ThirdsOfMonthsMmDdYy) | Example is 3/1/10. |
| [ThirdsOfMonthsMmDdd](#ThirdsOfMonthsMmDdd) | Examples are 3/B, 3/M, 3/E, 4/B |
| [ThirdsOfMonthsMmDddYy](#ThirdsOfMonthsMmDddYy) | Example is 3/B/10. |
| [ThirdsOfMonthsMmmDd](#ThirdsOfMonthsMmmDd) | Examples are Mar 1, Mar 11, Mar 21, Apr 1 |
| [ThirdsOfMonthsMmmDdYy](#ThirdsOfMonthsMmmDdYy) | Examples are Mar 1, '10; Mar 11, '10; Mar 21, '10; Apr 1, 10 |
| [ThirdsOfMonthsMmmDdd](#ThirdsOfMonthsMmmDdd) | Examples are Mar B, Mar M, Mar E, Apr B |
| [ThirdsOfMonthsMmmDddYy](#ThirdsOfMonthsMmmDddYy) | Examples are Mar B, '10; Mar M, '10; Mar E, '10; Apr B '10 |
| [ThirdsOfMonthsMmmmDd](#ThirdsOfMonthsMmmmDd) | Examples are March 1, March 11, March 21, April 1 |
| [ThirdsOfMonthsMmmmDdYyyy](#ThirdsOfMonthsMmmmDdYyyy) | Examples are March 1, 2010; March 11, 2010; March 21, 2010; April 1, 2010 |
| [ThirdsOfMonthsMmmmDddd](#ThirdsOfMonthsMmmmDddd) | Examples are March Beginning, March Middle, March End, April Beginning |
| [ThirdsOfMonthsMmmmDdddYyyy](#ThirdsOfMonthsMmmmDdddYyyy) | Examples are March Beginning, 2010; March Middle, 2010; March End, 2010; April Beginning, 2010 |
| [WeekDayOfMonthDd](#WeekDayOfMonthDd) | Examples are 21, 28, 4 |
| [WeekDddDd](#WeekDddDd) | Examples are Sun 21, Sun 28, Sun 4. |
| [WeekDddMDd](#WeekDddMDd) | Examples are Sun M 21, Sun M 28, Sun A 4 |
| [WeekDddMmDd](#WeekDddMmDd) | Examples are Sun 3/21, Sun 3/28, Sun 4/4 |
| [WeekDddMmDdYy](#WeekDddMmDdYy) | Examples are Sun 3/21/10, Sun 3/28/10, Sun 4/4/10 |
| [WeekDddMmmDd](#WeekDddMmmDd) | Examples are Sun Mar 21, Sun Mar 28, Sun Apr 4 |
| [WeekDddMmmDdYyy](#WeekDddMmmDdYyy) | Examples are Sun Mar 21, '10; Sun Mar 28, '10; Sun Apr 4, '10 |
| [WeekDddMmmmDd](#WeekDddMmmmDd) | Examples are Sun Mar 21, Sun March 28, Sun Apr 4 |
| [WeekDddMmmmDdYyy](#WeekDddMmmmDdYyy) | Examples are Sun March 21, '10; Sun March 28, '10; Sun April 4, '10 |
| [WeekDddWw](#WeekDddWw) | Examples are Sun 12, Sun 13, Sun 14 |
| [WeekDdiMDd](#WeekDdiMDd) | Examples are Su M 21, Su M 28, Su A 4 |
| [WeekDdiMmDd](#WeekDdiMmDd) | Examples are Su 3/21. |
| [WeekDdiMmmDd](#WeekDdiMmmDd) | Examples are Su Mar 21, Su Mar 28, Su Apr 4 |
| [WeekDiMDd](#WeekDiMDd) | Examples are S M 21, S M 28, S A 4 |
| [WeekDiMmDd](#WeekDiMmDd) | Examples are S 3/21, S 3/28, S 4/4 |
| [WeekDiMmmDd](#WeekDiMmmDd) | Examples are S Mar 21, S Mar 28, S Apr 4 |
| [WeekFromEndWeekWw](#WeekFromEndWeekWw) | Examples are Week 2, Week 1, Week -1 from the project end. |
| [WeekFromEndWw](#WeekFromEndWw) | Examples are 2, 1, -1 |
| [WeekFromEndWww](#WeekFromEndWww) | Examples are W2, W1, W-1 |
| [WeekFromStartWeekWw](#WeekFromStartWeekWw) | Examples are Week -1, Week 1, Week 2 from the project start. |
| [WeekFromStartWw](#WeekFromStartWw) | Examples are -1, 1, 2 |
| [WeekFromStartWww](#WeekFromStartWww) | Examples are W-1, W1, W2 |
| [WeekMDd](#WeekMDd) | Examples are M21, M28, A 4 |
| [WeekMmDd](#WeekMmDd) | Examples are 3/21, 3/28, 4/4 |
| [WeekMmDdYy](#WeekMmDdYy) | Example is '3/21/10'. |
| [WeekMmmDd](#WeekMmmDd) | Examples are Mar 21, Mar 28, Apr 4 |
| [WeekMmmDdYyy](#WeekMmmDdYyy) | Examples are Mar 21, '10; Mar 28, '10; Apr 4, '10 |
| [WeekMmmmDd](#WeekMmmmDd) | Examples are March 21, March 28, April 4 |
| [WeekMmmmDdYyyy](#WeekMmmmDdYyyy) | Examples are March 21, 2010; March 28, 2010; April 4, 2010 |
| [WeekNumberDdWw](#WeekNumberDdWw) | Examples are 1 12, 1 13, 1 14 (day 1 of week 12, day 1 of week 13, and so forth) |
| [WeekNumberWw](#WeekNumberWw) | Examples are 12, 13, 14 |
| [YearFromEndYearYy](#YearFromEndYearYy) | Examples are Year 2, Year 1, Year -1 from the project end. |
| [YearFromEndYy](#YearFromEndYy) | Examples are 2, 1, -1 |
| [YearFromEndYyy](#YearFromEndYyy) | Examples are Y2, Y1, Y-1 |
| [YearFromStartYearYy](#YearFromStartYearYy) | Examples are Year -1, Year 1, Year 2 from the project start. |
| [YearFromStartYy](#YearFromStartYy) | Examples are -1, 1, 2 |
| [YearFromStartYyy](#YearFromStartYyy) | Examples are Y-1, Y1, Y2 |
| [YearYy](#YearYy) | Examples are 10, 11, 12. |
| [YearYyy](#YearYyy) | Examples are '10, '11, '12 |
| [YearYyyy](#YearYyyy) | Examples are 2010, 2011, 2012 |
### DayDdMmYyyy {#DayDdMmYyyy}
```
public static final int DayDdMmYyyy
```


Example is 19/07/2016.

### DayDdd {#DayDdd}
```
public static final int DayDdd
```


Examples are Mon, Tue.

### DayDddDd {#DayDddDd}
```
public static final int DayDddDd
```


Examples are Mon 30, Tue 1

### DayDddMDd {#DayDddMDd}
```
public static final int DayDddMDd
```


Examples are Mon S 30, Tue O 1

### DayDddMmDd {#DayDddMmDd}
```
public static final int DayDddMmDd
```


Examples are Mon 9/30, Tue 10/1

### DayDddMmDdYy {#DayDddMmDdYy}
```
public static final int DayDddMmDdYy
```


Examples are Mon 9/30/02, Tue 10/1/02

### DayDddMmmDd {#DayDddMmmDd}
```
public static final int DayDddMmmDd
```


Examples are Mon Sep 30, Tue Oct 1

### DayDddMmmDdYyy {#DayDddMmmDdYyy}
```
public static final int DayDddMmmDdYyy
```


Examples are Mon Sep 30 '02, Tue Oct 1 '02

### DayDddMmmmDd {#DayDddMmmmDd}
```
public static final int DayDddMmmmDd
```


Examples are Mon September 30, Tue October 1

### DayDddd {#DayDddd}
```
public static final int DayDddd
```


Examples are Tuesday, Wednesday.

### DayDdi {#DayDdi}
```
public static final int DayDdi
```


Examples are Mo, Tu

### DayDdiDd {#DayDdiDd}
```
public static final int DayDdiDd
```


Examples are Mo 30, Tu 1

### DayDdiMDd {#DayDdiMDd}
```
public static final int DayDdiMDd
```


Examples are Mo S 30, Tu O 1

### DayDdiMmDd {#DayDdiMmDd}
```
public static final int DayDdiMmDd
```


Examples are Mo 9/30, Tu 10/1

### DayDi {#DayDi}
```
public static final int DayDi
```


Examples are M, T

### DayDiDdNoSpace {#DayDiDdNoSpace}
```
public static final int DayDiDdNoSpace
```


Examples are M30, T1

### DayDiDdSpace {#DayDiDdSpace}
```
public static final int DayDiDdSpace
```


Examples are M 30, T 1

### DayDiMDd {#DayDiMDd}
```
public static final int DayDiMDd
```


Examples are M S 30, T O 1

### DayDiMmDd {#DayDiMmDd}
```
public static final int DayDiMmDd
```


Examples are M 9/30, T 10/1

### DayFromEndDayDd {#DayFromEndDayDd}
```
public static final int DayFromEndDayDd
```


Examples are Day 2, Day 1, Day -1, Day -2 from the project end.

### DayFromEndDd {#DayFromEndDd}
```
public static final int DayFromEndDd
```


Examples are 2, 1, -1, -2

### DayFromEndDdd {#DayFromEndDdd}
```
public static final int DayFromEndDdd
```


Examples are D2, D1, D-1, D-2

### DayFromStartDayDd {#DayFromStartDayDd}
```
public static final int DayFromStartDayDd
```


Examples are Day -2, Day -1, Day 1, Day 2 from the project start.

### DayFromStartDd {#DayFromStartDd}
```
public static final int DayFromStartDd
```


Examples are -2, -1, 1, 2

### DayFromStartDdd {#DayFromStartDdd}
```
public static final int DayFromStartDdd
```


Examples are D-2, D-1, D1, D2

### DayMDd {#DayMDd}
```
public static final int DayMDd
```


Examples are S 30, O 1

### DayMmDd {#DayMmDd}
```
public static final int DayMmDd
```


Examples are 9/30, 10/1

### DayMmDdYy {#DayMmDdYy}
```
public static final int DayMmDdYy
```


Examples are 9/30/02, 10/1/02

### DayMmmDd {#DayMmmDd}
```
public static final int DayMmmDd
```


Examples are Sep 30, Oct 1

### DayMmmDdYyy {#DayMmmDdYyy}
```
public static final int DayMmmDdYyy
```


Examples are Sep 30 '02, Oct 10 '02

### DayOfMonthDd {#DayOfMonthDd}
```
public static final int DayOfMonthDd
```


Examples are 30, 1

### DayOfYearDd {#DayOfYearDd}
```
public static final int DayOfYearDd
```


Examples are 77, 78

### DayOfYearDdYyy {#DayOfYearDdYyy}
```
public static final int DayOfYearDdYyy
```


Examples are 77 '10, 78 '10

### DayOfYearDdYyyy {#DayOfYearDdYyyy}
```
public static final int DayOfYearDdYyyy
```


Examples are 77 2010, 78 2010

### HalfYearFromEndH {#HalfYearFromEndH}
```
public static final int HalfYearFromEndH
```


Examples are 2, 1, -1, -2. Half years from the project end date.

### HalfYearFromEndHalfH {#HalfYearFromEndHalfH}
```
public static final int HalfYearFromEndHalfH
```


Examples are Half 2, Half 1, Half -1, Half -2

### HalfYearFromEndHh {#HalfYearFromEndHh}
```
public static final int HalfYearFromEndHh
```


Examples are H2, H1, H-1, H-2

### HalfYearFromStartH {#HalfYearFromStartH}
```
public static final int HalfYearFromStartH
```


Examples are -2, -1, 1, 2. Half years from the project start date.

### HalfYearFromStartHalfH {#HalfYearFromStartHalfH}
```
public static final int HalfYearFromStartHalfH
```


Examples are Half -2, Half -1, Half 1, Half 2

### HalfYearFromStartHh {#HalfYearFromStartHh}
```
public static final int HalfYearFromStartHh
```


Examples are H-2, H-1, H1, H2

### HalfYearH {#HalfYearH}
```
public static final int HalfYearH
```


Examples are 1, 2. Requires the time unit to be TimescaleHalfYears.

### HalfYearHHyy {#HalfYearHHyy}
```
public static final int HalfYearHHyy
```


Examples are 1H10, 2H10

### HalfYearHh {#HalfYearHh}
```
public static final int HalfYearHh
```


Examples are H1, H2

### HalfYearHhYyy {#HalfYearHhYyy}
```
public static final int HalfYearHhYyy
```


Examples are H1 '10, H2 '10

### HalfYearHhhHalf {#HalfYearHhhHalf}
```
public static final int HalfYearHhhHalf
```


Examples are 1st Half, 2d Half

### HalfYearHlfH {#HalfYearHlfH}
```
public static final int HalfYearHlfH
```


Examples are Half 1, Half 2

### HalfYearHlfHYyyy {#HalfYearHlfHYyyy}
```
public static final int HalfYearHlfHYyyy
```


Examples are Half 1, 2010; Half 2, 2010

### HourDddMmmDdHhAm {#HourDddMmmDdHhAm}
```
public static final int HourDddMmmDdHhAm
```


Examples are Wed Mar 18, 8 AM; Wed Mar 18, 9 AM. Requires the time unit to be TimescaleHours.

### HourFromEndHh {#HourFromEndHh}
```
public static final int HourFromEndHh
```


Examples are 3, 2, 1, -1, -2 hours from the project end.

### HourFromEndHhh {#HourFromEndHhh}
```
public static final int HourFromEndHhh
```


Examples are H3, H2, H1, H-1, H-2

### HourFromEndHourHh {#HourFromEndHourHh}
```
public static final int HourFromEndHourHh
```


Examples are Hour 3, Hour 2, Hour 1, Hour -1, Hour -2

### HourFromStartHh {#HourFromStartHh}
```
public static final int HourFromStartHh
```


Examples are -2, -1, 1, 2, 3 hours from the project start.

### HourFromStartHhh {#HourFromStartHhh}
```
public static final int HourFromStartHhh
```


Examples are H-2, H-1, H1, H2, H3

### HourFromStartHourHh {#HourFromStartHourHh}
```
public static final int HourFromStartHourHh
```


Examples are Hour -2, Hour -1, Hour 1, Hour 2, Hour 3

### HourHh {#HourHh}
```
public static final int HourHh
```


Examples are 8, 9, 10, 11

### HourHhAm {#HourHhAm}
```
public static final int HourHhAm
```


Examples are 8AM, 9AM

### HourHhMmAm {#HourHhMmAm}
```
public static final int HourHhMmAm
```


Examples are 8:00 AM, 9:00 AM

### HourMmDdHhAm {#HourMmDdHhAm}
```
public static final int HourMmDdHhAm
```


Examples are 3/18 8 AM, 3/18 9 AM

### HourMmmDdHhAm {#HourMmmDdHhAm}
```
public static final int HourMmmDdHhAm
```


Examples are Mar 18, 8 AM; Mar 18, 9 AM

### MinuteFromEndMinuteMm {#MinuteFromEndMinuteMm}
```
public static final int MinuteFromEndMinuteMm
```


Examples are Minute 181, Minute 180, ..., Minute 1, Minute -1 from the project end.

### MinuteFromEndMm {#MinuteFromEndMm}
```
public static final int MinuteFromEndMm
```


Examples are 181, 180, ..., 1, -1

### MinuteFromEndMmm {#MinuteFromEndMmm}
```
public static final int MinuteFromEndMmm
```


Examples are M181, M180, ..., M1, M-1

### MinuteFromStartMinuteMm {#MinuteFromStartMinuteMm}
```
public static final int MinuteFromStartMinuteMm
```


Examples are Minute -2, Minute -1, Minute 1, ... Minute 180 from the project start.

### MinuteFromStartMm {#MinuteFromStartMm}
```
public static final int MinuteFromStartMm
```


Examples are -2, -1, 1, ..., 180

### MinuteFromStartMmm {#MinuteFromStartMmm}
```
public static final int MinuteFromStartMmm
```


Examples are M-2, M-1, M1, ..., M180

### MinuteHhMmAm {#MinuteHhMmAm}
```
public static final int MinuteHhMmAm
```


Examples are 8:00 AM, 8:01 AM, 8:02 AM. Requires the time unit to be TimescaleMinutes.

### MinuteMm {#MinuteMm}
```
public static final int MinuteMm
```


Examples are 0, 1, 2, ..., 59 minutes

### MonthFromEndMm {#MonthFromEndMm}
```
public static final int MonthFromEndMm
```


Examples are 2, 1, -1, -2 months from the project end.

### MonthFromEndMmm {#MonthFromEndMmm}
```
public static final int MonthFromEndMmm
```


Examples are M2, M1, M-1, M-2

### MonthFromEndMonthMm {#MonthFromEndMonthMm}
```
public static final int MonthFromEndMonthMm
```


Examples are Month 2, Month 1, Month -1, Month -2

### MonthFromStartMm {#MonthFromStartMm}
```
public static final int MonthFromStartMm
```


Examples are -2, -2, 1, 2 months from the project start.

### MonthFromStartMmm {#MonthFromStartMmm}
```
public static final int MonthFromStartMmm
```


Examples are M-2, M-1, M1, M2

### MonthFromStartMonthMm {#MonthFromStartMonthMm}
```
public static final int MonthFromStartMonthMm
```


Examples are Month -2, Month -1, Month 1, Month 2

### MonthM {#MonthM}
```
public static final int MonthM
```


Examples are M, A, M, J, J. Requires the time unit to be TimescaleMonths.

### MonthMm {#MonthMm}
```
public static final int MonthMm
```


Examples are 11, 12, 1, 2

### MonthMmYy {#MonthMmYy}
```
public static final int MonthMmYy
```


Examples are 3/10, 4/10, 5/10

### MonthMmYyy {#MonthMmYyy}
```
public static final int MonthMmYyy
```


Examples are 3 '10, 4 '10, 5 '10

### MonthMmm {#MonthMmm}
```
public static final int MonthMmm
```


Examples are Mar, Apr, May

### MonthMmmYyy {#MonthMmmYyy}
```
public static final int MonthMmmYyy
```


Examples are Mar '10, Apr '10, May '10

### MonthMmmm {#MonthMmmm}
```
public static final int MonthMmmm
```


Examples are March, April, May

### MonthMmmmYyyy {#MonthMmmmYyyy}
```
public static final int MonthMmmmYyyy
```


Examples are March 2010, April 2010, May 2010

### None {#None}
```
public static final int None
```


No date is displayed.

### QuarterFromEndQ {#QuarterFromEndQ}
```
public static final int QuarterFromEndQ
```


Examples are 5, 4, 3, 2, 1, -1 quarters from the project end.

### QuarterFromEndQq {#QuarterFromEndQq}
```
public static final int QuarterFromEndQq
```


Examples are Q5, Q4, Q3, Q2, Q1, Q-1

### QuarterFromEndQuarterQ {#QuarterFromEndQuarterQ}
```
public static final int QuarterFromEndQuarterQ
```


Examples are Quarter 5, Quarter 4, Quarter 3, Quarter 2, Quarter 1, Quarter -1

### QuarterFromStartQ {#QuarterFromStartQ}
```
public static final int QuarterFromStartQ
```


Examples are -5, -4, -3, -2, -1, 1 quarters from the project start.

### QuarterFromStartQq {#QuarterFromStartQq}
```
public static final int QuarterFromStartQq
```


Examples are Q-5, Q-4, Q-3, Q-2, Q-1, Q1

### QuarterFromStartQuarterQ {#QuarterFromStartQuarterQ}
```
public static final int QuarterFromStartQuarterQ
```


Examples are Quarter -5, Quarter -4, Quarter -3, Quarter -2, Quarter -1, Quarter 1

### QuarterQ {#QuarterQ}
```
public static final int QuarterQ
```


Examples are 3, 4, 1. Requires the time unit to be TimescaleQuarters.

### QuarterQQyy {#QuarterQQyy}
```
public static final int QuarterQQyy
```


Examples are 3Q10, 4Q10, 1Q11

### QuarterQq {#QuarterQq}
```
public static final int QuarterQq
```


Examples are Q3, Q4, Q1

### QuarterQqYyy {#QuarterQqYyy}
```
public static final int QuarterQqYyy
```


Examples are Q3 '10, Q4 '10, Q1 '11

### QuarterQqqQuarter {#QuarterQqqQuarter}
```
public static final int QuarterQqqQuarter
```


Examples are 3rd Quarter, 1st Quarter

### QuarterQtrQ {#QuarterQtrQ}
```
public static final int QuarterQtrQ
```


Examples are Qtr3, Qtr4, Qtr1

### QuarterQtrQYyyy {#QuarterQtrQYyyy}
```
public static final int QuarterQtrQYyyy
```


Examples are Qtr3, 2010; Qtr4, 2010; Qtr1, 2011

### ThirdsOfMonthsDd {#ThirdsOfMonthsDd}
```
public static final int ThirdsOfMonthsDd
```


Examples are 1, 11, 21, 1. Requires the time unit to be TimescaleThirdsOfMonths.

### ThirdsOfMonthsDdd {#ThirdsOfMonthsDdd}
```
public static final int ThirdsOfMonthsDdd
```


Examples are B, M, E, B

### ThirdsOfMonthsDddd {#ThirdsOfMonthsDddd}
```
public static final int ThirdsOfMonthsDddd
```


Examples are Beginning, Middle, End, Beginning

### ThirdsOfMonthsMmDd {#ThirdsOfMonthsMmDd}
```
public static final int ThirdsOfMonthsMmDd
```


Example is 3/1.

### ThirdsOfMonthsMmDdYy {#ThirdsOfMonthsMmDdYy}
```
public static final int ThirdsOfMonthsMmDdYy
```


Example is 3/1/10.

### ThirdsOfMonthsMmDdd {#ThirdsOfMonthsMmDdd}
```
public static final int ThirdsOfMonthsMmDdd
```


Examples are 3/B, 3/M, 3/E, 4/B

### ThirdsOfMonthsMmDddYy {#ThirdsOfMonthsMmDddYy}
```
public static final int ThirdsOfMonthsMmDddYy
```


Example is 3/B/10.

### ThirdsOfMonthsMmmDd {#ThirdsOfMonthsMmmDd}
```
public static final int ThirdsOfMonthsMmmDd
```


Examples are Mar 1, Mar 11, Mar 21, Apr 1

### ThirdsOfMonthsMmmDdYy {#ThirdsOfMonthsMmmDdYy}
```
public static final int ThirdsOfMonthsMmmDdYy
```


Examples are Mar 1, '10; Mar 11, '10; Mar 21, '10; Apr 1, 10

### ThirdsOfMonthsMmmDdd {#ThirdsOfMonthsMmmDdd}
```
public static final int ThirdsOfMonthsMmmDdd
```


Examples are Mar B, Mar M, Mar E, Apr B

### ThirdsOfMonthsMmmDddYy {#ThirdsOfMonthsMmmDddYy}
```
public static final int ThirdsOfMonthsMmmDddYy
```


Examples are Mar B, '10; Mar M, '10; Mar E, '10; Apr B '10

### ThirdsOfMonthsMmmmDd {#ThirdsOfMonthsMmmmDd}
```
public static final int ThirdsOfMonthsMmmmDd
```


Examples are March 1, March 11, March 21, April 1

### ThirdsOfMonthsMmmmDdYyyy {#ThirdsOfMonthsMmmmDdYyyy}
```
public static final int ThirdsOfMonthsMmmmDdYyyy
```


Examples are March 1, 2010; March 11, 2010; March 21, 2010; April 1, 2010

### ThirdsOfMonthsMmmmDddd {#ThirdsOfMonthsMmmmDddd}
```
public static final int ThirdsOfMonthsMmmmDddd
```


Examples are March Beginning, March Middle, March End, April Beginning

### ThirdsOfMonthsMmmmDdddYyyy {#ThirdsOfMonthsMmmmDdddYyyy}
```
public static final int ThirdsOfMonthsMmmmDdddYyyy
```


Examples are March Beginning, 2010; March Middle, 2010; March End, 2010; April Beginning, 2010

### WeekDayOfMonthDd {#WeekDayOfMonthDd}
```
public static final int WeekDayOfMonthDd
```


Examples are 21, 28, 4

### WeekDddDd {#WeekDddDd}
```
public static final int WeekDddDd
```


Examples are Sun 21, Sun 28, Sun 4. Requires the time unit to be TimescaleWeeks.

### WeekDddMDd {#WeekDddMDd}
```
public static final int WeekDddMDd
```


Examples are Sun M 21, Sun M 28, Sun A 4

### WeekDddMmDd {#WeekDddMmDd}
```
public static final int WeekDddMmDd
```


Examples are Sun 3/21, Sun 3/28, Sun 4/4

### WeekDddMmDdYy {#WeekDddMmDdYy}
```
public static final int WeekDddMmDdYy
```


Examples are Sun 3/21/10, Sun 3/28/10, Sun 4/4/10

### WeekDddMmmDd {#WeekDddMmmDd}
```
public static final int WeekDddMmmDd
```


Examples are Sun Mar 21, Sun Mar 28, Sun Apr 4

### WeekDddMmmDdYyy {#WeekDddMmmDdYyy}
```
public static final int WeekDddMmmDdYyy
```


Examples are Sun Mar 21, '10; Sun Mar 28, '10; Sun Apr 4, '10

### WeekDddMmmmDd {#WeekDddMmmmDd}
```
public static final int WeekDddMmmmDd
```


Examples are Sun Mar 21, Sun March 28, Sun Apr 4

### WeekDddMmmmDdYyy {#WeekDddMmmmDdYyy}
```
public static final int WeekDddMmmmDdYyy
```


Examples are Sun March 21, '10; Sun March 28, '10; Sun April 4, '10

### WeekDddWw {#WeekDddWw}
```
public static final int WeekDddWw
```


Examples are Sun 12, Sun 13, Sun 14

### WeekDdiMDd {#WeekDdiMDd}
```
public static final int WeekDdiMDd
```


Examples are Su M 21, Su M 28, Su A 4

### WeekDdiMmDd {#WeekDdiMmDd}
```
public static final int WeekDdiMmDd
```


Examples are Su 3/21. Su 3/28, Su 4/4

### WeekDdiMmmDd {#WeekDdiMmmDd}
```
public static final int WeekDdiMmmDd
```


Examples are Su Mar 21, Su Mar 28, Su Apr 4

### WeekDiMDd {#WeekDiMDd}
```
public static final int WeekDiMDd
```


Examples are S M 21, S M 28, S A 4

### WeekDiMmDd {#WeekDiMmDd}
```
public static final int WeekDiMmDd
```


Examples are S 3/21, S 3/28, S 4/4

### WeekDiMmmDd {#WeekDiMmmDd}
```
public static final int WeekDiMmmDd
```


Examples are S Mar 21, S Mar 28, S Apr 4

### WeekFromEndWeekWw {#WeekFromEndWeekWw}
```
public static final int WeekFromEndWeekWw
```


Examples are Week 2, Week 1, Week -1 from the project end.

### WeekFromEndWw {#WeekFromEndWw}
```
public static final int WeekFromEndWw
```


Examples are 2, 1, -1

### WeekFromEndWww {#WeekFromEndWww}
```
public static final int WeekFromEndWww
```


Examples are W2, W1, W-1

### WeekFromStartWeekWw {#WeekFromStartWeekWw}
```
public static final int WeekFromStartWeekWw
```


Examples are Week -1, Week 1, Week 2 from the project start.

### WeekFromStartWw {#WeekFromStartWw}
```
public static final int WeekFromStartWw
```


Examples are -1, 1, 2

### WeekFromStartWww {#WeekFromStartWww}
```
public static final int WeekFromStartWww
```


Examples are W-1, W1, W2

### WeekMDd {#WeekMDd}
```
public static final int WeekMDd
```


Examples are M21, M28, A 4

### WeekMmDd {#WeekMmDd}
```
public static final int WeekMmDd
```


Examples are 3/21, 3/28, 4/4

### WeekMmDdYy {#WeekMmDdYy}
```
public static final int WeekMmDdYy
```


Example is '3/21/10'.

### WeekMmmDd {#WeekMmmDd}
```
public static final int WeekMmmDd
```


Examples are Mar 21, Mar 28, Apr 4

### WeekMmmDdYyy {#WeekMmmDdYyy}
```
public static final int WeekMmmDdYyy
```


Examples are Mar 21, '10; Mar 28, '10; Apr 4, '10

### WeekMmmmDd {#WeekMmmmDd}
```
public static final int WeekMmmmDd
```


Examples are March 21, March 28, April 4

### WeekMmmmDdYyyy {#WeekMmmmDdYyyy}
```
public static final int WeekMmmmDdYyyy
```


Examples are March 21, 2010; March 28, 2010; April 4, 2010

### WeekNumberDdWw {#WeekNumberDdWw}
```
public static final int WeekNumberDdWw
```


Examples are 1 12, 1 13, 1 14 (day 1 of week 12, day 1 of week 13, and so forth)

### WeekNumberWw {#WeekNumberWw}
```
public static final int WeekNumberWw
```


Examples are 12, 13, 14

### YearFromEndYearYy {#YearFromEndYearYy}
```
public static final int YearFromEndYearYy
```


Examples are Year 2, Year 1, Year -1 from the project end.

### YearFromEndYy {#YearFromEndYy}
```
public static final int YearFromEndYy
```


Examples are 2, 1, -1

### YearFromEndYyy {#YearFromEndYyy}
```
public static final int YearFromEndYyy
```


Examples are Y2, Y1, Y-1

### YearFromStartYearYy {#YearFromStartYearYy}
```
public static final int YearFromStartYearYy
```


Examples are Year -1, Year 1, Year 2 from the project start.

### YearFromStartYy {#YearFromStartYy}
```
public static final int YearFromStartYy
```


Examples are -1, 1, 2

### YearFromStartYyy {#YearFromStartYyy}
```
public static final int YearFromStartYyy
```


Examples are Y-1, Y1, Y2

### YearYy {#YearYy}
```
public static final int YearYy
```


Examples are 10, 11, 12. Requires the time unit to be TimescaleYears.

### YearYyy {#YearYyy}
```
public static final int YearYyy
```


Examples are '10, '11, '12

### YearYyyy {#YearYyyy}
```
public static final int YearYyyy
```


Examples are 2010, 2011, 2012

