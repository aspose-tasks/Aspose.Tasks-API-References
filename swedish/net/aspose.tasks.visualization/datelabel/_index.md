---
title: Enum DateLabel
second_title: Aspose.Tasks för .NET API-referens
description: Aspose.Tasks.Visualization.DateLabel uppräkning. Anger visningsformatet för datum och tidsetiketter i en tidsskala.
type: docs
weight: 2650
url: /sv/net/aspose.tasks.visualization/datelabel/
---
## DateLabel enumeration

Anger visningsformatet för datum- och tidsetiketter i en tidsskala.

```csharp
public enum DateLabel
```

### Värderingar

| namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `35` | Inget datum visas. |
| DayDdd | `19` | Exempel är mån, ti. |
| DayDddDd | `105` | Exempel är mån 30, ti 1 |
| DayDddMDd | `112` | Exempel är mån S 30, ti O 1 |
| DayDddMmDd | `108` | Exempel är mån 30/9, ti 10/1 |
| DayDddMmDdYy | `52` | Exempel är mån 9/30/02, ti 10/1/02 |
| DayDddMmmDd | `23` | Exempel är mån 30 sep, tis 1 okt |
| DayDddMmmDdYyy | `22` | Exempel är mån 30 sep '02, tis 1 okt '02 |
| DayDddMmmmDd | `111` | Exempel är mån 30 september, tis 1 oktober |
| DayDddd | `18` | Exempel är tisdag, onsdag. |
| DayDdi | `119` | Exempel är Mo, Tu |
| DayDdiDd | `106` | Exempel är Mo 30, Tu 1 |
| DayDdiMDd | `113` | Exempel är Mo S 30, Tu O 1 |
| DayDdiMmDd | `109` | Exempel är Mo 9/30, Tu 10/1 |
| DayDi | `20` | Exempel är M, T |
| DayDiDdSpace | `107` | Exempel är M 30, T 1 |
| DayDiMDd | `114` | Exempel är MS 30, TO 1 |
| DayDiMmDd | `110` | Exempel är M 9/30, T 10/1 |
| DayDiDdNoSpace | `121` | Exempel är M30, T1 |
| DayMDd | `115` | Exempel är S 30, O 1 |
| DayMmDd | `27` | Exempel är 9/30, 10/1 |
| DayMmDdYy | `26` | Exempel är 9/30/02, 10/1/02 |
| DayMmmDd | `25` | Exempel är 30 september, 1 oktober |
| DayMmmDdYyy | `24` | Exempel är 30 sep '02, 10 okt '02 |
| DayFromEndDayDd | `41` | Exempel är dag 2, dag 1, dag -1, dag -2 från projektets slut. |
| DayFromEndDd | `54` | Exempel är 2, 1, -1, -2 |
| DayFromEndDdd | `53` | Exempel är D2, D1, D-1, D-2 |
| DayFromStartDayDd | `40` | Exempel är Dag -2, Dag -1, Dag 1, Dag 2 från projektets start. |
| DayFromStartDd | `56` | Exempel är -2, -1, 1, 2 |
| DayFromStartDdd | `55` | Exempel är D-2, D-1, D1, D2 |
| DayOfMonthDd | `21` | Exempel är 30, 1 |
| DayOfYearDd | `118` | Exempel är 77, 78 |
| DayOfYearDdYyy | `116` | Exempel är 77 '10, 78 '10 |
| DayOfYearDdYyyy | `117` | Exempel är 77 2010, 78 2010 |
| DayDdMmYyyy | `256` | Exempel är 19/07/2016. |
| HalfYearH | `128` | Exempel är 1, 2. Kräver att tidsenheten är TimescaleHalfYears. |
| HalfYearHh | `127` | Exempel är H1, H2 |
| HalfYearHhYyy | `126` | Exempel är H1 '10, H2 '10 |
| HalfYearHhhHalf | `123` | Exempel är 1:a halvan, 2d halvan |
| HalfYearHHyy | `129` | Exempel är 1H10, 2H10 |
| HalfYearHlfH | `125` | Exempel är Half 1, Half 2 |
| HalfYearHlfHYyyy | `124` | Exempel är Half 1, 2010; Halv 2, 2010 |
| HalfYearFromEndH | `135` | Exempel är 2, 1, -1, -2. Halvår från projektets slutdatum. |
| HalfYearFromEndHalfH | `133` | Exempel är Half 2, Half 1, Half -1, Half -2 |
| HalfYearFromEndHh | `134` | Exempel är H2, H1, H-1, H-2 |
| HalfYearFromStartH | `132` | Exempel är -2, -1, 1, 2. Halvår från projektets startdatum. |
| HalfYearFromStartHalfH | `130` | Exempel är Half -2, Half -1, Half 1, Half 2 |
| HalfYearFromStartHh | `131` | Exempel är H-2, H-1, H1, H2 |
| HourDddMmmDdHhAm | `28` | Exempel är ons 18 mars kl. 8; ons 18 mars kl. 09.00. Kräver att tidsenheten är TimescaleHours. |
| HourHh | `32` | Exempel är 8, 9, 10, 11 |
| HourHhMmAm | `30` | Exempel är 8:00 AM, 9:00 AM |
| HourHhAm | `31` | Exempel är 8AM, 9AM |
| HourMmDdHhAm | `120` | Exempel är 3/18 8 AM, 3/18 9 AM |
| HourMmmDdHhAm | `29` | Exempel är 18 mars kl. 08.00; 18 mars, 9 AM |
| HourFromEndHh | `77` | Exempel är 3, 2, 1, -1, -2 timmar från projektets slut. |
| HourFromEndHhh | `76` | Exempel är H3, H2, H1, H-1, H-2 |
| HourFromEndHourHh | `39` | Exempel är timme 3, timme 2, timme 1, timme -1, timme -2 |
| HourFromStartHh | `79` | Exempel är -2, -1, 1, 2, 3 timmar från projektets start. |
| HourFromStartHhh | `78` | Exempel är H-2, H-1, H1, H2, H3 |
| HourFromStartHourHh | `38` | Exempel är Hour -2, Hour -1, Hour 1, Hour 2, Hour 3 |
| MinuteHhMmAm | `33` | Exempel är 8:00 AM, 8:01 AM, 8:02 AM. Kräver att tidsenheten är TimescaleMinutes. |
| MinuteMm | `34` | Exempel är 0, 1, 2, ..., 59 minuter |
| MinuteFromEndMinuteMm | `37` | Exempel är minut 181, minut 180, ..., minut 1, minut -1 från projektets slut. |
| MinuteFromEndMm | `81` | Exempel är 181, 180, ..., 1, -1 |
| MinuteFromEndMmm | `80` | Exempel är M181, M180, ..., M1, M-1 |
| MinuteFromStartMinuteMm | `36` | Exempel är Minut -2, Minut -1, Minut 1, ... Minut 180 från projektets start. |
| MinuteFromStartMm | `83` | Exempel är -2, -1, 1, ..., 180 |
| MinuteFromStartMmm | `82` | Exempel är M-2, M-1, M1, ..., M180 |
| MonthM | `11` | Exempel är M, A, M, J, J. Kräver att tidsenheten är TimescaleMonths. |
| MonthMm | `57` | Exempel är 11, 12, 1, 2 |
| MonthMmYy | `86` | Exempel är 3/10, 4/10, 5/10 |
| MonthMmYyy | `85` | Exempel är 3 '10, 4 '10, 5 '10 |
| MonthMmm | `10` | Exempel är Mar, Apr, May |
| MonthMmmYyy | `8` | Exempel är mars '10, apr '10, maj '10 |
| MonthMmmm | `9` | Exempel är mars, april, maj |
| MonthMmmmYyyy | `7` | Exempel är mars 2010, april 2010, maj 2010 |
| MonthFromEndMm | `59` | Exempel är 2, 1, -1, -2 månader från projektets slut. |
| MonthFromEndMmm | `58` | Exempel är M2, M1, M-1, M-2 |
| MonthFromEndMonthMm | `45` | Exempel är månad 2, månad 1, månad -1, månad -2 |
| MonthFromStartMm | `61` | Exempel är -2, -2, 1, 2 månader från projektets start. |
| MonthFromStartMmm | `60` | Exempel är M-2, M-1, M1, M2 |
| MonthFromStartMonthMm | `44` | Exempel är månad -2, månad -1, månad 1, månad 2 |
| QuarterQ | `62` | Exempel är 3, 4, 1. Kräver att tidsenheten är TimescaleQuarters. |
| QuarterQq | `6` | Exempel är Q3, Q4, Q1 |
| QuarterQqYyy | `4` | Exempel är Q3 '10, Q4 '10, Q1 '11 |
| QuarterQqqQuarter | `2` | Exempel är 3:e kvartalet, 1:a kvartalet |
| QuarterQQyy | `51` | Exempel är 3Q10, 4Q10, 1Q11 |
| QuarterQtrQ | `5` | Exempel är Qtr3, Qtr4, Qtr1 |
| QuarterQtrQYyyy | `3` | Exempel är Qtr3, 2010; Qtr4, 2010; Qtr1, 2011 |
| QuarterFromEndQ | `64` | Exempel är 5, 4, 3, 2, 1, -1 kvartal från projektets slut. |
| QuarterFromEndQq | `63` | Exempel är Q5, Q4, Q3, Q2, Q1, Q-1 |
| QuarterFromEndQuarterQ | `47` | Exempel är Quarter 5, Quarter 4, Quarter 3, Quarter 2, Quarter 1, Quarter -1 |
| QuarterFromStartQ | `66` | Exempel är -5, -4, -3, -2, -1, 1 kvartal från projektets start. |
| QuarterFromStartQq | `65` | Exempel är Q-5, Q-4, Q-3, Q-2, Q-1, Q1 |
| QuarterFromStartQuarterQ | `46` | Exempel är Quarter -5, Quarter -4, Quarter -3, Quarter -2, Quarter -1, Quarter 1 |
| ThirdsOfMonthsDd | `136` | Exempel är 1, 11, 21, 1. Kräver att tidsenheten är TimescaleThirdsOfMonths. |
| ThirdsOfMonthsDdd | `137` | Exempel är B, M, E, B |
| ThirdsOfMonthsDddd | `138` | Exempel är Beginning, Middle, End, Beginning |
| ThirdsOfMonthsMmDd | `139` | Exempel är 3/1. |
| ThirdsOfMonthsMmDdYy | `145` | Exempel är 3/1/10. |
| ThirdsOfMonthsMmDdd | `140` | Exempel är 3/B, 3/M, 3/E, 4/B |
| ThirdsOfMonthsMmDddYy | `146` | Exempel är 3/B/10. |
| ThirdsOfMonthsMmmDd | `142` | Exempel är 1 mars, 11 mars, 21 mars, 1 april |
| ThirdsOfMonthsMmmDdYy | `147` | Exempel är 1 mars '10; 11 mars '10; 21 mars '10; 1 april, 10 |
| ThirdsOfMonthsMmmDdd | `143` | Exempel är Mar B, Mar M, Mar E, Apr B |
| ThirdsOfMonthsMmmDddYy | `148` | Exempel är Mar B, '10; Mar M, '10; Mar E, '10; apr B '10 |
| ThirdsOfMonthsMmmmDd | `144` | Exempel är 1 mars, 11 mars, 21 mars, 1 april |
| ThirdsOfMonthsMmmmDdYyyy | `149` | Exempel är 1 mars 2010; 11 mars 2010; 21 mars 2010; 1 april 2010 |
| ThirdsOfMonthsMmmmDddd | `141` | Exempel är mars början, mars mitten, mars slut, april början |
| ThirdsOfMonthsMmmmDdddYyyy | `150` | Exempel är början av mars 2010; Mars mitten, 2010; Slutet av mars 2010; April Början, 2010 |
| WeekDddDd | `88` | Exempel är sön 21, sön 28, sön 4. Kräver att tidsenheten är TimescaleWeeks. |
| WeekDddMDd | `97` | Exempel är Sun M 21, Sun M 28, Sun A 4 |
| WeekDddMmDd | `90` | Exempel är sön 21/3, sön 28/3, sön 4/4 |
| WeekDddMmDdYy | `100` | Exempel är sön 21/3/10, sön 28/3/10, sön 4/4/10 |
| WeekDddMmmDd | `93` | Exempel är sön 21 mars, sön 28 mars, sön 4 april |
| WeekDddMmmDdYyy | `101` | Exempel är sön 21 mars '10; Sön 28 mars '10; Sön 4 april, '10 |
| WeekDddMmmmDd | `96` | Exempel är sön 21 mars, sön 28 mars, sön 4 april |
| WeekDddMmmmDdYyy | `102` | Exempel är sön 21 mars '10; Sön 28 mars '10; Sön 4 april, '10 |
| WeekDddWw | `103` | Exempel är sön 12, sön 13, sön 14 |
| WeekDdiMDd | `98` | Exempel är Su M 21, Su M 28, Su A 4 |
| WeekDdiMmDd | `91` | Exempel är Su 3/21. Sö 28/3, Sö 4/4 |
| WeekDdiMmmDd | `94` | Exempel är Su 21 Mar, Su 28 Mar, Su 4 Apr |
| WeekDiMDd | `99` | Exempel är SM 21, SM 28, SA 4 |
| WeekDiMmDd | `92` | Exempel är S 3/21, S 3/28, S 4/4 |
| WeekDiMmmDd | `95` | Exempel är S 21 mars, S 28 mars, S 4 april |
| WeekMDd | `89` | Exempel är M21, M28, A 4 |
| WeekMmDd | `17` | Exempel är 3/21, 3/28, 4/4 |
| WeekMmDdYy | `16` | Exempel är '3/21/10'. |
| WeekMmmDd | `15` | Exempel är 21 mars, 28 mars, 4 april |
| WeekMmmDdYyy | `13` | Exempel är 21 mars '10; 28 mars '10; 4 april, '10 |
| WeekMmmmDd | `14` | Exempel är 21 mars, 28 mars, 4 april |
| WeekMmmmDdYyyy | `12` | Exempel är 21 mars 2010; 28 mars 2010; 4 april 2010 |
| WeekDayOfMonthDd | `87` | Exempel är 21, 28, 4 |
| WeekFromEndWeekWw | `43` | Exempel är vecka 2, vecka 1, vecka -1 från projektets slut. |
| WeekFromEndWw | `68` | Exempel är 2, 1, -1 |
| WeekFromEndWww | `67` | Exempel är W2, W1, W-1 |
| WeekFromStartWeekWw | `42` | Exempel är vecka -1, vecka 1, vecka 2 från projektets start. |
| WeekFromStartWw | `70` | Exempel är -1, 1, 2 |
| WeekFromStartWww | `69` | Exempel är W-1, W1, W2 |
| WeekNumberDdWw | `104` | Exempel är 1 12, 1 13, 1 14 (dag 1 i vecka 12, dag 1 i vecka 13 och så vidare) |
| WeekNumberWw | `50` | Exempel är 12, 13, 14 |
| YearYy | `75` | Exempel är 10, 11, 12. Kräver att tidsenheten är TimescaleYears. |
| YearYyy | `1` | Exempel är '10, '11, '12 |
| YearYyyy | `0` | Exempel är 2010, 2011, 2012 |
| YearFromEndYearYy | `49` | Exempel är år 2, år 1, år -1 från projektets slut. |
| YearFromEndYy | `72` | Exempel är 2, 1, -1 |
| YearFromEndYyy | `71` | Exempel är Y2, Y1, Y-1 |
| YearFromStartYearYy | `48` | Exempel är år -1, år 1, år 2 från projektets start. |
| YearFromStartYy | `74` | Exempel är -1, 1, 2 |
| YearFromStartYyy | `73` | Exempel är Y-1, Y1, Y2 |

### Se även

* namnutrymme [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* hopsättning [Aspose.Tasks](../../)


