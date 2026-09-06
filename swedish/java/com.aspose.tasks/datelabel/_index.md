---
title: "DateLabel"
second_title: "Aspose.Tasks for Java API-referens"
description: "Anger visningsformatet för datum- och tidsetiketter i en tidslinje."
type: docs
weight: 69
url: /sv/java/com.aspose.tasks/datelabel/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class DateLabel extends System.Enum
```

Anger visningsformatet för datum- och tidsetiketter i en tidslinje.
## Fält

| Fält | Beskrivning |
| --- | --- |
| [DayDdMmYyyy](#DayDdMmYyyy) | Exempel är 19/07/2016. |
| [DayDdd](#DayDdd) | Exempel är Mon, Tue. |
| [DayDddDd](#DayDddDd) | Exempel är Mon 30, Tue 1 |
| [DayDddMDd](#DayDddMDd) | Exempel är Mon S 30, Tue O 1 |
| [DayDddMmDd](#DayDddMmDd) | Exempel är Mon 9/30, Tue 10/1 |
| [DayDddMmDdYy](#DayDddMmDdYy) | Exempel är Mon 9/30/02, Tue 10/1/02 |
| [DayDddMmmDd](#DayDddMmmDd) | Exempel är Mån sep 30, Tis okt 1 |
| [DayDddMmmDdYyy](#DayDddMmmDdYyy) | Exempel är Mån sep 30 '02, Tis okt 1 '02 |
| [DayDddMmmmDd](#DayDddMmmmDd) | Exempel är Måndag september 30, Tisdag oktober 1 |
| [DayDddd](#DayDddd) | Exempel är tisdag, onsdag. |
| [DayDdi](#DayDdi) | Exempel är Må, Ti |
| [DayDdiDd](#DayDdiDd) | Exempel är Må 30, Ti 1 |
| [DayDdiMDd](#DayDdiMDd) | Exempel är Må sep 30, Ti okt 1 |
| [DayDdiMmDd](#DayDdiMmDd) | Exempel är Må 9/30, Ti 10/1 |
| [DayDi](#DayDi) | Exempel är M, T |
| [DayDiDdNoSpace](#DayDiDdNoSpace) | Exempel är M30, T1 |
| [DayDiDdSpace](#DayDiDdSpace) | Exempel är M 30, T 1 |
| [DayDiMDd](#DayDiMDd) | Exempel är M sep 30, T okt 1 |
| [DayDiMmDd](#DayDiMmDd) | Exempel är M 9/30, T 10/1 |
| [DayFromEndDayDd](#DayFromEndDayDd) | Exempel är Dag 2, Dag 1, Dag -1, Dag -2 från projektets slut. |
| [DayFromEndDd](#DayFromEndDd) | Exempel är 2, 1, -1, -2 |
| [DayFromEndDdd](#DayFromEndDdd) | Exempel är D2, D1, D-1, D-2 |
| [DayFromStartDayDd](#DayFromStartDayDd) | Exempel är Dag -2, Dag -1, Dag 1, Dag 2 från projektets start. |
| [DayFromStartDd](#DayFromStartDd) | Exempel är -2, -1, 1, 2 |
| [DayFromStartDdd](#DayFromStartDdd) | Exempel är D-2, D-1, D1, D2 |
| [DayMDd](#DayMDd) | Exempel är sep 30, okt 1 |
| [DayMmDd](#DayMmDd) | Exempel är 9/30, 10/1 |
| [DayMmDdYy](#DayMmDdYy) | Exempel är 9/30/02, 10/1/02 |
| [DayMmmDd](#DayMmmDd) | Exempel är sep 30, okt 1 |
| [DayMmmDdYyy](#DayMmmDdYyy) | Exempel är sep 30 '02, okt 10 '02 |
| [DayOfMonthDd](#DayOfMonthDd) | Exempel är 30, 1 |
| [DayOfYearDd](#DayOfYearDd) | Exempel är 77, 78 |
| [DayOfYearDdYyy](#DayOfYearDdYyy) | Exempel är 77 '10, 78 '10 |
| [DayOfYearDdYyyy](#DayOfYearDdYyyy) | Exempel är 77 2010, 78 2010 |
| [HalfYearFromEndH](#HalfYearFromEndH) | Exempel är 2, 1, -1, -2. |
| [HalfYearFromEndHalfH](#HalfYearFromEndHalfH) | Exempel är Halv 2, Halv 1, Halv -1, Halv -2 |
| [HalfYearFromEndHh](#HalfYearFromEndHh) | Exempel är H2, H1, H-1, H-2 |
| [HalfYearFromStartH](#HalfYearFromStartH) | Exempel är -2, -1, 1, 2. |
| [HalfYearFromStartHalfH](#HalfYearFromStartHalfH) | Exempel är Halv -2, Halv -1, Halv 1, Halv 2 |
| [HalfYearFromStartHh](#HalfYearFromStartHh) | Exempel är H-2, H-1, H1, H2 |
| [HalfYearH](#HalfYearH) | Exempel är 1, 2. |
| [HalfYearHHyy](#HalfYearHHyy) | Exempel är 1H10, 2H10 |
| [HalfYearHh](#HalfYearHh) | Exempel är H1, H2 |
| [HalfYearHhYyy](#HalfYearHhYyy) | Exempel är H1 '10, H2 '10 |
| [HalfYearHhhHalf](#HalfYearHhhHalf) | Exempel är 1:a Halv, 2:a Halv |
| [HalfYearHlfH](#HalfYearHlfH) | Exempel är Halv 1, Halv 2 |
| [HalfYearHlfHYyyy](#HalfYearHlfHYyyy) | Exempel är Halv 1, 2010; Halv 2, 2010 |
| [HourDddMmmDdHhAm](#HourDddMmmDdHhAm) | Exempel är Wed Mar 18, 8 fm; Wed Mar 18, 9 fm. |
| [HourFromEndHh](#HourFromEndHh) | Exempel är 3, 2, 1, -1, -2 timmar från projektets slut. |
| [HourFromEndHhh](#HourFromEndHhh) | Exempel är H3, H2, H1, H-1, H-2 |
| [HourFromEndHourHh](#HourFromEndHourHh) | Exempel är Timme 3, Timme 2, Timme 1, Timme -1, Timme -2 |
| [HourFromStartHh](#HourFromStartHh) | Exempel är -2, -1, 1, 2, 3 timmar från projektets start. |
| [HourFromStartHhh](#HourFromStartHhh) | Exempel är H-2, H-1, H1, H2, H3 |
| [HourFromStartHourHh](#HourFromStartHourHh) | Exempel är Timme -2, Timme -1, Timme 1, Timme 2, Timme 3 |
| [HourHh](#HourHh) | Exempel är 8, 9, 10, 11 |
| [HourHhAm](#HourHhAm) | Exempel är 8 fm, 9 fm |
| [HourHhMmAm](#HourHhMmAm) | Exempel är 8:00 AM, 9:00 AM |
| [HourMmDdHhAm](#HourMmDdHhAm) | Exempel är 3/18 8 AM, 3/18 9 AM |
| [HourMmmDdHhAm](#HourMmmDdHhAm) | Exempel är Mar 18, 8 AM; Mar 18, 9 AM |
| [MinuteFromEndMinuteMm](#MinuteFromEndMinuteMm) | Exempel är Minute 181, Minute 180, ..., Minute 1, Minute -1 från projektets slut. |
| [MinuteFromEndMm](#MinuteFromEndMm) | Exempel är 181, 180, ..., 1, -1 |
| [MinuteFromEndMmm](#MinuteFromEndMmm) | Exempel är M181, M180, ..., M1, M-1 |
| [MinuteFromStartMinuteMm](#MinuteFromStartMinuteMm) | Exempel är Minute -2, Minute -1, Minute 1, ... |
| [MinuteFromStartMm](#MinuteFromStartMm) | Exempel är -2, -1, 1, ..., 180 |
| [MinuteFromStartMmm](#MinuteFromStartMmm) | Exempel är M-2, M-1, M1, ..., M180 |
| [MinuteHhMmAm](#MinuteHhMmAm) | Exempel är 8:00 AM, 8:01 AM, 8:02 AM. |
| [MinuteMm](#MinuteMm) | Exempel är 0, 1, 2, ..., 59 minuter |
| [MonthFromEndMm](#MonthFromEndMm) | Exempel är 2, 1, -1, -2 månader från projektets slut. |
| [MonthFromEndMmm](#MonthFromEndMmm) | Exempel är M2, M1, M-1, M-2 |
| [MonthFromEndMonthMm](#MonthFromEndMonthMm) | Exempel är Month 2, Month 1, Month -1, Month -2 |
| [MonthFromStartMm](#MonthFromStartMm) | Exempel är -2, -2, 1, 2 månader från projektets start. |
| [MonthFromStartMmm](#MonthFromStartMmm) | Exempel är M-2, M-1, M1, M2 |
| [MonthFromStartMonthMm](#MonthFromStartMonthMm) | Exempel är Month -2, Month -1, Month 1, Month 2 |
| [MonthM](#MonthM) | Exempel är M, A, M, J, J. |
| [MonthMm](#MonthMm) | Exempel är 11, 12, 1, 2 |
| [MonthMmYy](#MonthMmYy) | Exempel är 3/10, 4/10, 5/10 |
| [MonthMmYyy](#MonthMmYyy) | Exempel är 3 '10, 4 '10, 5 '10 |
| [MonthMmm](#MonthMmm) | Exempel är Mar, Apr, May |
| [MonthMmmYyy](#MonthMmmYyy) | Exempel är Mar '10, Apr '10, May '10 |
| [MonthMmmm](#MonthMmmm) | Exempel är March, April, May |
| [MonthMmmmYyyy](#MonthMmmmYyyy) | Exempel är March 2010, April 2010, May 2010 |
| [None](#None) | Inget datum visas. |
| [QuarterFromEndQ](#QuarterFromEndQ) | Exempel är 5, 4, 3, 2, 1, -1 kvartal från projektets slut. |
| [QuarterFromEndQq](#QuarterFromEndQq) | Exempel är Q5, Q4, Q3, Q2, Q1, Q-1 |
| [QuarterFromEndQuarterQ](#QuarterFromEndQuarterQ) | Exempel är Kvartal 5, Kvartal 4, Kvartal 3, Kvartal 2, Kvartal 1, Kvartal -1 |
| [QuarterFromStartQ](#QuarterFromStartQ) | Exempel är -5, -4, -3, -2, -1, 1 kvartal från projektets start. |
| [QuarterFromStartQq](#QuarterFromStartQq) | Exempel är Q-5, Q-4, Q-3, Q-2, Q-1, Q1 |
| [QuarterFromStartQuarterQ](#QuarterFromStartQuarterQ) | Exempel är Kvartal -5, Kvartal -4, Kvartal -3, Kvartal -2, Kvartal -1, Kvartal 1 |
| [QuarterQ](#QuarterQ) | Exempel är 3, 4, 1. |
| [QuarterQQyy](#QuarterQQyy) | Exempel är 3Q10, 4Q10, 1Q11 |
| [QuarterQq](#QuarterQq) | Exempel är Q3, Q4, Q1 |
| [QuarterQqYyy](#QuarterQqYyy) | Exempel är Q3 '10, Q4 '10, Q1 '11 |
| [QuarterQqqQuarter](#QuarterQqqQuarter) | Exempel är 3:e kvartalet, 1:a kvartalet |
| [QuarterQtrQ](#QuarterQtrQ) | Exempel är Qtr3, Qtr4, Qtr1 |
| [QuarterQtrQYyyy](#QuarterQtrQYyyy) | Exempel är Qtr3, 2010; Qtr4, 2010; Qtr1, 2011 |
| [ThirdsOfMonthsDd](#ThirdsOfMonthsDd) | Exempel är 1, 11, 21, 1. |
| [ThirdsOfMonthsDdd](#ThirdsOfMonthsDdd) | Exempel är B, M, E, B |
| [ThirdsOfMonthsDddd](#ThirdsOfMonthsDddd) | Exempel är Början, Mitten, Slutet, Början |
| [ThirdsOfMonthsMmDd](#ThirdsOfMonthsMmDd) | Exempel är 3/1. |
| [ThirdsOfMonthsMmDdYy](#ThirdsOfMonthsMmDdYy) | Exempel är 3/1/10. |
| [ThirdsOfMonthsMmDdd](#ThirdsOfMonthsMmDdd) | Exempel är 3/B, 3/M, 3/E, 4/B |
| [ThirdsOfMonthsMmDddYy](#ThirdsOfMonthsMmDddYy) | Exempel är 3/B/10. |
| [ThirdsOfMonthsMmmDd](#ThirdsOfMonthsMmmDd) | Exempel är 1 mars, 11 mars, 21 mars, 1 apr |
| [ThirdsOfMonthsMmmDdYy](#ThirdsOfMonthsMmmDdYy) | Exempel är 1 mars, '10; 11 mars, '10; 21 mars, '10; 1 apr, 10 |
| [ThirdsOfMonthsMmmDdd](#ThirdsOfMonthsMmmDdd) | Exempel är mars B, mars M, mars E, apr B |
| [ThirdsOfMonthsMmmDddYy](#ThirdsOfMonthsMmmDddYy) | Exempel är mars B, '10; mars M, '10; mars E, '10; apr B '10 |
| [ThirdsOfMonthsMmmmDd](#ThirdsOfMonthsMmmmDd) | Exempel är 1 mars, 11 mars, 21 mars, 1 april |
| [ThirdsOfMonthsMmmmDdYyyy](#ThirdsOfMonthsMmmmDdYyyy) | Exempel är 1 mars 2010; 11 mars 2010; 21 mars 2010; 1 april 2010 |
| [ThirdsOfMonthsMmmmDddd](#ThirdsOfMonthsMmmmDddd) | Exempel är mars början, mars mitten, mars slutet, april början |
| [ThirdsOfMonthsMmmmDdddYyyy](#ThirdsOfMonthsMmmmDdddYyyy) | Exempel är mars början, 2010; mars mitten, 2010; mars slutet, 2010; april början, 2010 |
| [WeekDayOfMonthDd](#WeekDayOfMonthDd) | Exempel är 21, 28, 4 |
| [WeekDddDd](#WeekDddDd) | Exempel är sön 21, sön 28, sön 4. |
| [WeekDddMDd](#WeekDddMDd) | Exempel är sön M 21, sön M 28, sön A 4 |
| [WeekDddMmDd](#WeekDddMmDd) | Exempel är sön 3/21, sön 3/28, sön 4/4 |
| [WeekDddMmDdYy](#WeekDddMmDdYy) | Exempel är sön 3/21/10, sön 3/28/10, sön 4/4/10 |
| [WeekDddMmmDd](#WeekDddMmmDd) | Exempel är sön mars 21, sön mars 28, sön apr 4 |
| [WeekDddMmmDdYyy](#WeekDddMmmDdYyy) | Exempel är sön mars 21, '10; sön mars 28, '10; sön apr 4, '10 |
| [WeekDddMmmmDd](#WeekDddMmmmDd) | Exempel är sön mars 21, sön mars 28, sön apr 4 |
| [WeekDddMmmmDdYyy](#WeekDddMmmmDdYyy) | Exempel är sön mars 21, '10; sön mars 28, '10; sön april 4, '10 |
| [WeekDddWw](#WeekDddWw) | Exempel är sön 12, sön 13, sön 14 |
| [WeekDdiMDd](#WeekDdiMDd) | Exempel är sön M 21, sön M 28, sön A 4 |
| [WeekDdiMmDd](#WeekDdiMmDd) | Exempel är sön 3/21. |
| [WeekDdiMmmDd](#WeekDdiMmmDd) | Exempel är sön mars 21, sön mars 28, sön apr 4 |
| [WeekDiMDd](#WeekDiMDd) | Exempel är sön M 21, sön M 28, sön A 4 |
| [WeekDiMmDd](#WeekDiMmDd) | Exempel är sön 3/21, sön 3/28, sön 4/4 |
| [WeekDiMmmDd](#WeekDiMmmDd) | Exempel är sön mars 21, sön mars 28, sön apr 4 |
| [WeekFromEndWeekWw](#WeekFromEndWeekWw) | Exempel är Vecka 2, Vecka 1, Vecka -1 från projektets slut. |
| [WeekFromEndWw](#WeekFromEndWw) | Exempel är 2, 1, -1 |
| [WeekFromEndWww](#WeekFromEndWww) | Exempel är W2, W1, W-1 |
| [WeekFromStartWeekWw](#WeekFromStartWeekWw) | Exempel är Vecka -1, Vecka 1, Vecka 2 från projektets start. |
| [WeekFromStartWw](#WeekFromStartWw) | Exempel är -1, 1, 2 |
| [WeekFromStartWww](#WeekFromStartWww) | Exempel är W-1, W1, W2 |
| [WeekMDd](#WeekMDd) | Exempel är M21, M28, A 4 |
| [WeekMmDd](#WeekMmDd) | Exempel är 3/21, 3/28, 4/4 |
| [WeekMmDdYy](#WeekMmDdYy) | Exempel är '3/21/10'. |
| [WeekMmmDd](#WeekMmmDd) | Exempel är 21 mar, 28 mar, 4 apr |
| [WeekMmmDdYyy](#WeekMmmDdYyy) | Exempel är 21 mar, '10; 28 mar, '10; 4 apr, '10 |
| [WeekMmmmDd](#WeekMmmmDd) | Exempel är 21 mars, 28 mars, 4 april |
| [WeekMmmmDdYyyy](#WeekMmmmDdYyyy) | Exempel är 21 mars, 2010; 28 mars, 2010; 4 april, 2010 |
| [WeekNumberDdWw](#WeekNumberDdWw) | Exempel är 1 12, 1 13, 1 14 (dag 1 i vecka 12, dag 1 i vecka 13, och så vidare) |
| [WeekNumberWw](#WeekNumberWw) | Exempel är 12, 13, 14 |
| [YearFromEndYearYy](#YearFromEndYearYy) | Exempel är År 2, År 1, År -1 från projektets slut. |
| [YearFromEndYy](#YearFromEndYy) | Exempel är 2, 1, -1 |
| [YearFromEndYyy](#YearFromEndYyy) | Exempel är Y2, Y1, Y-1 |
| [YearFromStartYearYy](#YearFromStartYearYy) | Exempel är År -1, År 1, År 2 från projektets start. |
| [YearFromStartYy](#YearFromStartYy) | Exempel är -1, 1, 2 |
| [YearFromStartYyy](#YearFromStartYyy) | Exempel är Y-1, Y1, Y2 |
| [YearYy](#YearYy) | Exempel är 10, 11, 12. |
| [YearYyy](#YearYyy) | Exempel är '10, '11, '12 |
| [YearYyyy](#YearYyyy) | Exempel är 2010, 2011, 2012 |
### DayDdMmYyyy {#DayDdMmYyyy}
```
public static final int DayDdMmYyyy
```


Exempel är 19/07/2016.

### DayDdd {#DayDdd}
```
public static final int DayDdd
```


Exempel är Mon, Tue.

### DayDddDd {#DayDddDd}
```
public static final int DayDddDd
```


Exempel är Mon 30, Tue 1

### DayDddMDd {#DayDddMDd}
```
public static final int DayDddMDd
```


Exempel är Mon S 30, Tue O 1

### DayDddMmDd {#DayDddMmDd}
```
public static final int DayDddMmDd
```


Exempel är Mon 9/30, Tue 10/1

### DayDddMmDdYy {#DayDddMmDdYy}
```
public static final int DayDddMmDdYy
```


Exempel är Mon 9/30/02, Tue 10/1/02

### DayDddMmmDd {#DayDddMmmDd}
```
public static final int DayDddMmmDd
```


Exempel är Mån sep 30, Tis okt 1

### DayDddMmmDdYyy {#DayDddMmmDdYyy}
```
public static final int DayDddMmmDdYyy
```


Exempel är Mån sep 30 '02, Tis okt 1 '02

### DayDddMmmmDd {#DayDddMmmmDd}
```
public static final int DayDddMmmmDd
```


Exempel är Måndag september 30, Tisdag oktober 1

### DayDddd {#DayDddd}
```
public static final int DayDddd
```


Exempel är tisdag, onsdag.

### DayDdi {#DayDdi}
```
public static final int DayDdi
```


Exempel är Må, Ti

### DayDdiDd {#DayDdiDd}
```
public static final int DayDdiDd
```


Exempel är Må 30, Ti 1

### DayDdiMDd {#DayDdiMDd}
```
public static final int DayDdiMDd
```


Exempel är Må sep 30, Ti okt 1

### DayDdiMmDd {#DayDdiMmDd}
```
public static final int DayDdiMmDd
```


Exempel är Må 9/30, Ti 10/1

### DayDi {#DayDi}
```
public static final int DayDi
```


Exempel är M, T

### DayDiDdNoSpace {#DayDiDdNoSpace}
```
public static final int DayDiDdNoSpace
```


Exempel är M30, T1

### DayDiDdSpace {#DayDiDdSpace}
```
public static final int DayDiDdSpace
```


Exempel är M 30, T 1

### DayDiMDd {#DayDiMDd}
```
public static final int DayDiMDd
```


Exempel är M sep 30, T okt 1

### DayDiMmDd {#DayDiMmDd}
```
public static final int DayDiMmDd
```


Exempel är M 9/30, T 10/1

### DayFromEndDayDd {#DayFromEndDayDd}
```
public static final int DayFromEndDayDd
```


Exempel är Dag 2, Dag 1, Dag -1, Dag -2 från projektets slut.

### DayFromEndDd {#DayFromEndDd}
```
public static final int DayFromEndDd
```


Exempel är 2, 1, -1, -2

### DayFromEndDdd {#DayFromEndDdd}
```
public static final int DayFromEndDdd
```


Exempel är D2, D1, D-1, D-2

### DayFromStartDayDd {#DayFromStartDayDd}
```
public static final int DayFromStartDayDd
```


Exempel är Dag -2, Dag -1, Dag 1, Dag 2 från projektets start.

### DayFromStartDd {#DayFromStartDd}
```
public static final int DayFromStartDd
```


Exempel är -2, -1, 1, 2

### DayFromStartDdd {#DayFromStartDdd}
```
public static final int DayFromStartDdd
```


Exempel är D-2, D-1, D1, D2

### DayMDd {#DayMDd}
```
public static final int DayMDd
```


Exempel är sep 30, okt 1

### DayMmDd {#DayMmDd}
```
public static final int DayMmDd
```


Exempel är 9/30, 10/1

### DayMmDdYy {#DayMmDdYy}
```
public static final int DayMmDdYy
```


Exempel är 9/30/02, 10/1/02

### DayMmmDd {#DayMmmDd}
```
public static final int DayMmmDd
```


Exempel är sep 30, okt 1

### DayMmmDdYyy {#DayMmmDdYyy}
```
public static final int DayMmmDdYyy
```


Exempel är sep 30 '02, okt 10 '02

### DayOfMonthDd {#DayOfMonthDd}
```
public static final int DayOfMonthDd
```


Exempel är 30, 1

### DayOfYearDd {#DayOfYearDd}
```
public static final int DayOfYearDd
```


Exempel är 77, 78

### DayOfYearDdYyy {#DayOfYearDdYyy}
```
public static final int DayOfYearDdYyy
```


Exempel är 77 '10, 78 '10

### DayOfYearDdYyyy {#DayOfYearDdYyyy}
```
public static final int DayOfYearDdYyyy
```


Exempel är 77 2010, 78 2010

### HalfYearFromEndH {#HalfYearFromEndH}
```
public static final int HalfYearFromEndH
```


Exempel är 2, 1, -1, -2. Halvår från projektets slutdatum.

### HalfYearFromEndHalfH {#HalfYearFromEndHalfH}
```
public static final int HalfYearFromEndHalfH
```


Exempel är Halv 2, Halv 1, Halv -1, Halv -2

### HalfYearFromEndHh {#HalfYearFromEndHh}
```
public static final int HalfYearFromEndHh
```


Exempel är H2, H1, H-1, H-2

### HalfYearFromStartH {#HalfYearFromStartH}
```
public static final int HalfYearFromStartH
```


Exempel är -2, -1, 1, 2. Halvår från projektets startdatum.

### HalfYearFromStartHalfH {#HalfYearFromStartHalfH}
```
public static final int HalfYearFromStartHalfH
```


Exempel är Halv -2, Halv -1, Halv 1, Halv 2

### HalfYearFromStartHh {#HalfYearFromStartHh}
```
public static final int HalfYearFromStartHh
```


Exempel är H-2, H-1, H1, H2

### HalfYearH {#HalfYearH}
```
public static final int HalfYearH
```


Exempel är 1, 2. Kräver att tidsenheten är TimescaleHalfYears.

### HalfYearHHyy {#HalfYearHHyy}
```
public static final int HalfYearHHyy
```


Exempel är 1H10, 2H10

### HalfYearHh {#HalfYearHh}
```
public static final int HalfYearHh
```


Exempel är H1, H2

### HalfYearHhYyy {#HalfYearHhYyy}
```
public static final int HalfYearHhYyy
```


Exempel är H1 '10, H2 '10

### HalfYearHhhHalf {#HalfYearHhhHalf}
```
public static final int HalfYearHhhHalf
```


Exempel är 1:a Halv, 2:a Halv

### HalfYearHlfH {#HalfYearHlfH}
```
public static final int HalfYearHlfH
```


Exempel är Halv 1, Halv 2

### HalfYearHlfHYyyy {#HalfYearHlfHYyyy}
```
public static final int HalfYearHlfHYyyy
```


Exempel är Halv 1, 2010; Halv 2, 2010

### HourDddMmmDdHhAm {#HourDddMmmDdHhAm}
```
public static final int HourDddMmmDdHhAm
```


Exempel är ons 18 mar, 08:00; ons 18 mar, 09:00. Kräver att tidsenheten är TimescaleHours.

### HourFromEndHh {#HourFromEndHh}
```
public static final int HourFromEndHh
```


Exempel är 3, 2, 1, -1, -2 timmar från projektets slut.

### HourFromEndHhh {#HourFromEndHhh}
```
public static final int HourFromEndHhh
```


Exempel är H3, H2, H1, H-1, H-2

### HourFromEndHourHh {#HourFromEndHourHh}
```
public static final int HourFromEndHourHh
```


Exempel är Timme 3, Timme 2, Timme 1, Timme -1, Timme -2

### HourFromStartHh {#HourFromStartHh}
```
public static final int HourFromStartHh
```


Exempel är -2, -1, 1, 2, 3 timmar från projektets start.

### HourFromStartHhh {#HourFromStartHhh}
```
public static final int HourFromStartHhh
```


Exempel är H-2, H-1, H1, H2, H3

### HourFromStartHourHh {#HourFromStartHourHh}
```
public static final int HourFromStartHourHh
```


Exempel är Timme -2, Timme -1, Timme 1, Timme 2, Timme 3

### HourHh {#HourHh}
```
public static final int HourHh
```


Exempel är 8, 9, 10, 11

### HourHhAm {#HourHhAm}
```
public static final int HourHhAm
```


Exempel är 8 fm, 9 fm

### HourHhMmAm {#HourHhMmAm}
```
public static final int HourHhMmAm
```


Exempel är 8:00 AM, 9:00 AM

### HourMmDdHhAm {#HourMmDdHhAm}
```
public static final int HourMmDdHhAm
```


Exempel är 3/18 8 AM, 3/18 9 AM

### HourMmmDdHhAm {#HourMmmDdHhAm}
```
public static final int HourMmmDdHhAm
```


Exempel är Mar 18, 8 AM; Mar 18, 9 AM

### MinuteFromEndMinuteMm {#MinuteFromEndMinuteMm}
```
public static final int MinuteFromEndMinuteMm
```


Exempel är Minute 181, Minute 180, ..., Minute 1, Minute -1 från projektets slut.

### MinuteFromEndMm {#MinuteFromEndMm}
```
public static final int MinuteFromEndMm
```


Exempel är 181, 180, ..., 1, -1

### MinuteFromEndMmm {#MinuteFromEndMmm}
```
public static final int MinuteFromEndMmm
```


Exempel är M181, M180, ..., M1, M-1

### MinuteFromStartMinuteMm {#MinuteFromStartMinuteMm}
```
public static final int MinuteFromStartMinuteMm
```


Exempel är Minut -2, Minut -1, Minut 1, ... Minut 180 från projektets start.

### MinuteFromStartMm {#MinuteFromStartMm}
```
public static final int MinuteFromStartMm
```


Exempel är -2, -1, 1, ..., 180

### MinuteFromStartMmm {#MinuteFromStartMmm}
```
public static final int MinuteFromStartMmm
```


Exempel är M-2, M-1, M1, ..., M180

### MinuteHhMmAm {#MinuteHhMmAm}
```
public static final int MinuteHhMmAm
```


Exempel är 08:00, 08:01, 08:02. Kräver att tidsenheten är TimescaleMinutes.

### MinuteMm {#MinuteMm}
```
public static final int MinuteMm
```


Exempel är 0, 1, 2, ..., 59 minuter

### MonthFromEndMm {#MonthFromEndMm}
```
public static final int MonthFromEndMm
```


Exempel är 2, 1, -1, -2 månader från projektets slut.

### MonthFromEndMmm {#MonthFromEndMmm}
```
public static final int MonthFromEndMmm
```


Exempel är M2, M1, M-1, M-2

### MonthFromEndMonthMm {#MonthFromEndMonthMm}
```
public static final int MonthFromEndMonthMm
```


Exempel är Month 2, Month 1, Month -1, Month -2

### MonthFromStartMm {#MonthFromStartMm}
```
public static final int MonthFromStartMm
```


Exempel är -2, -2, 1, 2 månader från projektets start.

### MonthFromStartMmm {#MonthFromStartMmm}
```
public static final int MonthFromStartMmm
```


Exempel är M-2, M-1, M1, M2

### MonthFromStartMonthMm {#MonthFromStartMonthMm}
```
public static final int MonthFromStartMonthMm
```


Exempel är Month -2, Month -1, Month 1, Month 2

### MonthM {#MonthM}
```
public static final int MonthM
```


Exempel är M, A, M, J, J. Kräver att tidsenheten är TimescaleMonths.

### MonthMm {#MonthMm}
```
public static final int MonthMm
```


Exempel är 11, 12, 1, 2

### MonthMmYy {#MonthMmYy}
```
public static final int MonthMmYy
```


Exempel är 3/10, 4/10, 5/10

### MonthMmYyy {#MonthMmYyy}
```
public static final int MonthMmYyy
```


Exempel är 3 '10, 4 '10, 5 '10

### MonthMmm {#MonthMmm}
```
public static final int MonthMmm
```


Exempel är Mar, Apr, May

### MonthMmmYyy {#MonthMmmYyy}
```
public static final int MonthMmmYyy
```


Exempel är Mar '10, Apr '10, May '10

### MonthMmmm {#MonthMmmm}
```
public static final int MonthMmmm
```


Exempel är March, April, May

### MonthMmmmYyyy {#MonthMmmmYyyy}
```
public static final int MonthMmmmYyyy
```


Exempel är March 2010, April 2010, May 2010

### None {#None}
```
public static final int None
```


Inget datum visas.

### QuarterFromEndQ {#QuarterFromEndQ}
```
public static final int QuarterFromEndQ
```


Exempel är 5, 4, 3, 2, 1, -1 kvartal från projektets slut.

### QuarterFromEndQq {#QuarterFromEndQq}
```
public static final int QuarterFromEndQq
```


Exempel är Q5, Q4, Q3, Q2, Q1, Q-1

### QuarterFromEndQuarterQ {#QuarterFromEndQuarterQ}
```
public static final int QuarterFromEndQuarterQ
```


Exempel är Kvartal 5, Kvartal 4, Kvartal 3, Kvartal 2, Kvartal 1, Kvartal -1

### QuarterFromStartQ {#QuarterFromStartQ}
```
public static final int QuarterFromStartQ
```


Exempel är -5, -4, -3, -2, -1, 1 kvartal från projektets start.

### QuarterFromStartQq {#QuarterFromStartQq}
```
public static final int QuarterFromStartQq
```


Exempel är Q-5, Q-4, Q-3, Q-2, Q-1, Q1

### QuarterFromStartQuarterQ {#QuarterFromStartQuarterQ}
```
public static final int QuarterFromStartQuarterQ
```


Exempel är Kvartal -5, Kvartal -4, Kvartal -3, Kvartal -2, Kvartal -1, Kvartal 1

### QuarterQ {#QuarterQ}
```
public static final int QuarterQ
```


Exempel är 3, 4, 1. Kräver att tidsenheten är TimescaleQuarters.

### QuarterQQyy {#QuarterQQyy}
```
public static final int QuarterQQyy
```


Exempel är 3Q10, 4Q10, 1Q11

### QuarterQq {#QuarterQq}
```
public static final int QuarterQq
```


Exempel är Q3, Q4, Q1

### QuarterQqYyy {#QuarterQqYyy}
```
public static final int QuarterQqYyy
```


Exempel är Q3 '10, Q4 '10, Q1 '11

### QuarterQqqQuarter {#QuarterQqqQuarter}
```
public static final int QuarterQqqQuarter
```


Exempel är 3:e kvartalet, 1:a kvartalet

### QuarterQtrQ {#QuarterQtrQ}
```
public static final int QuarterQtrQ
```


Exempel är Qtr3, Qtr4, Qtr1

### QuarterQtrQYyyy {#QuarterQtrQYyyy}
```
public static final int QuarterQtrQYyyy
```


Exempel är Qtr3, 2010; Qtr4, 2010; Qtr1, 2011

### ThirdsOfMonthsDd {#ThirdsOfMonthsDd}
```
public static final int ThirdsOfMonthsDd
```


Exempel är 1, 11, 21, 1. Kräver att tidsenheten är TimescaleThirdsOfMonths.

### ThirdsOfMonthsDdd {#ThirdsOfMonthsDdd}
```
public static final int ThirdsOfMonthsDdd
```


Exempel är B, M, E, B

### ThirdsOfMonthsDddd {#ThirdsOfMonthsDddd}
```
public static final int ThirdsOfMonthsDddd
```


Exempel är Början, Mitten, Slutet, Början

### ThirdsOfMonthsMmDd {#ThirdsOfMonthsMmDd}
```
public static final int ThirdsOfMonthsMmDd
```


Exempel är 3/1.

### ThirdsOfMonthsMmDdYy {#ThirdsOfMonthsMmDdYy}
```
public static final int ThirdsOfMonthsMmDdYy
```


Exempel är 3/1/10.

### ThirdsOfMonthsMmDdd {#ThirdsOfMonthsMmDdd}
```
public static final int ThirdsOfMonthsMmDdd
```


Exempel är 3/B, 3/M, 3/E, 4/B

### ThirdsOfMonthsMmDddYy {#ThirdsOfMonthsMmDddYy}
```
public static final int ThirdsOfMonthsMmDddYy
```


Exempel är 3/B/10.

### ThirdsOfMonthsMmmDd {#ThirdsOfMonthsMmmDd}
```
public static final int ThirdsOfMonthsMmmDd
```


Exempel är 1 mars, 11 mars, 21 mars, 1 apr

### ThirdsOfMonthsMmmDdYy {#ThirdsOfMonthsMmmDdYy}
```
public static final int ThirdsOfMonthsMmmDdYy
```


Exempel är 1 mars, '10; 11 mars, '10; 21 mars, '10; 1 apr, 10

### ThirdsOfMonthsMmmDdd {#ThirdsOfMonthsMmmDdd}
```
public static final int ThirdsOfMonthsMmmDdd
```


Exempel är mars B, mars M, mars E, apr B

### ThirdsOfMonthsMmmDddYy {#ThirdsOfMonthsMmmDddYy}
```
public static final int ThirdsOfMonthsMmmDddYy
```


Exempel är mars B, '10; mars M, '10; mars E, '10; apr B '10

### ThirdsOfMonthsMmmmDd {#ThirdsOfMonthsMmmmDd}
```
public static final int ThirdsOfMonthsMmmmDd
```


Exempel är 1 mars, 11 mars, 21 mars, 1 april

### ThirdsOfMonthsMmmmDdYyyy {#ThirdsOfMonthsMmmmDdYyyy}
```
public static final int ThirdsOfMonthsMmmmDdYyyy
```


Exempel är 1 mars 2010; 11 mars 2010; 21 mars 2010; 1 april 2010

### ThirdsOfMonthsMmmmDddd {#ThirdsOfMonthsMmmmDddd}
```
public static final int ThirdsOfMonthsMmmmDddd
```


Exempel är mars början, mars mitten, mars slutet, april början

### ThirdsOfMonthsMmmmDdddYyyy {#ThirdsOfMonthsMmmmDdddYyyy}
```
public static final int ThirdsOfMonthsMmmmDdddYyyy
```


Exempel är mars början, 2010; mars mitten, 2010; mars slutet, 2010; april början, 2010

### WeekDayOfMonthDd {#WeekDayOfMonthDd}
```
public static final int WeekDayOfMonthDd
```


Exempel är 21, 28, 4

### WeekDddDd {#WeekDddDd}
```
public static final int WeekDddDd
```


Exempel är Sun 21, Sun 28, Sun 4. Kräver att tidsenheten är TimescaleWeeks.

### WeekDddMDd {#WeekDddMDd}
```
public static final int WeekDddMDd
```


Exempel är sön M 21, sön M 28, sön A 4

### WeekDddMmDd {#WeekDddMmDd}
```
public static final int WeekDddMmDd
```


Exempel är sön 3/21, sön 3/28, sön 4/4

### WeekDddMmDdYy {#WeekDddMmDdYy}
```
public static final int WeekDddMmDdYy
```


Exempel är sön 3/21/10, sön 3/28/10, sön 4/4/10

### WeekDddMmmDd {#WeekDddMmmDd}
```
public static final int WeekDddMmmDd
```


Exempel är sön mars 21, sön mars 28, sön apr 4

### WeekDddMmmDdYyy {#WeekDddMmmDdYyy}
```
public static final int WeekDddMmmDdYyy
```


Exempel är sön mars 21, '10; sön mars 28, '10; sön apr 4, '10

### WeekDddMmmmDd {#WeekDddMmmmDd}
```
public static final int WeekDddMmmmDd
```


Exempel är sön mars 21, sön mars 28, sön apr 4

### WeekDddMmmmDdYyy {#WeekDddMmmmDdYyy}
```
public static final int WeekDddMmmmDdYyy
```


Exempel är sön mars 21, '10; sön mars 28, '10; sön april 4, '10

### WeekDddWw {#WeekDddWw}
```
public static final int WeekDddWw
```


Exempel är sön 12, sön 13, sön 14

### WeekDdiMDd {#WeekDdiMDd}
```
public static final int WeekDdiMDd
```


Exempel är sön M 21, sön M 28, sön A 4

### WeekDdiMmDd {#WeekDdiMmDd}
```
public static final int WeekDdiMmDd
```


Exempel är Su 3/21. Su 3/28, Su 4/4

### WeekDdiMmmDd {#WeekDdiMmmDd}
```
public static final int WeekDdiMmmDd
```


Exempel är sön mars 21, sön mars 28, sön apr 4

### WeekDiMDd {#WeekDiMDd}
```
public static final int WeekDiMDd
```


Exempel är sön M 21, sön M 28, sön A 4

### WeekDiMmDd {#WeekDiMmDd}
```
public static final int WeekDiMmDd
```


Exempel är sön 3/21, sön 3/28, sön 4/4

### WeekDiMmmDd {#WeekDiMmmDd}
```
public static final int WeekDiMmmDd
```


Exempel är sön mars 21, sön mars 28, sön apr 4

### WeekFromEndWeekWw {#WeekFromEndWeekWw}
```
public static final int WeekFromEndWeekWw
```


Exempel är Vecka 2, Vecka 1, Vecka -1 från projektets slut.

### WeekFromEndWw {#WeekFromEndWw}
```
public static final int WeekFromEndWw
```


Exempel är 2, 1, -1

### WeekFromEndWww {#WeekFromEndWww}
```
public static final int WeekFromEndWww
```


Exempel är W2, W1, W-1

### WeekFromStartWeekWw {#WeekFromStartWeekWw}
```
public static final int WeekFromStartWeekWw
```


Exempel är Vecka -1, Vecka 1, Vecka 2 från projektets start.

### WeekFromStartWw {#WeekFromStartWw}
```
public static final int WeekFromStartWw
```


Exempel är -1, 1, 2

### WeekFromStartWww {#WeekFromStartWww}
```
public static final int WeekFromStartWww
```


Exempel är W-1, W1, W2

### WeekMDd {#WeekMDd}
```
public static final int WeekMDd
```


Exempel är M21, M28, A 4

### WeekMmDd {#WeekMmDd}
```
public static final int WeekMmDd
```


Exempel är 3/21, 3/28, 4/4

### WeekMmDdYy {#WeekMmDdYy}
```
public static final int WeekMmDdYy
```


Exempel är '3/21/10'.

### WeekMmmDd {#WeekMmmDd}
```
public static final int WeekMmmDd
```


Exempel är 21 mar, 28 mar, 4 apr

### WeekMmmDdYyy {#WeekMmmDdYyy}
```
public static final int WeekMmmDdYyy
```


Exempel är 21 mar, '10; 28 mar, '10; 4 apr, '10

### WeekMmmmDd {#WeekMmmmDd}
```
public static final int WeekMmmmDd
```


Exempel är 21 mars, 28 mars, 4 april

### WeekMmmmDdYyyy {#WeekMmmmDdYyyy}
```
public static final int WeekMmmmDdYyyy
```


Exempel är 21 mars, 2010; 28 mars, 2010; 4 april, 2010

### WeekNumberDdWw {#WeekNumberDdWw}
```
public static final int WeekNumberDdWw
```


Exempel är 1 12, 1 13, 1 14 (dag 1 i vecka 12, dag 1 i vecka 13, och så vidare)

### WeekNumberWw {#WeekNumberWw}
```
public static final int WeekNumberWw
```


Exempel är 12, 13, 14

### YearFromEndYearYy {#YearFromEndYearYy}
```
public static final int YearFromEndYearYy
```


Exempel är År 2, År 1, År -1 från projektets slut.

### YearFromEndYy {#YearFromEndYy}
```
public static final int YearFromEndYy
```


Exempel är 2, 1, -1

### YearFromEndYyy {#YearFromEndYyy}
```
public static final int YearFromEndYyy
```


Exempel är Y2, Y1, Y-1

### YearFromStartYearYy {#YearFromStartYearYy}
```
public static final int YearFromStartYearYy
```


Exempel är År -1, År 1, År 2 från projektets start.

### YearFromStartYy {#YearFromStartYy}
```
public static final int YearFromStartYy
```


Exempel är -1, 1, 2

### YearFromStartYyy {#YearFromStartYyy}
```
public static final int YearFromStartYyy
```


Exempel är Y-1, Y1, Y2

### YearYy {#YearYy}
```
public static final int YearYy
```


Exempel är 10, 11, 12. Kräver att tidsenheten är TimescaleYears.

### YearYyy {#YearYyy}
```
public static final int YearYyy
```


Exempel är '10, '11, '12

### YearYyyy {#YearYyyy}
```
public static final int YearYyyy
```


Exempel är 2010, 2011, 2012

