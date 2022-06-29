---
title: DateLabel
second_title: Справочник по Aspose.Tasks для .NET API
description: Задает формат отображения меток даты и времени на шкале времени.
type: docs
weight: 2620
url: /ru/net/aspose.tasks.visualization/datelabel/
---
## DateLabel enumeration

Задает формат отображения меток даты и времени на шкале времени.

```csharp
public enum DateLabel
```

### Ценности

| Имя | Ценность | Описание |
| --- | --- | --- |
| None | `35` | Дата не отображается. |
| DayDdd | `19` | Примеры Пн, Вт. |
| DayDddDd | `105` | Примеры:Пн 30, Вт 1 |
| DayDddMDd | `112` | Примеры:Пн С 30, Вт О 1 |
| DayDddMmDd | `108` | Примеры:Пн 30.09, Вт 1.10 |
| DayDddMmDdYy | `52` | Примеры:Пн 30.09.02, Вт 01.10.02 |
| DayDddMmmDd | `23` | Примеры:понедельник 30 сентября, вторник 1 октября |
| DayDddMmmDdYyy | `22` | Примеры:понедельник, 30 сентября 2002 г., вторник, 1 октября 2002 г. |
| DayDddMmmmDd | `111` | Примеры:понедельник 30 сентября, вторник 1 октября |
| DayDddd | `18` | Примеры:вторник, среда. |
| DayDdi | `119` | Примеры Пн, Вт |
| DayDdiDd | `106` | Примеры:Пн 30, Вт 1 |
| DayDdiMDd | `113` | Примеры:Mo S 30, Tu O 1 |
| DayDdiMmDd | `109` | Примеры:Пн 9/30, Вт 10/1 |
| DayDi | `20` | Примеры:M, T |
| DayDiDdSpace | `107` | Примеры:M 30, T 1 |
| DayDiMDd | `114` | Примеры MS 30, TO 1 |
| DayDiMmDd | `110` | Примеры:M 9/30, T 10/1 |
| DayDiDdNoSpace | `121` | Примеры:M30, T1 |
| DayMDd | `115` | Примеры:S 30, O 1 |
| DayMmDd | `27` | Примеры:9/30, 10/1 |
| DayMmDdYy | `26` | Примеры:30.09.02, 01.10.02 |
| DayMmmDd | `25` | Примеры:30 сентября, 1 октября |
| DayMmmDdYyy | `24` | Примеры:30 сентября 2002 г., 10 октября 2002 г. |
| DayFromEndDayDd | `41` | Примеры:День 2, День 1, День -1, День -2 с конца проекта. |
| DayFromEndDd | `54` | Примеры:2, 1, -1, -2 |
| DayFromEndDdd | `53` | Примеры:D2, D1, D-1, D-2 |
| DayFromStartDayDd | `40` | Примеры:День -2, День -1, День 1, День 2 с начала проекта. |
| DayFromStartDd | `56` | Примеры:-2, -1, 1, 2 |
| DayFromStartDdd | `55` | Примеры:D-2, D-1, D1, D2 |
| DayOfMonthDd | `21` | Примеры:30, 1 |
| DayOfYearDd | `118` | Примеры:77, 78 |
| DayOfYearDdYyy | `116` | Примеры:77 '10, 78 '10 |
| DayOfYearDdYyyy | `117` | Примеры:77 2010, 78 2010 |
| DayDdMmYyyy | `256` | Пример:19/07/2016. |
| HalfYearH | `128` | Примеры:1, 2. Требует, чтобы единицей времени было TimescaleHalfYears. |
| HalfYearHh | `127` | Примеры H1, H2 |
| HalfYearHhYyy | `126` | Примеры:H1 '10, H2 '10 |
| HalfYearHhhHalf | `123` | Примеры:1-я половина, 2-я половина |
| HalfYearHHyy | `129` | Примеры:1H10, 2H10 |
| HalfYearHlfH | `125` | Примеры:Half 1, Half 2 |
| HalfYearHlfHYyyy | `124` | Примеры:Half 1, 2010; Половина 2, 2010 |
| HalfYearFromEndH | `135` | Примеры:2, 1, -1, -2. Полтора года с даты окончания проекта. |
| HalfYearFromEndHalfH | `133` | Примеры:Half 2, Half 1, Half -1, Half -2 |
| HalfYearFromEndHh | `134` | Примеры:H2, H1, H-1, H-2 |
| HalfYearFromStartH | `132` | Примеры:-2, -1, 1, 2. Полтора года с даты начала проекта. |
| HalfYearFromStartHalfH | `130` | Примеры:Half-2, Half-1, Half 1, Half 2 |
| HalfYearFromStartHh | `131` | Примеры:H-2, H-1, H1, H2 |
| HourDddMmmDdHhAm | `28` | Примеры:среда, 18 марта, 8:00; Ср, 18 марта, 9:00. Требует, чтобы единицей времени было TimescaleHours. |
| HourHh | `32` | Примеры:8, 9, 10, 11 |
| HourHhMmAm | `30` | Примеры:8:00, 9:00 |
| HourHhAm | `31` | Примеры:8:00, 9:00 |
| HourMmDdHhAm | `120` | Примеры:3/18 8:00, 3/18 9:00 |
| HourMmmDdHhAm | `29` | Примеры:18 марта, 8:00; 18 марта, 9:00 |
| HourFromEndHh | `77` | Примеры:3, 2, 1, -1, -2 часа с конца проекта. |
| HourFromEndHhh | `76` | Примеры:H3, H2, H1, H-1, H-2 |
| HourFromEndHourHh | `39` | Примеры:Час 3, Час 2, Час 1, Час -1, Час -2 |
| HourFromStartHh | `79` | Примеры -2, -1, 1, 2, 3 часа от начала проекта. |
| HourFromStartHhh | `78` | Примеры:H-2, H-1, H1, H2, H3 |
| HourFromStartHourHh | `38` | Примеры:Час -2, Час -1, Час 1, Час 2, Час 3 |
| MinuteHhMmAm | `33` | Примеры:8:00, 8:01, 8:02. Требует, чтобы единицей времени было TimescaleMinutes. |
| MinuteMm | `34` | Примеры:0, 1, 2, ..., 59 минут |
| MinuteFromEndMinuteMm | `37` | Примеры:Минута 181, Минута 180, ..., Минута 1, Минута -1 от конца проекта. |
| MinuteFromEndMm | `81` | Примеры:181, 180, ..., 1, -1 |
| MinuteFromEndMmm | `80` | Примеры:M181, M180, ..., M1, M-1 |
| MinuteFromStartMinuteMm | `36` | Примеры:Минута -2, Минута -1, Минута 1, ... Минута 180 от начала проекта. |
| MinuteFromStartMm | `83` | Примеры -2, -1, 1, ..., 180 |
| MinuteFromStartMmm | `82` | Примеры:M-2, M-1, M1, ..., M180 |
| MonthM | `11` | Примеры:M, A, M, J, J. Требуется, чтобы единицей времени было TimescaleMonths. |
| MonthMm | `57` | Примеры:11, 12, 1, 2 |
| MonthMmYy | `86` | Примеры:3/10, 4/10, 5/10 |
| MonthMmYyy | `85` | Примеры:3 '10, 4 '10, 5 '10 |
| MonthMmm | `10` | Примеры:март, апрель, май |
| MonthMmmYyy | `8` | Примеры:март '10, апр '10, май '10 |
| MonthMmmm | `9` | Примеры:март, апрель, май |
| MonthMmmmYyyy | `7` | Примеры:март 2010 г., апрель 2010 г., май 2010 г. |
| MonthFromEndMm | `59` | Примеры:2, 1, -1, -2 месяца после окончания проекта. |
| MonthFromEndMmm | `58` | Примеры:M2, M1, M-1, M-2 |
| MonthFromEndMonthMm | `45` | Примеры:Месяц 2, Месяц 1, Месяц -1, Месяц -2 |
| MonthFromStartMm | `61` | Примеры -2, -2, 1, 2 месяца с начала проекта. |
| MonthFromStartMmm | `60` | Примеры:M-2, M-1, M1, M2 |
| MonthFromStartMonthMm | `44` | Примеры:Месяц -2, Месяц -1, Месяц 1, Месяц 2 |
| QuarterQ | `62` | Примеры:3, 4, 1. Требуется, чтобы единицей времени было TimescaleQuarters. |
| QuarterQq | `6` | Примеры:Q3, Q4, Q1 |
| QuarterQqYyy | `4` | Примеры:Q3 '10, Q4 '10, Q1 '11 |
| QuarterQqqQuarter | `2` | Примеры:3-я четверть, 1-я четверть |
| QuarterQQyy | `51` | Примеры:3Q10, 4Q10, 1Q11 |
| QuarterQtrQ | `5` | Примеры Qtr3, Qtr4, Qtr1 |
| QuarterQtrQYyyy | `3` | Примеры:Qtr3, 2010; 4 квартал 2010 г.; Qtr1, 2011 |
| QuarterFromEndQ | `64` | Примеры:5, 4, 3, 2, 1, -1 квартал от конца проекта. |
| QuarterFromEndQq | `63` | Примеры:Q5, Q4, Q3, Q2, Q1, Q-1 |
| QuarterFromEndQuarterQ | `47` | Примеры:квартал 5, квартал 4, квартал 3, квартал 2, квартал 1, квартал -1 |
| QuarterFromStartQ | `66` | Примеры:-5, -4, -3, -2, -1, 1 квартал от начала проекта. |
| QuarterFromStartQq | `65` | Примеры:Q-5, Q-4, Q-3, Q-2, Q-1, Q1 |
| QuarterFromStartQuarterQ | `46` | Примеры:Квартал -5, Квартал -4, Квартал -3, Квартал -2, Квартал -1, Квартал 1 |
| ThirdsOfMonthsDd | `136` | Примеры:1, 11, 21, 1. Требуется, чтобы единицей времени было TimescaleThirdsOfMonths. |
| ThirdsOfMonthsDdd | `137` | Примеры:B, M, E, B |
| ThirdsOfMonthsDddd | `138` | Примеры:Начало, Середина, Конец, Начало |
| ThirdsOfMonthsMmDd | `139` | Пример:3/1. |
| ThirdsOfMonthsMmDdYy | `145` | Пример:01.03.10. |
| ThirdsOfMonthsMmDdd | `140` | Примеры:3/B, 3/M, 3/E, 4/B |
| ThirdsOfMonthsMmDddYy | `146` | Пример:3/B/10. |
| ThirdsOfMonthsMmmDd | `142` | Примеры:1 марта, 11 марта, 21 марта, 1 апреля |
| ThirdsOfMonthsMmmDdYy | `147` | Примеры:1 марта 2010 г.; 11 марта 2010 г .; 21 марта 2010 г .; 1, 10 апр |
| ThirdsOfMonthsMmmDdd | `143` | Примеры:март B, март M, март E, апр B |
| ThirdsOfMonthsMmmDddYy | `148` | Примеры:Mar B, '10; март М., 2010 г.; март 2010 г.; Апр B '10 |
| ThirdsOfMonthsMmmmDd | `144` | Примеры:1 марта, 11 марта, 21 марта, 1 апреля |
| ThirdsOfMonthsMmmmDdYyyy | `149` | Примеры:1 марта 2010 г.; 11 марта 2010 г.; 21 марта 2010 г.; 1 апреля 2010 г. |
| ThirdsOfMonthsMmmmDddd | `141` | Примеры:начало марта, середина марта, конец марта, начало апреля |
| ThirdsOfMonthsMmmmDdddYyyy | `150` | Примеры:начало марта 2010 г.; середина марта 2010 г.; Конец марта 2010 г .; Апрель Начало, 2010 |
| WeekDddDd | `88` | Примеры:Воскресенье 21, Воскресенье 28, Воскресенье 4. Требуется, чтобы единицей времени было TimescaleWeeks. |
| WeekDddMDd | `97` | Примеры:Солнце M 21, Солнце M 28, Солнце A 4 |
| WeekDddMmDd | `90` | Примеры:вс 3/21, вс 3/28, вс 4/4 |
| WeekDddMmDdYy | `100` | Примеры:вс 21.03.10, вс 28.03.10, вс 4/4/10 |
| WeekDddMmmDd | `93` | Примеры:вс 21 марта, вс 28 марта, вс 4 апр |
| WeekDddMmmDdYyy | `101` | Примеры:Sun 21 Mar '10; Вс, 28 марта 2010 г.; Вс 4 апр. '10 |
| WeekDddMmmmDd | `96` | Примеры:вс 21 марта, вс 28 марта, вс 4 апр |
| WeekDddMmmmDdYyy | `102` | Примеры:воскресенье, 21 марта 2010 г.; Вс, 28 марта 2010 г.; Вс, 4 апреля 2010 г. |
| WeekDddWw | `103` | Примеры:вс 12, вс 13, вс 14 |
| WeekDdiMDd | `98` | Примеры Su M 21, Su M 28, Su A 4 |
| WeekDdiMmDd | `91` | Примеры Su 3/21. Вс 28.03, Вс 4/4 |
| WeekDdiMmmDd | `94` | Примеры:вс 21 марта, вс 28 марта, вс 4 апр |
| WeekDiMDd | `99` | Примеры:SM 21, SM 28, SA 4 |
| WeekDiMmDd | `92` | Примеры:S 3/21, S 3/28, S 4/4 |
| WeekDiMmmDd | `95` | Примеры:С 21 марта, С 28 марта, С 4 апреля |
| WeekMDd | `89` | Примеры:M21, M28, A 4 |
| WeekMmDd | `17` | Примеры:3/21, 3/28, 4/4 |
| WeekMmDdYy | `16` | Пример:"21.03.10". |
| WeekMmmDd | `15` | Примеры:21 марта, 28 марта, 4 апреля |
| WeekMmmDdYyy | `13` | Примеры:21 марта 2010 г.; 28 марта 2010 г .; 4 апр. 2010 г. |
| WeekMmmmDd | `14` | Примеры:21 марта, 28 марта, 4 апреля |
| WeekMmmmDdYyyy | `12` | Примеры:21 марта 2010 г.; 28 марта 2010 г.; 4 апреля 2010 г. |
| WeekDayOfMonthDd | `87` | Примеры:21, 28, 4 |
| WeekFromEndWeekWw | `43` | Примеры:Неделя 2, Неделя 1, Неделя -1 с конца проекта. |
| WeekFromEndWw | `68` | Примеры:2, 1, -1 |
| WeekFromEndWww | `67` | Примеры:W2, W1, W-1 |
| WeekFromStartWeekWw | `42` | Примеры:неделя -1, неделя 1, неделя 2 с начала проекта. |
| WeekFromStartWw | `70` | Примеры -1, 1, 2 |
| WeekFromStartWww | `69` | Примеры:W-1, W1, W2 |
| WeekNumberDdWw | `104` | Примеры:1 12, 1 13, 1 14 (день 1 недели 12, день 1 недели 13 и т. д.) |
| WeekNumberWw | `50` | Примеры:12, 13, 14 |
| YearYy | `75` | Примеры:10, 11, 12. Требуется, чтобы единицей времени было TimescaleYears. |
| YearYyy | `1` | Примеры:'10, '11, '12 |
| YearYyyy | `0` | Примеры:2010, 2011, 2012 |
| YearFromEndYearYy | `49` | Примеры:Год 2, Год 1, Год -1 с конца проекта. |
| YearFromEndYy | `72` | Примеры:2, 1, -1 |
| YearFromEndYyy | `71` | Примеры:Y2, Y1, Y-1 |
| YearFromStartYearYy | `48` | Примеры:Год -1, Год 1, Год 2 с начала проекта. |
| YearFromStartYy | `74` | Примеры -1, 1, 2 |
| YearFromStartYyy | `73` | Примеры:Y-1, Y1, Y2 |

### Смотрите также

* пространство имен [Aspose.Tasks.Visualization](../../aspose.tasks.visualization)
* сборка [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
