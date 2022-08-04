---
title: DateLabel
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: Specifica il formato di visualizzazione per le etichette di data e ora in una scala cronologica.
type: docs
weight: 2630
url: /it/net/aspose.tasks.visualization/datelabel/
---
## DateLabel enumeration

Specifica il formato di visualizzazione per le etichette di data e ora in una scala cronologica.

```csharp
public enum DateLabel
```

### I valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `35` | Non viene visualizzata alcuna data. |
| DayDdd | `19` | Esempi sono lun, mar |
| DayDddDd | `105` | Esempi sono lun 30, mar 1 |
| DayDddMDd | `112` | Esempi sono Lun S 30, Mar O 1 |
| DayDddMmDd | `108` | Esempi sono lun 9/30, mar 10/10 |
| DayDddMmDdYy | `52` | Esempi sono Lun 30/09/02, Mar 01/10/02 |
| DayDddMmmDd | `23` | Esempi sono lun 30 settembre, mar 1 ottobre |
| DayDddMmmDdYyy | `22` | Esempi sono lun set 30 '02, mar 1 ottobre '02 |
| DayDddMmmmDd | `111` | Esempi sono lun 30 settembre, mar 1 ottobre |
| DayDddd | `18` | Esempi sono martedì, mercoledì. |
| DayDdi | `119` | Esempi sono Lu, Tu |
| DayDdiDd | `106` | Esempi sono Mo 30, Tu 1 |
| DayDdiMDd | `113` | Esempi sono Mo S 30, Tu O 1 |
| DayDdiMmDd | `109` | Esempi sono Lu 9/30, Mar 10/1 |
| DayDi | `20` | Esempi sono M, T |
| DayDiDdSpace | `107` | Esempi sono M 30, T 1 |
| DayDiMDd | `114` | Esempi sono MS 30, TO 1 |
| DayDiMmDd | `110` | Esempi sono M 9/30, T 10/1 |
| DayDiDdNoSpace | `121` | Esempi sono M30, T1 |
| DayMDd | `115` | Esempi sono S 30, O 1 |
| DayMmDd | `27` | Esempi sono 9/30, 10/1 |
| DayMmDdYy | `26` | Esempi sono 30/09/02, 01/10/02 |
| DayMmmDd | `25` | Esempi sono 30 settembre, 1 ottobre |
| DayMmmDdYyy | `24` | Esempi sono il 30 settembre '02, il 10 ottobre '02 |
| DayFromEndDayDd | `41` | Esempi sono il giorno 2, il giorno 1, il giorno -1, il giorno -2 dalla fine del progetto. |
| DayFromEndDd | `54` | Esempi sono 2, 1, -1, -2 |
| DayFromEndDdd | `53` | Esempi sono D2, D1, D-1, D-2 |
| DayFromStartDayDd | `40` | Esempi sono Giorno -2, Giorno -1, Giorno 1, Giorno 2 dall'inizio del progetto. |
| DayFromStartDd | `56` | Esempi sono -2, -1, 1, 2 |
| DayFromStartDdd | `55` | Esempi sono D-2, D-1, D1, D2 |
| DayOfMonthDd | `21` | Esempi sono 30, 1 |
| DayOfYearDd | `118` | Esempi sono 77, 78 |
| DayOfYearDdYyy | `116` | Esempi sono 77 '10, 78 '10 |
| DayOfYearDdYyyy | `117` | Esempi sono 77 2010, 78 2010 |
| DayDdMmYyyy | `256` | L'esempio è 19/07/2016. |
| HalfYearH | `128` | Gli esempi sono 1, 2. Richiede che l'unità di tempo sia TimescaleHalfYears. |
| HalfYearHh | `127` | Esempi sono H1, H2 |
| HalfYearHhYyy | `126` | Esempi sono H1 '10, H2 '10 |
| HalfYearHhhHalf | `123` | Esempi sono 1a metà, 2d metà |
| HalfYearHHyy | `129` | Esempi sono 1H10, 2H10 |
| HalfYearHlfH | `125` | Esempi sono Metà 1, Metà 2 |
| HalfYearHlfHYyyy | `124` | Esempi sono Half 1, 2010; Metà 2, 2010 |
| HalfYearFromEndH | `135` | Esempi sono 2, 1, -1, -2. Sei mesi dalla data di fine del progetto. |
| HalfYearFromEndHalfH | `133` | Esempi sono Metà 2, Metà 1, Metà -1, Metà -2 |
| HalfYearFromEndHh | `134` | Esempi sono H2, H1, H-1, H-2 |
| HalfYearFromStartH | `132` | Esempi sono -2, -1, 1, 2. Mezzi anni dalla data di inizio del progetto. |
| HalfYearFromStartHalfH | `130` | Esempi sono Metà -2, Metà -1, Metà 1, Metà 2 |
| HalfYearFromStartHh | `131` | Esempi sono H-2, H-1, H1, H2 |
| HourDddMmmDdHhAm | `28` | Esempi sono mercoledì 18 marzo, 8:00; mercoledì 18 marzo, 9:00. Richiede che l'unità di tempo sia TimescaleHours. |
| HourHh | `32` | Esempi sono 8, 9, 10, 11 |
| HourHhMmAm | `30` | Esempi sono 8:00, 9:00 |
| HourHhAm | `31` | Esempi sono 8:00, 9:00 |
| HourMmDdHhAm | `120` | Esempi sono 3/18 8 AM, 3/18 9 AM |
| HourMmmDdHhAm | `29` | Esempi sono 18 marzo, 8:00; 18 marzo, 9:00 |
| HourFromEndHh | `77` | Esempi sono 3, 2, 1, -1, -2 ore dalla fine del progetto. |
| HourFromEndHhh | `76` | Esempi sono H3, H2, H1, H-1, H-2 |
| HourFromEndHourHh | `39` | Esempi sono Ora 3, Ora 2, Ora 1, Ora -1, Ora -2 |
| HourFromStartHh | `79` | Esempi sono -2, -1, 1, 2, 3 ore dall'inizio del progetto. |
| HourFromStartHhh | `78` | Esempi sono H-2, H-1, H1, H2, H3 |
| HourFromStartHourHh | `38` | Esempi sono Ora -2, Ora -1, Ora 1, Ora 2, Ora 3 |
| MinuteHhMmAm | `33` | Esempi sono 8:00, 8:01, 8:02. Richiede che l'unità di tempo sia TimescaleMinutes. |
| MinuteMm | `34` | Esempi sono 0, 1, 2, ..., 59 minuti |
| MinuteFromEndMinuteMm | `37` | Esempi sono Minuto 181, Minuto 180, ..., Minuto 1, Minuto -1 dalla fine del progetto. |
| MinuteFromEndMm | `81` | Esempi sono 181, 180, ..., 1, -1 |
| MinuteFromEndMmm | `80` | Esempi sono M181, M180, ..., M1, M-1 |
| MinuteFromStartMinuteMm | `36` | Esempi sono Minuto -2, Minuto -1, Minuto 1, ... Minuto 180 dall'inizio del progetto. |
| MinuteFromStartMm | `83` | Esempi sono -2, -1, 1, ..., 180 |
| MinuteFromStartMmm | `82` | Esempi sono M-2, M-1, M1, ..., M180 |
| MonthM | `11` | Esempi sono M, A, M, J, J. Richiede che l'unità di tempo sia TimescaleMonths. |
| MonthMm | `57` | Esempi sono 11, 12, 1, 2 |
| MonthMmYy | `86` | Esempi sono 3/10, 4/10, 5/10 |
| MonthMmYyy | `85` | Esempi sono 3 '10, 4 '10, 5 '10 |
| MonthMmm | `10` | Esempi sono marzo, aprile, maggio |
| MonthMmmYyy | `8` | Esempi sono mar '10, apr '10, maggio '10 |
| MonthMmmm | `9` | Esempi sono marzo, aprile, maggio |
| MonthMmmmYyyy | `7` | Esempi sono marzo 2010, aprile 2010, maggio 2010 |
| MonthFromEndMm | `59` | Esempi sono 2, 1, -1, -2 mesi dalla fine del progetto. |
| MonthFromEndMmm | `58` | Esempi sono M2, M1, M-1, M-2 |
| MonthFromEndMonthMm | `45` | Esempi sono Mese 2, Mese 1, Mese -1, Mese -2 |
| MonthFromStartMm | `61` | Esempi sono -2, -2, 1, 2 mesi dall'inizio del progetto. |
| MonthFromStartMmm | `60` | Esempi sono M-2, M-1, M1, M2 |
| MonthFromStartMonthMm | `44` | Esempi sono Mese -2, Mese -1, Mese 1, Mese 2 |
| QuarterQ | `62` | Gli esempi sono 3, 4, 1. Richiede che l'unità di tempo sia TimescaleQuarts. |
| QuarterQq | `6` | Esempi sono Q3, Q4, Q1 |
| QuarterQqYyy | `4` | Esempi sono Q3 '10, Q4 '10, Q1 '11 |
| QuarterQqqQuarter | `2` | Esempi sono 3° trimestre, 1° trimestre |
| QuarterQQyy | `51` | Esempi sono 3Q10, 4Q10, 1Q11 |
| QuarterQtrQ | `5` | Esempi sono Qtr3, Qtr4, Qtr1 |
| QuarterQtrQYyyy | `3` | Esempi sono Qtr3, 2010; quarto trimestre, 2010; Qtr1, 2011 |
| QuarterFromEndQ | `64` | Esempi sono 5, 4, 3, 2, 1, -1 quarti dalla fine del progetto. |
| QuarterFromEndQq | `63` | Esempi sono Q5, Q4, Q3, Q2, Q1, Q-1 |
| QuarterFromEndQuarterQ | `47` | Esempi sono Trimestre 5, Trimestre 4, Trimestre 3, Trimestre 2, Trimestre 1, Trimestre -1 |
| QuarterFromStartQ | `66` | Esempi sono -5, -4, -3, -2, -1, 1 quarti dall'inizio del progetto. |
| QuarterFromStartQq | `65` | Esempi sono Q-5, Q-4, Q-3, Q-2, Q-1, Q1 |
| QuarterFromStartQuarterQ | `46` | Esempi sono Trimestre -5, Trimestre -4, Trimestre -3, Trimestre -2, Trimestre -1, Trimestre 1 |
| ThirdsOfMonthsDd | `136` | Esempi sono 1, 11, 21, 1. Richiede che l'unità di tempo sia TimescaleThirdsOfMonths. |
| ThirdsOfMonthsDdd | `137` | Esempi sono B, M, E, B |
| ThirdsOfMonthsDddd | `138` | Esempi sono Inizio, Mezzo, Fine, Inizio |
| ThirdsOfMonthsMmDd | `139` | L'esempio è 3/1. |
| ThirdsOfMonthsMmDdYy | `145` | L'esempio è 3/1/10. |
| ThirdsOfMonthsMmDdd | `140` | Esempi sono 3/B, 3/M, 3/E, 4/B |
| ThirdsOfMonthsMmDddYy | `146` | L'esempio è 3/B/10. |
| ThirdsOfMonthsMmmDd | `142` | Esempi sono 1 marzo, 11 marzo, 21 marzo, 1 aprile |
| ThirdsOfMonthsMmmDdYy | `147` | Esempi sono mar 1, '10; 11 marzo '10; 21 marzo '10; 1 aprile 10 |
| ThirdsOfMonthsMmmDdd | `143` | Esempi sono Mar B, Mar M, Mar E, Apr B |
| ThirdsOfMonthsMmmDddYy | `148` | Esempi sono Mar B, '10; Mar M, '10; marzo E, '10; Apr B '10 |
| ThirdsOfMonthsMmmmDd | `144` | Esempi sono 1 marzo, 11 marzo, 21 marzo, 1 aprile |
| ThirdsOfMonthsMmmmDdYyyy | `149` | Esempi sono 1 marzo 2010; 11 marzo 2010; 21 marzo 2010; 1 aprile 2010 |
| ThirdsOfMonthsMmmmDddd | `141` | Esempi sono inizio marzo, metà marzo, fine marzo, inizio aprile |
| ThirdsOfMonthsMmmmDdddYyyy | `150` | Esempi sono inizio marzo 2010; metà marzo, 2010; Fine marzo 2010; Inizio aprile 2010 |
| WeekDddDd | `88` | Esempi sono Sun 21, Sun 28, Sun 4. Richiede che l'unità di tempo sia TimescaleWeeks. |
| WeekDddMDd | `97` | Esempi sono Sun M 21, Sun M 28, Sun A 4 |
| WeekDddMmDd | `90` | Esempi sono Sun 21/3, Sun 28/3, Sun 4/4 |
| WeekDddMmDdYy | `100` | Esempi sono Sun 21/3/10, Sun 28/3/10, Sun 4/4/10 |
| WeekDddMmmDd | `93` | Esempi sono dom 21 marzo, dom 28 marzo, dom 4 aprile |
| WeekDddMmmDdYyy | `101` | Esempi sono Sun Mar 21, '10; dom 28 marzo '10; dom 4 aprile '10 |
| WeekDddMmmmDd | `96` | Esempi sono dom 21 marzo, dom 28 marzo, dom 4 aprile |
| WeekDddMmmmDdYyy | `102` | Esempi sono Sun March 21, '10; dom 28 marzo '10; 4 aprile '10 |
| WeekDddWw | `103` | Esempi sono Sun 12, Sun 13, Sun 14 |
| WeekDdiMDd | `98` | Esempi sono Su M 21, Su M 28, Su A 4 |
| WeekDdiMmDd | `91` | Esempi sono Do 21/3. Dom 28/3, Dom 4/4_x000g_ |
| WeekDdiMmmDd | `94` | Esempi sono dom 21 marzo, dom 28 marzo, dom 4 aprile |
| WeekDiMDd | `99` | Esempi sono SM 21, SM 28, SA 4 |
| WeekDiMmDd | `92` | Esempi sono S 3/21, S 3/28, S 4/4 |
| WeekDiMmmDd | `95` | Esempi sono S Mar 21, S Mar 28, S Apr 4 |
| WeekMDd | `89` | Esempi sono M21, M28, A 4 |
| WeekMmDd | `17` | Esempi sono 3/21, 3/28, 4/4 |
| WeekMmDdYy | `16` | L'esempio è '3/21/10'. |
| WeekMmmDd | `15` | Esempi sono 21 marzo, 28 marzo, 4 aprile |
| WeekMmmDdYyy | `13` | Esempi sono Mar 21, '10; 28 marzo '10; 4 aprile '10 |
| WeekMmmmDd | `14` | Esempi sono 21 marzo, 28 marzo, 4 aprile |
| WeekMmmmDdYyyy | `12` | Esempi sono 21 marzo 2010; 28 marzo 2010; 4 aprile 2010 |
| WeekDayOfMonthDd | `87` | Esempi sono 21, 28, 4 |
| WeekFromEndWeekWw | `43` | Esempi sono la settimana 2, la settimana 1, la settimana -1 dalla fine del progetto. |
| WeekFromEndWw | `68` | Esempi sono 2, 1, -1 |
| WeekFromEndWww | `67` | Esempi sono W2, W1, W-1 |
| WeekFromStartWeekWw | `42` | Esempi sono la settimana -1, la settimana 1, la settimana 2 dall'inizio del progetto. |
| WeekFromStartWw | `70` | Esempi sono -1, 1, 2 |
| WeekFromStartWww | `69` | Esempi sono W-1, W1, W2 |
| WeekNumberDdWw | `104` | Esempi sono 1 12, 1 13, 1 14 (giorno 1 della settimana 12, giorno 1 della settimana 13 e così via) |
| WeekNumberWw | `50` | Esempi sono 12, 13, 14 |
| YearYy | `75` | Gli esempi sono 10, 11, 12. Richiede che l'unità di tempo sia TimescaleYears. |
| YearYyy | `1` | Esempi sono '10, '11, '12 |
| YearYyyy | `0` | Esempi sono 2010, 2011, 2012 |
| YearFromEndYearYy | `49` | Esempi sono Anno 2, Anno 1, Anno -1 dalla fine del progetto. |
| YearFromEndYy | `72` | Esempi sono 2, 1, -1 |
| YearFromEndYyy | `71` | Esempi sono Y2, Y1, Y-1 |
| YearFromStartYearYy | `48` | Esempi sono Anno -1, Anno 1, Anno 2 dall'inizio del progetto. |
| YearFromStartYy | `74` | Esempi sono -1, 1, 2 |
| YearFromStartYyy | `73` | Esempi sono Y-1, Y1, Y2 |

### Guarda anche

* spazio dei nomi [Aspose.Tasks.Visualization](../../aspose.tasks.visualization)
* assemblea [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
