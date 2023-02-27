---
title: Enum DateLabel
second_title: Referencia de Aspose.Tasks para la API de .NET
description: Aspose.Tasks.Visualization.DateLabel enumeración. Especifica el formato de visualización de las etiquetas de fecha y hora en una escala de tiempo.
type: docs
weight: 2650
url: /es/net/aspose.tasks.visualization/datelabel/
---
## DateLabel enumeration

Especifica el formato de visualización de las etiquetas de fecha y hora en una escala de tiempo.

```csharp
public enum DateLabel
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `35` | No se muestra ninguna fecha. |
| DayDdd | `19` | Los ejemplos son lun, mar. |
| DayDddDd | `105` | Los ejemplos son lun 30, mar 1 |
| DayDddMDd | `112` | Los ejemplos son Lun S 30, Mar O 1 |
| DayDddMmDd | `108` | Los ejemplos son lun 9/30, mar 10/1 |
| DayDddMmDdYy | `52` | Los ejemplos son lunes 30/9/02, martes 1/10/02 |
| DayDddMmmDd | `23` | Los ejemplos son el lunes 30 de septiembre, el martes 1 de octubre |
| DayDddMmmDdYyy | `22` | Los ejemplos son el lunes 30 de septiembre de 2002, el martes 1 de octubre de 2002 |
| DayDddMmmmDd | `111` | Los ejemplos son lunes 30 de septiembre, martes 1 de octubre |
| DayDddd | `18` | Los ejemplos son martes, miércoles. |
| DayDdi | `119` | Los ejemplos son Mo, Tu |
| DayDdiDd | `106` | Los ejemplos son Mo 30, Tu 1 |
| DayDdiMDd | `113` | Los ejemplos son Mo S 30, Tu O 1 |
| DayDdiMmDd | `109` | Ejemplos: Lun 9/30, Mar 10/1 |
| DayDi | `20` | Los ejemplos son M, T |
| DayDiDdSpace | `107` | Los ejemplos son M 30, T 1 |
| DayDiMDd | `114` | Los ejemplos son MS 30, TO 1 |
| DayDiMmDd | `110` | Los ejemplos son M 9/30, T 10/1 |
| DayDiDdNoSpace | `121` | Los ejemplos son M30, T1 |
| DayMDd | `115` | Los ejemplos son S 30, O 1 |
| DayMmDd | `27` | Los ejemplos son 9/30, 10/1 |
| DayMmDdYy | `26` | Los ejemplos son 30/9/02, 1/10/02 |
| DayMmmDd | `25` | Los ejemplos son 30 de septiembre, 1 de octubre |
| DayMmmDdYyy | `24` | Los ejemplos son 30 de septiembre de 2002, 10 de octubre de 2002 |
| DayFromEndDayDd | `41` | Los ejemplos son Día 2, Día 1, Día -1, Día -2 desde el final del proyecto. |
| DayFromEndDd | `54` | Los ejemplos son 2, 1, -1, -2 |
| DayFromEndDdd | `53` | Los ejemplos son D2, D1, D-1, D-2 |
| DayFromStartDayDd | `40` | Los ejemplos son Día -2, Día -1, Día 1, Día 2 desde el inicio del proyecto. |
| DayFromStartDd | `56` | Los ejemplos son -2, -1, 1, 2 |
| DayFromStartDdd | `55` | Los ejemplos son D-2, D-1, D1, D2 |
| DayOfMonthDd | `21` | Los ejemplos son 30, 1 |
| DayOfYearDd | `118` | Los ejemplos son 77, 78 |
| DayOfYearDdYyy | `116` | Los ejemplos son 77 '10, 78 '10 |
| DayOfYearDdYyyy | `117` | Los ejemplos son 77 2010, 78 2010 |
| DayDdMmYyyy | `256` | El ejemplo es 19/07/2016. |
| HalfYearH | `128` | Los ejemplos son 1, 2. Requiere que la unidad de tiempo sea TimescaleHalfYears. |
| HalfYearHh | `127` | Los ejemplos son H1, H2 |
| HalfYearHhYyy | `126` | Los ejemplos son H1 '10, H2 '10 |
| HalfYearHhhHalf | `123` | Los ejemplos son 1st Half, 2d Half |
| HalfYearHHyy | `129` | Los ejemplos son 1H10, 2H10 |
| HalfYearHlfH | `125` | Los ejemplos son Mitad 1, Mitad 2 |
| HalfYearHlfHYyyy | `124` | Los ejemplos son Half 1, 2010; Mitad 2, 2010 |
| HalfYearFromEndH | `135` | Los ejemplos son 2, 1, -1, -2. Medio años desde la fecha de finalización del proyecto. |
| HalfYearFromEndHalfH | `133` | Los ejemplos son Mitad 2, Mitad 1, Mitad -1, Mitad -2 |
| HalfYearFromEndHh | `134` | Los ejemplos son H2, H1, H-1, H-2 |
| HalfYearFromStartH | `132` | Los ejemplos son -2, -1, 1, 2. Medio año desde la fecha de inicio del proyecto. |
| HalfYearFromStartHalfH | `130` | Los ejemplos son Mitad -2, Mitad -1, Mitad 1, Mitad 2 |
| HalfYearFromStartHh | `131` | Los ejemplos son H-2, H-1, H1, H2 |
| HourDddMmmDdHhAm | `28` | Los ejemplos son miércoles 18 de marzo, 8 a. m.; miércoles 18 de marzo, 9 a.m. Requiere que la unidad de tiempo sea TimescaleHours. |
| HourHh | `32` | Los ejemplos son 8, 9, 10, 11 |
| HourHhMmAm | `30` | Los ejemplos son 8:00 AM, 9:00 AM |
| HourHhAm | `31` | Ejemplos son 8AM, 9AM |
| HourMmDdHhAm | `120` | Los ejemplos son 3/18 8 AM, 3/18 9 AM |
| HourMmmDdHhAm | `29` | Los ejemplos son 18 de marzo, 8 a. m.; 18 de marzo, 9 a.m. |
| HourFromEndHh | `77` | Los ejemplos son 3, 2, 1, -1, -2 horas desde el final del proyecto. |
| HourFromEndHhh | `76` | Los ejemplos son H3, H2, H1, H-1, H-2 |
| HourFromEndHourHh | `39` | Los ejemplos son Hora 3, Hora 2, Hora 1, Hora -1, Hora -2 |
| HourFromStartHh | `79` | Los ejemplos son -2, -1, 1, 2, 3 horas desde el inicio del proyecto. |
| HourFromStartHhh | `78` | Los ejemplos son H-2, H-1, H1, H2, H3 |
| HourFromStartHourHh | `38` | Los ejemplos son Hora -2, Hora -1, Hora 1, Hora 2, Hora 3 |
| MinuteHhMmAm | `33` | Los ejemplos son 8:00 a. m., 8:01 a. m., 8:02 a. m. Requiere que la unidad de tiempo sea TimescaleMinutes. |
| MinuteMm | `34` | Los ejemplos son 0, 1, 2, ..., 59 minutos |
| MinuteFromEndMinuteMm | `37` | Ejemplos son Minuto 181, Minuto 180, ..., Minuto 1, Minuto -1 desde el final del proyecto. |
| MinuteFromEndMm | `81` | Los ejemplos son 181, 180, ..., 1, -1 |
| MinuteFromEndMmm | `80` | Los ejemplos son M181, M180, ..., M1, M-1 |
| MinuteFromStartMinuteMm | `36` | Ejemplos son Minuto -2, Minuto -1, Minuto 1, ... Minuto 180 desde el inicio del proyecto. |
| MinuteFromStartMm | `83` | Los ejemplos son -2, -1, 1, ..., 180 |
| MinuteFromStartMmm | `82` | Los ejemplos son M-2, M-1, M1, ..., M180 |
| MonthM | `11` | Los ejemplos son M, A, M, J, J. Requiere que la unidad de tiempo sea TimescaleMonths. |
| MonthMm | `57` | Los ejemplos son 11, 12, 1, 2 |
| MonthMmYy | `86` | Los ejemplos son 3/10, 4/10, 5/10 |
| MonthMmYyy | `85` | Los ejemplos son 3 '10, 4 '10, 5 '10 |
| MonthMmm | `10` | Los ejemplos son marzo, abril, mayo |
| MonthMmmYyy | `8` | Los ejemplos son Mar '10, Abr '10, May '10 |
| MonthMmmm | `9` | Los ejemplos son marzo, abril, mayo |
| MonthMmmmYyyy | `7` | Los ejemplos son marzo de 2010, abril de 2010, mayo de 2010 |
| MonthFromEndMm | `59` | Los ejemplos son 2, 1, -1, -2 meses desde el final del proyecto. |
| MonthFromEndMmm | `58` | Los ejemplos son M2, M1, M-1, M-2 |
| MonthFromEndMonthMm | `45` | Los ejemplos son Mes 2, Mes 1, Mes -1, Mes -2 |
| MonthFromStartMm | `61` | Los ejemplos son -2, -2, 1, 2 meses desde el inicio del proyecto. |
| MonthFromStartMmm | `60` | Los ejemplos son M-2, M-1, M1, M2 |
| MonthFromStartMonthMm | `44` | Los ejemplos son Mes -2, Mes -1, Mes 1, Mes 2 |
| QuarterQ | `62` | Los ejemplos son 3, 4, 1. Requiere que la unidad de tiempo sea TimescaleQuarters. |
| QuarterQq | `6` | Los ejemplos son Q3, Q4, Q1 |
| QuarterQqYyy | `4` | Los ejemplos son Q3 '10, Q4 '10, Q1 '11 |
| QuarterQqqQuarter | `2` | Los ejemplos son 3er trimestre, 1er trimestre |
| QuarterQQyy | `51` | Los ejemplos son 3T10, 4T10, 1T11 |
| QuarterQtrQ | `5` | Los ejemplos son Qtr3, Qtr4, Qtr1 |
| QuarterQtrQYyyy | `3` | Los ejemplos son Qtr3, 2010; Qtr4, 2010; Qtr1, 2011 |
| QuarterFromEndQ | `64` | Los ejemplos son 5, 4, 3, 2, 1, -1 trimestres desde el final del proyecto. |
| QuarterFromEndQq | `63` | Los ejemplos son Q5, Q4, Q3, Q2, Q1, Q-1 |
| QuarterFromEndQuarterQ | `47` | Los ejemplos son Trimestre 5, Trimestre 4, Trimestre 3, Trimestre 2, Trimestre 1, Trimestre -1 |
| QuarterFromStartQ | `66` | Los ejemplos son -5, -4, -3, -2, -1, 1 trimestre desde el inicio del proyecto. |
| QuarterFromStartQq | `65` | Los ejemplos son Q-5, Q-4, Q-3, Q-2, Q-1, Q1 |
| QuarterFromStartQuarterQ | `46` | Los ejemplos son Trimestre -5, Trimestre -4, Trimestre -3, Trimestre -2, Trimestre -1, Trimestre 1 |
| ThirdsOfMonthsDd | `136` | Los ejemplos son 1, 11, 21, 1. Requiere que la unidad de tiempo sea TimescaleThirdsOfMonths. |
| ThirdsOfMonthsDdd | `137` | Los ejemplos son B, M, E, B |
| ThirdsOfMonthsDddd | `138` | Los ejemplos son Principio, Medio, Fin, Principio |
| ThirdsOfMonthsMmDd | `139` | El ejemplo es 3/1. |
| ThirdsOfMonthsMmDdYy | `145` | El ejemplo es 3/1/10. |
| ThirdsOfMonthsMmDdd | `140` | Los ejemplos son 3/B, 3/M, 3/E, 4/B |
| ThirdsOfMonthsMmDddYy | `146` | El ejemplo es 3/B/10. |
| ThirdsOfMonthsMmmDd | `142` | Los ejemplos son 1 de marzo, 11 de marzo, 21 de marzo, 1 de abril |
| ThirdsOfMonthsMmmDdYy | `147` | Los ejemplos son 1 de marzo de 2010; 11 de marzo de 2010; 21 de marzo de 2010; 1 de abril de 10 |
| ThirdsOfMonthsMmmDdd | `143` | Los ejemplos son Mar B, Mar M, Mar E, Abr B |
| ThirdsOfMonthsMmmDddYy | `148` | Los ejemplos son Mar B, '10; marzo M, '10; Mar E, '10; Abril B '10 |
| ThirdsOfMonthsMmmmDd | `144` | Los ejemplos son 1 de marzo, 11 de marzo, 21 de marzo, 1 de abril |
| ThirdsOfMonthsMmmmDdYyyy | `149` | Los ejemplos son el 1 de marzo de 2010; 11 de marzo de 2010; 21 de marzo de 2010; 1 de abril de 2010 |
| ThirdsOfMonthsMmmmDddd | `141` | Los ejemplos son Principio de marzo, Medio de marzo, Fin de marzo, Principio de abril |
| ThirdsOfMonthsMmmmDdddYyyy | `150` | Los ejemplos son principios de marzo de 2010; Mediados de marzo de 2010; fines de marzo de 2010; Principios de abril, 2010 |
| WeekDddDd | `88` | Los ejemplos son Sun 21, Sun 28, Sun 4. Requiere que la unidad de tiempo sea TimescaleWeeks. |
| WeekDddMDd | `97` | Los ejemplos son Sun M 21, Sun M 28, Sun A 4 |
| WeekDddMmDd | `90` | Los ejemplos son dom 3/21, dom 3/28, dom 4/4 |
| WeekDddMmDdYy | `100` | Los ejemplos son dom 21/3/10, dom 28/3/10, dom 4/4/10 |
| WeekDddMmmDd | `93` | Los ejemplos son dom 21 de marzo, dom 28 de marzo, dom 4 de abril |
| WeekDddMmmDdYyy | `101` | Los ejemplos son dom 21 de marzo de '10; dom. 28 mar. '10; dom 4 abr, '10 |
| WeekDddMmmmDd | `96` | Los ejemplos son dom 21 de marzo, dom 28 de marzo, dom 4 de abril |
| WeekDddMmmmDdYyy | `102` | Los ejemplos son dom 21 de marzo de '10; dom 28 marzo '10; dom 4 de abril de '10 |
| WeekDddWw | `103` | Los ejemplos son dom 12, dom 13, dom 14 |
| WeekDdiMDd | `98` | Los ejemplos son Su M 21, Su M 28, Su A 4 |
| WeekDdiMmDd | `91` | Los ejemplos son Dom 3/21. Dom 3/28, Dom 4/4 |
| WeekDdiMmmDd | `94` | Los ejemplos son el domingo 21 de marzo, el domingo 28 de marzo, el domingo 4 de abril |
| WeekDiMDd | `99` | Los ejemplos son SM 21, SM 28, SA 4 |
| WeekDiMmDd | `92` | Los ejemplos son S 3/21, S 3/28, S 4/4 |
| WeekDiMmmDd | `95` | Los ejemplos son S 21 de marzo, S 28 de marzo, S 4 de abril |
| WeekMDd | `89` | Los ejemplos son M21, M28, A 4 |
| WeekMmDd | `17` | Los ejemplos son 3/21, 3/28, 4/4 |
| WeekMmDdYy | `16` | El ejemplo es '21/3/10'. |
| WeekMmmDd | `15` | Los ejemplos son 21 de marzo, 28 de marzo, 4 de abril |
| WeekMmmDdYyy | `13` | Los ejemplos son 21 de marzo de 2010; 28 de marzo de 2010; 4 abr. '10 |
| WeekMmmmDd | `14` | Los ejemplos son 21 de marzo, 28 de marzo, 4 de abril |
| WeekMmmmDdYyyy | `12` | Los ejemplos son el 21 de marzo de 2010; 28 de marzo de 2010; 4 de abril de 2010 |
| WeekDayOfMonthDd | `87` | Los ejemplos son 21, 28, 4 |
| WeekFromEndWeekWw | `43` | Los ejemplos son Semana 2, Semana 1, Semana -1 desde el final del proyecto. |
| WeekFromEndWw | `68` | Los ejemplos son 2, 1, -1 |
| WeekFromEndWww | `67` | Los ejemplos son W2, W1, W-1 |
| WeekFromStartWeekWw | `42` | Los ejemplos son Semana -1, Semana 1, Semana 2 desde el inicio del proyecto. |
| WeekFromStartWw | `70` | Los ejemplos son -1, 1, 2 |
| WeekFromStartWww | `69` | Los ejemplos son W-1, W1, W2 |
| WeekNumberDdWw | `104` | Los ejemplos son 1 12, 1 13, 1 14 (día 1 de la semana 12, día 1 de la semana 13, etc.) |
| WeekNumberWw | `50` | Los ejemplos son 12, 13, 14 |
| YearYy | `75` | Los ejemplos son 10, 11, 12. Requiere que la unidad de tiempo sea TimescaleYears. |
| YearYyy | `1` | Los ejemplos son '10, '11, '12 |
| YearYyyy | `0` | Los ejemplos son 2010, 2011, 2012 |
| YearFromEndYearYy | `49` | Los ejemplos son Año 2, Año 1, Año -1 desde el final del proyecto. |
| YearFromEndYy | `72` | Los ejemplos son 2, 1, -1 |
| YearFromEndYyy | `71` | Los ejemplos son Y2, Y1, Y-1 |
| YearFromStartYearYy | `48` | Los ejemplos son Año -1, Año 1, Año 2 desde el inicio del proyecto. |
| YearFromStartYy | `74` | Los ejemplos son -1, 1, 2 |
| YearFromStartYyy | `73` | Los ejemplos son Y-1, Y1, Y2 |

### Ver también

* espacio de nombres [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* asamblea [Aspose.Tasks](../../)


