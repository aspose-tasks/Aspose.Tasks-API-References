---
title: DateLabel
second_title: Aspose.Tasks für .NET-API-Referenz
description: Gibt das Anzeigeformat für Datums- und Zeitbeschriftungen in einer Zeitskala an.
type: docs
weight: 2630
url: /de/net/aspose.tasks.visualization/datelabel/
---
## DateLabel enumeration

Gibt das Anzeigeformat für Datums- und Zeitbeschriftungen in einer Zeitskala an.

```csharp
public enum DateLabel
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `35` | Es wird kein Datum angezeigt. |
| DayDdd | `19` | Beispiele sind Mo, Di. |
| DayDddDd | `105` | Beispiele sind Mo 30, Di 1 |
| DayDddMDd | `112` | Beispiele sind Mo S 30, Di O 1 |
| DayDddMmDd | `108` | Beispiele sind Mo 30.9., Di 1.10. |
| DayDddMmDdYy | `52` | Beispiele sind Mo 30.09.02, Di 01.10.02 |
| DayDddMmmDd | `23` | Beispiele sind Mo 30. Sep, Di 1. Okt |
| DayDddMmmDdYyy | `22` | Beispiele sind Mo 30. Sep '02, Di 1. Okt '02 |
| DayDddMmmmDd | `111` | Beispiele sind Mo, 30. September, Di, 1. Oktober |
| DayDddd | `18` | Beispiele sind Dienstag, Mittwoch. |
| DayDdi | `119` | Beispiele sind Mo, Di |
| DayDdiDd | `106` | Beispiele sind Mo 30, Di 1 |
| DayDdiMDd | `113` | Beispiele sind Mo S 30, Tu O 1 |
| DayDdiMmDd | `109` | Beispiele sind Mo 30.9., Di 1.10. |
| DayDi | `20` | Beispiele sind M, T |
| DayDiDdSpace | `107` | Beispiele sind M 30, T 1 |
| DayDiMDd | `114` | Beispiele sind MS 30, TO 1 |
| DayDiMmDd | `110` | Beispiele sind M 9/30, T 10/1 |
| DayDiDdNoSpace | `121` | Beispiele sind M30, T1 |
| DayMDd | `115` | Beispiele sind S 30, O 1 |
| DayMmDd | `27` | Beispiele sind 9/30, 10/1 |
| DayMmDdYy | `26` | Beispiele sind 30.09.02, 01.10.02 |
| DayMmmDd | `25` | Beispiele sind 30. September, 1. Oktober |
| DayMmmDdYyy | `24` | Beispiele sind 30. Sep. '02, 10. Okt. '02 |
| DayFromEndDayDd | `41` | Beispiele sind Tag 2, Tag 1, Tag -1, Tag -2 ab Projektende. |
| DayFromEndDd | `54` | Beispiele sind 2, 1, -1, -2 |
| DayFromEndDdd | `53` | Beispiele sind D2, D1, D-1, D-2 |
| DayFromStartDayDd | `40` | Beispiele sind Tag -2, Tag -1, Tag 1, Tag 2 ab Projektstart. |
| DayFromStartDd | `56` | Beispiele sind -2, -1, 1, 2 |
| DayFromStartDdd | `55` | Beispiele sind D-2, D-1, D1, D2 |
| DayOfMonthDd | `21` | Beispiele sind 30, 1 |
| DayOfYearDd | `118` | Beispiele sind 77, 78 |
| DayOfYearDdYyy | `116` | Beispiele sind 77 '10, 78 '10 |
| DayOfYearDdYyyy | `117` | Beispiele sind 77 2010, 78 2010 |
| DayDdMmYyyy | `256` | Beispiel ist 19.07.2016. |
| HalfYearH | `128` | Beispiele sind 1, 2. Erfordert die Zeiteinheit TimescaleHalfYears. |
| HalfYearHh | `127` | Beispiele sind H1, H2 |
| HalfYearHhYyy | `126` | Beispiele sind H1 '10, H2 '10 |
| HalfYearHhhHalf | `123` | Beispiele sind 1. Hälfte, 2. Hälfte |
| HalfYearHHyy | `129` | Beispiele sind 1H10, 2H10 |
| HalfYearHlfH | `125` | Beispiele sind Hälfte 1, Hälfte 2 |
| HalfYearHlfHYyyy | `124` | Beispiele sind 1. Halbjahr 2010; Hälfte 2, 2010 |
| HalfYearFromEndH | `135` | Beispiele sind 2, 1, -1, -2. Halbe Jahre ab Enddatum des Projekts. |
| HalfYearFromEndHalfH | `133` | Beispiele sind Halb 2, Halb 1, Halb -1, Halb -2 |
| HalfYearFromEndHh | `134` | Beispiele sind H2, H1, H-1, H-2 |
| HalfYearFromStartH | `132` | Beispiele sind -2, -1, 1, 2. Halbe Jahre ab Projektstartdatum. |
| HalfYearFromStartHalfH | `130` | Beispiele sind Half -2, Half -1, Half 1, Half 2 |
| HalfYearFromStartHh | `131` | Beispiele sind H-2, H-1, H1, H2 |
| HourDddMmmDdHhAm | `28` | Beispiele sind Mittwoch, 18. März, 8 Uhr; Mi 18. März, 9 Uhr. Erfordert die Zeiteinheit TimescaleHours. |
| HourHh | `32` | Beispiele sind 8, 9, 10, 11 |
| HourHhMmAm | `30` | Beispiele sind 8:00 Uhr, 9:00 Uhr |
| HourHhAm | `31` | Beispiele sind 8:00, 9:00 |
| HourMmDdHhAm | `120` | Beispiele sind 18.3. 8 Uhr, 18.3. 9 Uhr |
| HourMmmDdHhAm | `29` | Beispiele sind 18. März, 8 Uhr; 18. März, 9 Uhr |
| HourFromEndHh | `77` | Beispiele sind 3, 2, 1, -1, -2 Stunden nach Projektende. |
| HourFromEndHhh | `76` | Beispiele sind H3, H2, H1, H-1, H-2 |
| HourFromEndHourHh | `39` | Beispiele sind Stunde 3, Stunde 2, Stunde 1, Stunde -1, Stunde -2 |
| HourFromStartHh | `79` | Beispiele sind -2, -1, 1, 2, 3 Stunden ab Projektstart. |
| HourFromStartHhh | `78` | Beispiele sind H-2, H-1, H1, H2, H3 |
| HourFromStartHourHh | `38` | Beispiele sind Stunde -2, Stunde -1, Stunde 1, Stunde 2, Stunde 3 |
| MinuteHhMmAm | `33` | Beispiele sind 8:00 Uhr, 8:01 Uhr, 8:02 Uhr. Erfordert die Zeiteinheit TimescaleMinutes. |
| MinuteMm | `34` | Beispiele sind 0, 1, 2, ..., 59 Minuten |
| MinuteFromEndMinuteMm | `37` | Beispiele sind Minute 181, Minute 180, ..., Minute 1, Minute -1 vom Projektende. |
| MinuteFromEndMm | `81` | Beispiele sind 181, 180, ..., 1, -1 |
| MinuteFromEndMmm | `80` | Beispiele sind M181, M180, ..., M1, M-1 |
| MinuteFromStartMinuteMm | `36` | Beispiele sind Minute -2, Minute -1, Minute 1, ... Minute 180 ab Projektstart. |
| MinuteFromStartMm | `83` | Beispiele sind -2, -1, 1, ..., 180 |
| MinuteFromStartMmm | `82` | Beispiele sind M-2, M-1, M1, ..., M180 |
| MonthM | `11` | Beispiele sind M, A, M, J, J. Erfordert die Zeiteinheit TimescaleMonths. |
| MonthMm | `57` | Beispiele sind 11, 12, 1, 2 |
| MonthMmYy | `86` | Beispiele sind 3/10, 4/10, 5/10 |
| MonthMmYyy | `85` | Beispiele sind 3 '10, 4 '10, 5 '10 |
| MonthMmm | `10` | Beispiele sind März, April, Mai |
| MonthMmmYyy | `8` | Beispiele sind Mär '10, Apr '10, Mai '10 |
| MonthMmmm | `9` | Beispiele sind März, April, Mai |
| MonthMmmmYyyy | `7` | Beispiele sind März 2010, April 2010, Mai 2010 |
| MonthFromEndMm | `59` | Beispiele sind 2, 1, -1, -2 Monate ab Projektende. |
| MonthFromEndMmm | `58` | Beispiele sind M2, M1, M-1, M-2 |
| MonthFromEndMonthMm | `45` | Beispiele sind Monat 2, Monat 1, Monat -1, Monat -2 |
| MonthFromStartMm | `61` | Beispiele sind -2, -2, 1, 2 Monate ab Projektstart. |
| MonthFromStartMmm | `60` | Beispiele sind M-2, M-1, M1, M2 |
| MonthFromStartMonthMm | `44` | Beispiele sind Monat -2, Monat -1, Monat 1, Monat 2 |
| QuarterQ | `62` | Beispiele sind 3, 4, 1. Erfordert die Zeiteinheit TimescaleQuarters. |
| QuarterQq | `6` | Beispiele sind Q3, Q4, Q1 |
| QuarterQqYyy | `4` | Beispiele sind Q3 '10, Q4 '10, Q1 '11 |
| QuarterQqqQuarter | `2` | Beispiele sind 3. Quartal, 1. Quartal |
| QuarterQQyy | `51` | Beispiele sind 3Q10, 4Q10, 1Q11 |
| QuarterQtrQ | `5` | Beispiele sind Qtr3, Qtr4, Qtr1 |
| QuarterQtrQYyyy | `3` | Beispiele sind Qtr3, 2010; 4. Quartal 2010; Qtr1, 2011 |
| QuarterFromEndQ | `64` | Beispiele sind 5, 4, 3, 2, 1, -1 Quartal vor Projektende. |
| QuarterFromEndQq | `63` | Beispiele sind Q5, Q4, Q3, Q2, Q1, Q-1 |
| QuarterFromEndQuarterQ | `47` | Beispiele sind Quartal 5, Quartal 4, Quartal 3, Quartal 2, Quartal 1, Quartal -1 |
| QuarterFromStartQ | `66` | Beispiele sind -5, -4, -3, -2, -1, 1 Quartal ab Projektstart. |
| QuarterFromStartQq | `65` | Beispiele sind Q-5, Q-4, Q-3, Q-2, Q-1, Q1 |
| QuarterFromStartQuarterQ | `46` | Beispiele sind Quartal -5, Quartal -4, Quartal -3, Quartal -2, Quartal -1, Quartal 1 |
| ThirdsOfMonthsDd | `136` | Beispiele sind 1, 11, 21, 1. Erfordert die Zeiteinheit TimescaleThirdsOfMonths. |
| ThirdsOfMonthsDdd | `137` | Beispiele sind B, M, E, B |
| ThirdsOfMonthsDddd | `138` | Beispiele sind Anfang, Mitte, Ende, Anfang |
| ThirdsOfMonthsMmDd | `139` | Beispiel ist 3/1. |
| ThirdsOfMonthsMmDdYy | `145` | Beispiel ist 1.3.10. |
| ThirdsOfMonthsMmDdd | `140` | Beispiele sind 3/B, 3/M, 3/E, 4/B |
| ThirdsOfMonthsMmDddYy | `146` | Beispiel ist 3/B/10. |
| ThirdsOfMonthsMmmDd | `142` | Beispiele sind 1. März, 11. März, 21. März, 1. April |
| ThirdsOfMonthsMmmDdYy | `147` | Beispiele sind 1. März '10; 11. März '10; 21. März '10; 1. April 10 |
| ThirdsOfMonthsMmmDdd | `143` | Beispiele sind Mrz B, Mrz M, Mrz E, Apr B |
| ThirdsOfMonthsMmmDddYy | `148` | Beispiele sind März B, '10; März M, '10; Mär E, '10; April B '10 |
| ThirdsOfMonthsMmmmDd | `144` | Beispiele sind 1. März, 11. März, 21. März, 1. April |
| ThirdsOfMonthsMmmmDdYyyy | `149` | Beispiele sind 1. März 2010; 11. März 2010; 21. März 2010; 1. April 2010 |
| ThirdsOfMonthsMmmmDddd | `141` | Beispiele sind Anfang März, Mitte März, Ende März, Anfang April |
| ThirdsOfMonthsMmmmDdddYyyy | `150` | Beispiele sind Anfang März 2010; März Mitte 2010; Ende März 2010; Anfang April, 2010 |
| WeekDddDd | `88` | Beispiele sind So 21, So 28, So 4. Erfordert die Zeiteinheit TimescaleWeeks. |
| WeekDddMDd | `97` | Beispiele sind Sonne M 21, Sonne M 28, Sonne A 4 |
| WeekDddMmDd | `90` | Beispiele sind So 21.3., So 28.3., So 4.4 |
| WeekDddMmDdYy | `100` | Beispiele sind So 21.3.10, So 28.3.10, So 4.4.10 |
| WeekDddMmmDd | `93` | Beispiele sind So 21. Mär, So 28. Mär, So 4. Apr |
| WeekDddMmmDdYyy | `101` | Beispiele sind Sun 21. März '10; So 28. März '10; So. 4. Apr. '10 |
| WeekDddMmmmDd | `96` | Beispiele sind So 21. März, So 28. März, So 4. April |
| WeekDddMmmmDdYyy | `102` | Beispiele sind Sonntag, 21. März '10; So 28. März '10; So 4. April '10 |
| WeekDddWw | `103` | Beispiele sind So 12, So 13, So 14 |
| WeekDdiMDd | `98` | Beispiele sind Su M 21, Su M 28, Su A 4 |
| WeekDdiMmDd | `91` | Beispiele sind So 21.3. So 28.3., So 4.4 |
| WeekDdiMmmDd | `94` | Beispiele sind So 21. März, So 28. März, So 4. April |
| WeekDiMDd | `99` | Beispiele sind SM 21, SM 28, SA 4 |
| WeekDiMmDd | `92` | Beispiele sind S 3/21, S 3/28, S 4/4 |
| WeekDiMmmDd | `95` | Beispiele sind S 21. März, S 28. März, S 4. April |
| WeekMDd | `89` | Beispiele sind M21, M28, A 4 |
| WeekMmDd | `17` | Beispiele sind 21.3., 28.3., 4.4 |
| WeekMmDdYy | `16` | Beispiel ist '21.3.10'. |
| WeekMmmDd | `15` | Beispiele sind 21. März, 28. März, 4. April |
| WeekMmmDdYyy | `13` | Beispiele sind 21. März '10; 28. März '10; 4. April '10 |
| WeekMmmmDd | `14` | Beispiele sind 21. März, 28. März, 4. April |
| WeekMmmmDdYyyy | `12` | Beispiele sind 21. März 2010; 28. März 2010; 4. April 2010 |
| WeekDayOfMonthDd | `87` | Beispiele sind 21, 28, 4 |
| WeekFromEndWeekWw | `43` | Beispiele sind Woche 2, Woche 1, Woche -1 ab Projektende. |
| WeekFromEndWw | `68` | Beispiele sind 2, 1, -1 |
| WeekFromEndWww | `67` | Beispiele sind W2, W1, W-1 |
| WeekFromStartWeekWw | `42` | Beispiele sind Woche -1, Woche 1, Woche 2 ab Projektstart. |
| WeekFromStartWw | `70` | Beispiele sind -1, 1, 2 |
| WeekFromStartWww | `69` | Beispiele sind W-1, W1, W2 |
| WeekNumberDdWw | `104` | Beispiele sind 1 12, 1 13, 1 14 (Tag 1 der Woche 12, Tag 1 der Woche 13 usw.) |
| WeekNumberWw | `50` | Beispiele sind 12, 13, 14 |
| YearYy | `75` | Beispiele sind 10, 11, 12. Erfordert die Zeiteinheit TimescaleYears. |
| YearYyy | `1` | Beispiele sind '10, '11, '12 |
| YearYyyy | `0` | Beispiele sind 2010, 2011, 2012 |
| YearFromEndYearYy | `49` | Beispiele sind Jahr 2, Jahr 1, Jahr -1 ab Projektende. |
| YearFromEndYy | `72` | Beispiele sind 2, 1, -1 |
| YearFromEndYyy | `71` | Beispiele sind Y2, Y1, Y-1 |
| YearFromStartYearYy | `48` | Beispiele sind Jahr -1, Jahr 1, Jahr 2 ab Projektstart. |
| YearFromStartYy | `74` | Beispiele sind -1, 1, 2 |
| YearFromStartYyy | `73` | Beispiele sind Y-1, Y1, Y2 |

### Siehe auch

* namensraum [Aspose.Tasks.Visualization](../../aspose.tasks.visualization)
* Montage [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
