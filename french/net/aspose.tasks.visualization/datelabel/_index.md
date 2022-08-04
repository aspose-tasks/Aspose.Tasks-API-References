---
title: DateLabel
second_title: Référence de l'API Aspose.Tasks pour .NET
description: Spécifie le format daffichage des étiquettes de date et dheure dans une échelle de temps.
type: docs
weight: 2630
url: /fr/net/aspose.tasks.visualization/datelabel/
---
## DateLabel enumeration

Spécifie le format d'affichage des étiquettes de date et d'heure dans une échelle de temps.

```csharp
public enum DateLabel
```

### Valeurs

| Nom | Évaluer | La description |
| --- | --- | --- |
| None | `35` | Aucune date n'est affichée. |
| DayDdd | `19` | Les exemples sont lundi, mar. |
| DayDddDd | `105` | Exemples : lundi 30, mardi 1 |
| DayDddMDd | `112` | Exemples : lundi S 30, mardi O 1 |
| DayDddMmDd | `108` | Les exemples sont le lundi 30/09, le mardi 1/10 |
| DayDddMmDdYy | `52` | Les exemples sont lun 30/09/02, mar 01/10/02 |
| DayDddMmmDd | `23` | Les exemples sont le lundi 30 septembre, le mardi 1er octobre |
| DayDddMmmDdYyy | `22` | Exemples : lundi 30 septembre 2002, mardi 1er octobre 2002 |
| DayDddMmmmDd | `111` | Les exemples sont le lundi 30 septembre, le mardi 1er octobre |
| DayDddd | `18` | Les exemples sont mardi, mercredi. |
| DayDdi | `119` | Les exemples sont Mo, Tu |
| DayDdiDd | `106` | Les exemples sont Mo 30, Tu 1 |
| DayDdiMDd | `113` | Les exemples sont Mo S 30, Tu O 1 |
| DayDdiMmDd | `109` | Les exemples sont Lu 9/30, Tu 10/1 |
| DayDi | `20` | Les exemples sont M, T |
| DayDiDdSpace | `107` | Les exemples sont M 30, T 1 |
| DayDiMDd | `114` | Les exemples sont MS 30, TO 1 |
| DayDiMmDd | `110` | Les exemples sont M 9/30, T 10/1 |
| DayDiDdNoSpace | `121` | Les exemples sont M30, T1 |
| DayMDd | `115` | Les exemples sont S 30, O 1 |
| DayMmDd | `27` | Les exemples sont 9/30, 10/1 |
| DayMmDdYy | `26` | Les exemples sont 9/30/02, 10/1/02 |
| DayMmmDd | `25` | Les exemples sont le 30 septembre, le 1er octobre |
| DayMmmDdYyy | `24` | Exemples : 30 septembre 2002, 10 octobre 2002 |
| DayFromEndDayDd | `41` | Les exemples sont Jour 2, Jour 1, Jour -1, Jour -2 à partir de la fin du projet. |
| DayFromEndDd | `54` | Les exemples sont 2, 1, -1, -2 |
| DayFromEndDdd | `53` | Les exemples sont D2, D1, D-1, D-2 |
| DayFromStartDayDd | `40` | Les exemples sont Jour -2, Jour -1, Jour 1, Jour 2 depuis le début du projet. |
| DayFromStartDd | `56` | Les exemples sont -2, -1, 1, 2 |
| DayFromStartDdd | `55` | Les exemples sont D-2, D-1, D1, D2 |
| DayOfMonthDd | `21` | Les exemples sont 30, 1 |
| DayOfYearDd | `118` | Les exemples sont 77, 78 |
| DayOfYearDdYyy | `116` | Les exemples sont 77 '10, 78 '10 |
| DayOfYearDdYyyy | `117` | Les exemples sont 77 2010, 78 2010 |
| DayDdMmYyyy | `256` | Exemple : 19/07/2016. |
| HalfYearH | `128` | Les exemples sont 1, 2. Nécessite que l'unité de temps soit TimescaleHalfYears. |
| HalfYearHh | `127` | Les exemples sont H1, H2 |
| HalfYearHhYyy | `126` | Les exemples sont H1 '10, H2 '10 |
| HalfYearHhhHalf | `123` | Exemples : 1ère mi-temps, 2e mi-temps |
| HalfYearHHyy | `129` | Les exemples sont 1H10, 2H10 |
| HalfYearHlfH | `125` | Les exemples sont Moitié 1, Moitié 2 |
| HalfYearHlfHYyyy | `124` | Les exemples sont Half 1, 2010 ; Demi 2, 2010 |
| HalfYearFromEndH | `135` | Les exemples sont 2, 1, -1, -2. Six mois à compter de la date de fin du projet. |
| HalfYearFromEndHalfH | `133` | Les exemples sont Moitié 2, Moitié 1, Moitié -1, Moitié -2 |
| HalfYearFromEndHh | `134` | Les exemples sont H2, H1, H-1, H-2 |
| HalfYearFromStartH | `132` | Les exemples sont -2, -1, 1, 2. Six mois à compter de la date de début du projet. |
| HalfYearFromStartHalfH | `130` | Les exemples sont Moitié -2, Moitié -1, Moitié 1, Moitié 2 |
| HalfYearFromStartHh | `131` | Les exemples sont H-2, H-1, H1, H2 |
| HourDddMmmDdHhAm | `28` | Exemples : mercredi 18 mars, 8 h ; Mer 18 mars, 9 h. Nécessite que l'unité de temps soit TimescaleHours. |
| HourHh | `32` | Les exemples sont 8, 9, 10, 11 |
| HourHhMmAm | `30` | Exemples : 8h00, 9h00 |
| HourHhAm | `31` | Les exemples sont 8h00, 9h00 |
| HourMmDdHhAm | `120` | Les exemples sont 3/18 8 AM, 3/18 9 AM |
| HourMmmDdHhAm | `29` | Exemples : 18 mars, 8 h ; 18 mars, 9 h |
| HourFromEndHh | `77` | Les exemples sont 3, 2, 1, -1, -2 heures à partir de la fin du projet. |
| HourFromEndHhh | `76` | Les exemples sont H3, H2, H1, H-1, H-2 |
| HourFromEndHourHh | `39` | Les exemples sont Heure 3, Heure 2, Heure 1, Heure -1, Heure -2 |
| HourFromStartHh | `79` | Les exemples sont -2, -1, 1, 2, 3 heures à partir du début du projet. |
| HourFromStartHhh | `78` | Les exemples sont H-2, H-1, H1, H2, H3 |
| HourFromStartHourHh | `38` | Les exemples sont Heure -2, Heure -1, Heure 1, Heure 2, Heure 3 |
| MinuteHhMmAm | `33` | Les exemples sont 8h00, 8h01, 8h02. Nécessite que l'unité de temps soit TimescaleMinutes. |
| MinuteMm | `34` | Les exemples sont 0, 1, 2, ..., 59 minutes |
| MinuteFromEndMinuteMm | `37` | Exemples : Minute 181, Minute 180, ..., Minute 1, Minute -1 à partir de la fin du projet. |
| MinuteFromEndMm | `81` | Les exemples sont 181, 180, ..., 1, -1 |
| MinuteFromEndMmm | `80` | Les exemples sont M181, M180, ..., M1, M-1 |
| MinuteFromStartMinuteMm | `36` | Exemples : Minute -2, Minute -1, Minute 1, ... Minute 180 depuis le début du projet. |
| MinuteFromStartMm | `83` | Les exemples sont -2, -1, 1, ..., 180 |
| MinuteFromStartMmm | `82` | Les exemples sont M-2, M-1, M1, ..., M180 |
| MonthM | `11` | Les exemples sont M, A, M, J, J. Nécessite que l'unité de temps soit TimescaleMonths. |
| MonthMm | `57` | Les exemples sont 11, 12, 1, 2 |
| MonthMmYy | `86` | Les exemples sont 3/10, 4/10, 5/10 |
| MonthMmYyy | `85` | Les exemples sont 3 '10, 4 '10, 5 '10 |
| MonthMmm | `10` | Les exemples sont mars, avril, mai |
| MonthMmmYyy | `8` | Les exemples sont mars '10, avril '10, mai '10 |
| MonthMmmm | `9` | Les exemples sont mars, avril, mai |
| MonthMmmmYyyy | `7` | Les exemples sont mars 2010, avril 2010, mai 2010 |
| MonthFromEndMm | `59` | Les exemples sont 2, 1, -1, -2 mois à compter de la fin du projet. |
| MonthFromEndMmm | `58` | Les exemples sont M2, M1, M-1, M-2 |
| MonthFromEndMonthMm | `45` | Les exemples sont Mois 2, Mois 1, Mois -1, Mois -2 |
| MonthFromStartMm | `61` | Les exemples sont -2, -2, 1, 2 mois à partir du début du projet. |
| MonthFromStartMmm | `60` | Les exemples sont M-2, M-1, M1, M2 |
| MonthFromStartMonthMm | `44` | Les exemples sont Mois -2, Mois -1, Mois 1, Mois 2 |
| QuarterQ | `62` | Les exemples sont 3, 4, 1. Nécessite que l'unité de temps soit TimescaleQuarters. |
| QuarterQq | `6` | Les exemples sont Q3, Q4, Q1 |
| QuarterQqYyy | `4` | Les exemples sont Q3 '10, Q4 '10, Q1 '11 |
| QuarterQqqQuarter | `2` | Exemples : 3e trimestre, 1er trimestre |
| QuarterQQyy | `51` | Les exemples sont 3Q10, 4Q10, 1Q11 |
| QuarterQtrQ | `5` | Les exemples sont Qtr3, Qtr4, Qtr1 |
| QuarterQtrQYyyy | `3` | Les exemples sont Qtr3, 2010 ; 4e trimestre, 2010 ; Trim1, 2011 |
| QuarterFromEndQ | `64` | Les exemples sont 5, 4, 3, 2, 1, -1 trimestres à partir de la fin du projet. |
| QuarterFromEndQq | `63` | Les exemples sont Q5, Q4, Q3, Q2, Q1, Q-1 |
| QuarterFromEndQuarterQ | `47` | Exemples : Trimestre 5, Trimestre 4, Trimestre 3, Trimestre 2, Trimestre 1, Trimestre -1 |
| QuarterFromStartQ | `66` | Les exemples sont -5, -4, -3, -2, -1, 1 trimestres depuis le début du projet. |
| QuarterFromStartQq | `65` | Les exemples sont Q-5, Q-4, Q-3, Q-2, Q-1, Q1 |
| QuarterFromStartQuarterQ | `46` | Exemples : Trimestre -5, Trimestre -4, Trimestre -3, Trimestre -2, Trimestre -1, Trimestre 1 |
| ThirdsOfMonthsDd | `136` | Les exemples sont 1, 11, 21, 1. Nécessite que l'unité de temps soit TimescaleThirdsOfMonths. |
| ThirdsOfMonthsDdd | `137` | Les exemples sont B, M, E, B |
| ThirdsOfMonthsDddd | `138` | Les exemples sont Début, Milieu, Fin, Début |
| ThirdsOfMonthsMmDd | `139` | L'exemple est 3/1. |
| ThirdsOfMonthsMmDdYy | `145` | L'exemple est 3/1/10. |
| ThirdsOfMonthsMmDdd | `140` | Les exemples sont 3/B, 3/M, 3/E, 4/B |
| ThirdsOfMonthsMmDddYy | `146` | L'exemple est 3/B/10. |
| ThirdsOfMonthsMmmDd | `142` | Exemples : 1er mars, 11 mars, 21 mars, 1er avril |
| ThirdsOfMonthsMmmDdYy | `147` | Les exemples sont le 1er mars '10 ; 11 mars 2010 ; 21 mars 2010 ; 1 avril 10 |
| ThirdsOfMonthsMmmDdd | `143` | Les exemples sont Mar B, Mar M, Mar E, Avr B |
| ThirdsOfMonthsMmmDddYy | `148` | Les exemples sont Mar B, '10 ; Mars M, '10 ; Mars E, '10 ; Avr B '10 |
| ThirdsOfMonthsMmmmDd | `144` | Les exemples sont le 1er mars, le 11 mars, le 21 mars et le 1er avril |
| ThirdsOfMonthsMmmmDdYyyy | `149` | Les exemples sont le 1er mars 2010 ; 11 mars 2010 ; 21 mars 2010 ; 1 avril 2010 |
| ThirdsOfMonthsMmmmDddd | `141` | Les exemples sont Début mars, Milieu mars, Fin mars, Début avril |
| ThirdsOfMonthsMmmmDdddYyyy | `150` | Les exemples sont Début mars 2010 ; Mi-mars 2010 ; fin mars 2010 ; Début avril 2010 |
| WeekDddDd | `88` | Les exemples sont Sun 21, Sun 28, Sun 4. Nécessite que l'unité de temps soit TimescaleWeeks. |
| WeekDddMDd | `97` | Les exemples sont Sun M 21, Sun M 28, Sun A 4 |
| WeekDddMmDd | `90` | Les exemples sont dim 3/21, dim 3/28, dim 4/4 |
| WeekDddMmDdYy | `100` | Exemples : Dim 21/03/10, Dim 28/03/10, Dim 4/4/10 |
| WeekDddMmmDd | `93` | Exemples : dim 21 mars, dim 28 mars, dim 4 avril |
| WeekDddMmmDdYyy | `101` | Les exemples sont Sun Mar 21, '10; dim. 28 mars 2010 ; dim. 4 avril '10 |
| WeekDddMmmmDd | `96` | Exemples : dim 21 mars, dim 28 mars, dim 4 avril |
| WeekDddMmmmDdYyy | `102` | Les exemples sont le dimanche 21 mars '10 ; Dim 28 mars '10 ; Dim 4 avril '10 |
| WeekDddWw | `103` | Les exemples sont dim 12, dim 13, dim 14 |
| WeekDdiMDd | `98` | Les exemples sont Su M 21, Su M 28, Su A 4 |
| WeekDdiMmDd | `91` | Les exemples sont Su 3/21. Di 3/28, Di 4/4 |
| WeekDdiMmmDd | `94` | Exemples : Su 21 mars, Su 28 mars, Su 4 avril |
| WeekDiMDd | `99` | Les exemples sont SM 21, SM 28, SA 4 |
| WeekDiMmDd | `92` | Les exemples sont S 3/21, S 3/28, S 4/4 |
| WeekDiMmmDd | `95` | Exemples : S 21 mars, S 28 mars, S 4 avril |
| WeekMDd | `89` | Les exemples sont M21, M28, A 4 |
| WeekMmDd | `17` | Les exemples sont 3/21, 3/28, 4/4 |
| WeekMmDdYy | `16` | L'exemple est '3/21/10'. |
| WeekMmmDd | `15` | Exemples : 21 mars, 28 mars, 4 avril |
| WeekMmmDdYyy | `13` | Exemples : 21 mars 2010 ; 28 mars 2010 ; 4 avril '10 |
| WeekMmmmDd | `14` | Les exemples sont le 21 mars, le 28 mars, le 4 avril |
| WeekMmmmDdYyyy | `12` | Les exemples sont le 21 mars 2010 ; 28 mars 2010 ; 4 avril 2010 |
| WeekDayOfMonthDd | `87` | Les exemples sont 21, 28, 4 |
| WeekFromEndWeekWw | `43` | Les exemples sont Semaine 2, Semaine 1, Semaine -1 à partir de la fin du projet. |
| WeekFromEndWw | `68` | Les exemples sont 2, 1, -1 |
| WeekFromEndWww | `67` | Les exemples sont W2, W1, W-1 |
| WeekFromStartWeekWw | `42` | Les exemples sont Semaine -1, Semaine 1, Semaine 2 depuis le début du projet. |
| WeekFromStartWw | `70` | Les exemples sont -1, 1, 2 |
| WeekFromStartWww | `69` | Les exemples sont W-1, W1, W2 |
| WeekNumberDdWw | `104` | Les exemples sont 1 12, 1 13, 1 14 (jour 1 de la semaine 12, jour 1 de la semaine 13, etc.) |
| WeekNumberWw | `50` | Les exemples sont 12, 13, 14 |
| YearYy | `75` | Les exemples sont 10, 11, 12. Nécessite que l'unité de temps soit TimescaleYears. |
| YearYyy | `1` | Les exemples sont '10, '11, '12 |
| YearYyyy | `0` | Les exemples sont 2010, 2011, 2012 |
| YearFromEndYearYy | `49` | Les exemples sont l'année 2, l'année 1, l'année -1 à partir de la fin du projet. |
| YearFromEndYy | `72` | Les exemples sont 2, 1, -1 |
| YearFromEndYyy | `71` | Les exemples sont Y2, Y1, Y-1 |
| YearFromStartYearYy | `48` | Les exemples sont Année -1, Année 1, Année 2 depuis le début du projet. |
| YearFromStartYy | `74` | Les exemples sont -1, 1, 2 |
| YearFromStartYyy | `73` | Les exemples sont Y-1, Y1, Y2 |

### Voir également

* espace de noms [Aspose.Tasks.Visualization](../../aspose.tasks.visualization)
* Assemblée [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
