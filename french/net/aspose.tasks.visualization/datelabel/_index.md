---
title: "Enum DateLabel"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Visualization.DateLabel enum. Spécifie le format d'affichage des libellés de date et d'heure dans une échelle de temps"
type: docs
weight: 2980
url: /fr/net/aspose.tasks.visualization/datelabel/
---
## DateLabel enumeration

Spécifie le format d'affichage des étiquettes de date et d'heure dans une échelle de temps.

```csharp
public enum DateLabel
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `35` | Aucune date n'est affichée. |
| DayDdd | `19` | Les exemples sont lun., mar. |
| DayDddDd | `105` | Les exemples sont lun 30, mar 1 |
| DayDddMDd | `112` | Les exemples sont lun S 30, mar O 1 |
| DayDddMmDd | `108` | Les exemples sont lun 9/30, mar 10/1 |
| DayDddMmDdYy | `52` | Les exemples sont lun 9/30/02, mar 10/1/02 |
| DayDddMmmDd | `23` | Les exemples sont lun sept. 30, mar oct. 1 |
| DayDddMmmDdYyy | `22` | Les exemples sont lun sept. 30 '02, mar oct. 1 '02 |
| DayDddMmmmDd | `111` | Les exemples sont lun septembre 30, mar octobre 1 |
| DayDddd | `18` | Les exemples sont mardi, mercredi. |
| DayDdi | `119` | Les exemples sont lu, ma |
| DayDdiDd | `106` | Les exemples sont lu 30, ma 1 |
| DayDdiMDd | `113` | Les exemples sont lu S 30, ma O 1 |
| DayDdiMmDd | `109` | Les exemples sont lu 9/30, ma 10/1 |
| DayDi | `20` | Les exemples sont L, M |
| DayDiDdSpace | `107` | Les exemples sont L 30, M 1 |
| DayDiMDd | `114` | Les exemples sont L S 30, M O 1 |
| DayDiMmDd | `110` | Les exemples sont L 9/30, M 10/1 |
| DayDiDdNoSpace | `121` | Les exemples sont L30, M1 |
| DayMDd | `115` | Les exemples sont S 30, O 1 |
| DayMmDd | `27` | Les exemples sont 9/30, 10/1 |
| DayMmDdYy | `26` | Les exemples sont 9/30/02, 10/1/02 |
| DayMmmDd | `25` | Les exemples sont sept. 30, oct. 1 |
| DayMmmDdYyy | `24` | Les exemples sont sept. 30 '02, oct. 10 '02 |
| DayFromEndDayDd | `41` | Les exemples sont Jour 2, Jour 1, Jour -1, Jour -2 à partir de la fin du projet. |
| DayFromEndDd | `54` | Les exemples sont 2, 1, -1, -2 |
| DayFromEndDdd | `53` | Les exemples sont D2, D1, D-1, D-2 |
| DayFromStartDayDd | `40` | Les exemples sont Jour -2, Jour -1, Jour 1, Jour 2 à partir du début du projet. |
| DayFromStartDd | `56` | Les exemples sont -2, -1, 1, 2 |
| DayFromStartDdd | `55` | Les exemples sont D-2, D-1, D1, D2 |
| DayOfMonthDd | `21` | Les exemples sont 30, 1 |
| DayOfYearDd | `118` | Les exemples sont 77, 78 |
| DayOfYearDdYyy | `116` | Les exemples sont 77 '10, 78 '10 |
| DayOfYearDdYyyy | `117` | Les exemples sont 77 2010, 78 2010 |
| DayDdMmYyyy | `256` | L'exemple est le 19/07/2016. |
| HalfYearH | `128` | Les exemples sont 1, 2. Nécessite que l'unité de temps soit TimescaleHalfYears. |
| HalfYearHh | `127` | Les exemples sont H1, H2 |
| HalfYearHhYyy | `126` | Les exemples sont H1 '10, H2 '10 |
| HalfYearHhhHalf | `123` | Les exemples sont 1re moitié, 2e moitié |
| HalfYearHHyy | `129` | Les exemples sont 1H10, 2H10 |
| HalfYearHlfH | `125` | Les exemples sont Moitié 1, Moitié 2 |
| HalfYearHlfHYyyy | `124` | Les exemples sont Moitié 1, 2010 ; Moitié 2, 2010 |
| HalfYearFromEndH | `135` | Les exemples sont 2, 1, -1, -2. Semestres à partir de la date de fin du projet. |
| HalfYearFromEndHalfH | `133` | Les exemples sont Moitié 2, Moitié 1, Moitié -1, Moitié -2 |
| HalfYearFromEndHh | `134` | Les exemples sont H2, H1, H-1, H-2 |
| HalfYearFromStartH | `132` | Les exemples sont -2, -1, 1, 2. Semestres à partir de la date de début du projet. |
| HalfYearFromStartHalfH | `130` | Les exemples sont Moitié -2, Moitié -1, Moitié 1, Moitié 2 |
| HalfYearFromStartHh | `131` | Les exemples sont H-2, H-1, H1, H2 |
| HourDddMmmDdHhAm | `28` | Les exemples sont Wed Mar 18, 8 AM; Wed Mar 18, 9 AM. Nécessite que l'unité de temps soit TimescaleHours. |
| HourHh | `32` | Les exemples sont 8, 9, 10, 11 |
| HourHhMmAm | `30` | Les exemples sont 8:00 AM, 9:00 AM |
| HourHhAm | `31` | Les exemples sont 8AM, 9AM |
| HourMmDdHhAm | `120` | Les exemples sont 3/18 8 AM, 3/18 9 AM |
| HourMmmDdHhAm | `29` | Les exemples sont Mar 18, 8 AM; Mar 18, 9 AM |
| HourFromEndHh | `77` | Les exemples sont 3, 2, 1, -1, -2 heures depuis la fin du projet. |
| HourFromEndHhh | `76` | Les exemples sont H3, H2, H1, H-1, H-2 |
| HourFromEndHourHh | `39` | Les exemples sont Hour 3, Hour 2, Hour 1, Hour -1, Hour -2 |
| HourFromStartHh | `79` | Les exemples sont -2, -1, 1, 2, 3 heures depuis le début du projet. |
| HourFromStartHhh | `78` | Les exemples sont H-2, H-1, H1, H2, H3 |
| HourFromStartHourHh | `38` | Les exemples sont Hour -2, Hour -1, Hour 1, Hour 2, Hour 3 |
| MinuteHhMmAm | `33` | Les exemples sont 8:00 AM, 8:01 AM, 8:02 AM. Nécessite que l'unité de temps soit TimescaleMinutes. |
| MinuteMm | `34` | Les exemples sont 0, 1, 2, ..., 59 minutes |
| MinuteFromEndMinuteMm | `37` | Les exemples sont Minute 181, Minute 180, ..., Minute 1, Minute -1 depuis la fin du projet. |
| MinuteFromEndMm | `81` | Les exemples sont 181, 180, ..., 1, -1 |
| MinuteFromEndMmm | `80` | Les exemples sont M181, M180, ..., M1, M-1 |
| MinuteFromStartMinuteMm | `36` | Les exemples sont Minute -2, Minute -1, Minute 1, ... Minute 180 depuis le début du projet. |
| MinuteFromStartMm | `83` | Les exemples sont -2, -1, 1, ..., 180 |
| MinuteFromStartMmm | `82` | Les exemples sont M-2, M-1, M1, ..., M180 |
| MonthM | `11` | Les exemples sont M, A, M, J, J. Nécessite que l'unité de temps soit TimescaleMonths. |
| MonthMm | `57` | Les exemples sont 11, 12, 1, 2 |
| MonthMmYy | `86` | Les exemples sont 3/10, 4/10, 5/10 |
| MonthMmYyy | `85` | Les exemples sont 3 '10, 4 '10, 5 '10 |
| MonthMmm | `10` | Les exemples sont Mar, Apr, May |
| MonthMmmYyy | `8` | Les exemples sont Mar '10, Apr '10, May '10 |
| MonthMmmm | `9` | Les exemples sont mars, avril, mai |
| MonthMmmmYyyy | `7` | Les exemples sont mars 2010, avril 2010, mai 2010 |
| MonthFromEndMm | `59` | Les exemples sont 2, 1, -1, -2 mois à partir de la fin du projet. |
| MonthFromEndMmm | `58` | Les exemples sont M2, M1, M-1, M-2 |
| MonthFromEndMonthMm | `45` | Les exemples sont Mois 2, Mois 1, Mois -1, Mois -2 |
| MonthFromStartMm | `61` | Les exemples sont -2, -2, 1, 2 mois à partir du début du projet. |
| MonthFromStartMmm | `60` | Les exemples sont M-2, M-1, M1, M2 |
| MonthFromStartMonthMm | `44` | Les exemples sont Mois -2, Mois -1, Mois 1, Mois 2 |
| QuarterQ | `62` | Les exemples sont 3, 4, 1. Nécessite que l'unité de temps soit TimescaleQuarters. |
| QuarterQq | `6` | Les exemples sont Q3, Q4, Q1 |
| QuarterQqYyy | `4` | Les exemples sont Q3 '10, Q4 '10, Q1 '11 |
| QuarterQqqQuarter | `2` | Les exemples sont 3e trimestre, 1er trimestre |
| QuarterQQyy | `51` | Les exemples sont 3Q10, 4Q10, 1Q11 |
| QuarterQtrQ | `5` | Les exemples sont Qtr3, Qtr4, Qtr1 |
| QuarterQtrQYyyy | `3` | Les exemples sont Qtr3, 2010; Qtr4, 2010; Qtr1, 2011 |
| QuarterFromEndQ | `64` | Les exemples sont 5, 4, 3, 2, 1, -1 trimestres à partir de la fin du projet. |
| QuarterFromEndQq | `63` | Les exemples sont Q5, Q4, Q3, Q2, Q1, Q-1 |
| QuarterFromEndQuarterQ | `47` | Les exemples sont Trimestre 5, Trimestre 4, Trimestre 3, Trimestre 2, Trimestre 1, Trimestre -1 |
| QuarterFromStartQ | `66` | Les exemples sont -5, -4, -3, -2, -1, 1 trimestres à partir du début du projet. |
| QuarterFromStartQq | `65` | Les exemples sont Q-5, Q-4, Q-3, Q-2, Q-1, Q1 |
| QuarterFromStartQuarterQ | `46` | Les exemples sont Trimestre -5, Trimestre -4, Trimestre -3, Trimestre -2, Trimestre -1, Trimestre 1 |
| ThirdsOfMonthsDd | `136` | Les exemples sont 1, 11, 21, 1. Nécessite que l'unité de temps soit TimescaleThirdsOfMonths. |
| ThirdsOfMonthsDdd | `137` | Les exemples sont B, M, E, B |
| ThirdsOfMonthsDddd | `138` | Les exemples sont Début, Milieu, Fin, Début |
| ThirdsOfMonthsMmDd | `139` | L'exemple est 3/1. |
| ThirdsOfMonthsMmDdYy | `145` | L'exemple est 3/1/10. |
| ThirdsOfMonthsMmDdd | `140` | Les exemples sont 3/B, 3/M, 3/E, 4/B |
| ThirdsOfMonthsMmDddYy | `146` | L'exemple est 3/B/10. |
| ThirdsOfMonthsMmmDd | `142` | Les exemples sont 1 mars, 11 mars, 21 mars, 1 avr |
| ThirdsOfMonthsMmmDdYy | `147` | Les exemples sont 1 mars, '10; 11 mars, '10; 21 mars, '10; 1 avr, 10 |
| ThirdsOfMonthsMmmDdd | `143` | Les exemples sont mars B, mars M, mars E, avr B |
| ThirdsOfMonthsMmmDddYy | `148` | Les exemples sont mars B, '10; mars M, '10; mars E, '10; avr B '10 |
| ThirdsOfMonthsMmmmDd | `144` | Les exemples sont 1 mars, 11 mars, 21 mars, 1 avril |
| ThirdsOfMonthsMmmmDdYyyy | `149` | Les exemples sont 1 mars 2010; 11 mars 2010; 21 mars 2010; 1 avril 2010 |
| ThirdsOfMonthsMmmmDddd | `141` | Les exemples sont mars Début, mars Milieu, mars Fin, avril Début |
| ThirdsOfMonthsMmmmDdddYyyy | `150` | Les exemples sont mars Début, 2010; mars Milieu, 2010; mars Fin, 2010; avril Début, 2010 |
| WeekDddDd | `88` | Les exemples sont dim 21, dim 28, dim 4. L'unité de temps doit être TimescaleWeeks. |
| WeekDddMDd | `97` | Les exemples sont dim M 21, dim M 28, dim A 4 |
| WeekDddMmDd | `90` | Les exemples sont dim 3/21, dim 3/28, dim 4/4 |
| WeekDddMmDdYy | `100` | Les exemples sont dim 3/21/10, dim 3/28/10, dim 4/4/10 |
| WeekDddMmmDd | `93` | Les exemples sont dim 21 mars, dim 28 mars, dim 4 avr |
| WeekDddMmmDdYyy | `101` | Les exemples sont dim 21 mars, '10; dim 28 mars, '10; dim 4 avr, '10 |
| WeekDddMmmmDd | `96` | Les exemples sont dim 21 mars, dim 28 mars, dim 4 avr |
| WeekDddMmmmDdYyy | `102` | Les exemples sont dim 21 mars, '10; dim 28 mars, '10; dim 4 avr, '10 |
| WeekDddWw | `103` | Les exemples sont dim 12, dim 13, dim 14 |
| WeekDdiMDd | `98` | Les exemples sont dim M 21, dim M 28, dim A 4 |
| WeekDdiMmDd | `91` | Les exemples sont dim 3/21. dim 3/28, dim 4/4 |
| WeekDdiMmmDd | `94` | Les exemples sont dim 21 mars, dim 28 mars, dim 4 avr |
| WeekDiMDd | `99` | Les exemples sont S M 21, S M 28, S A 4 |
| WeekDiMmDd | `92` | Les exemples sont S 3/21, S 3/28, S 4/4 |
| WeekDiMmmDd | `95` | Les exemples sont S Mar 21, S Mar 28, S Apr 4 |
| WeekMDd | `89` | Les exemples sont M21, M28, A 4 |
| WeekMmDd | `17` | Les exemples sont 3/21, 3/28, 4/4 |
| WeekMmDdYy | `16` | L'exemple est '3/21/10'. |
| WeekMmmDd | `15` | Les exemples sont Mar 21, Mar 28, Apr 4 |
| WeekMmmDdYyy | `13` | Les exemples sont Mar 21, '10; Mar 28, '10; Apr 4, '10 |
| WeekMmmmDd | `14` | Les exemples sont mars 21, mars 28, avril 4 |
| WeekMmmmDdYyyy | `12` | Les exemples sont mars 21, 2010; mars 28, 2010; avril 4, 2010 |
| WeekDayOfMonthDd | `87` | Les exemples sont 21, 28, 4 |
| WeekFromEndWeekWw | `43` | Les exemples sont Semaine 2, Semaine 1, Semaine -1 à partir de la fin du projet. |
| WeekFromEndWw | `68` | Les exemples sont 2, 1, -1 |
| WeekFromEndWww | `67` | Les exemples sont W2, W1, W-1 |
| WeekFromStartWeekWw | `42` | Les exemples sont Semaine -1, Semaine 1, Semaine 2 à partir du début du projet. |
| WeekFromStartWw | `70` | Les exemples sont -1, 1, 2 |
| WeekFromStartWww | `69` | Les exemples sont W-1, W1, W2 |
| WeekNumberDdWw | `104` | Les exemples sont 1 12, 1 13, 1 14 (jour 1 de la semaine 12, jour 1 de la semaine 13, et ainsi de suite) |
| WeekNumberWw | `50` | Les exemples sont 12, 13, 14 |
| YearYy | `75` | Les exemples sont 10, 11, 12. Nécessite que l'unité de temps soit TimescaleYears. |
| YearYyy | `1` | Les exemples sont '10, '11, '12 |
| YearYyyy | `0` | Les exemples sont 2010, 2011, 2012 |
| YearFromEndYearYy | `49` | Les exemples sont Année 2, Année 1, Année -1 à partir de la fin du projet. |
| YearFromEndYy | `72` | Les exemples sont 2, 1, -1 |
| YearFromEndYyy | `71` | Les exemples sont Y2, Y1, Y-1 |
| YearFromStartYearYy | `48` | Les exemples sont Année -1, Année 1, Année 2 à partir du début du projet. |
| YearFromStartYy | `74` | Les exemples sont -1, 1, 2 |
| YearFromStartYyy | `73` | Les exemples sont Y-1, Y1, Y2 |

## Exemples

Ajouter des liens de tâche

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");

// ajuster les niveaux de l'échelle de temps
project.TaskLinks.Add(project.RootTask.Children.Add("Task 1"), project.RootTask.Children.Add("Task 2"));

var view = (GanttChartView)project.DefaultView;

// ajuster le niveau supérieur

// définir le niveau supérieur de l'échelle de temps de la vue du diagramme de Gantt.
// définir l'unité d'échelle de temps <see cref=\"T:Aspose.Tasks.Visualization.TimescaleUnit\" /> pour le niveau de l'échelle de temps.
view.MiddleTimescaleTier = new TimescaleTier();
// définir l'intervalle d'unité de temps dans lequel afficher les libellés pour le niveau.
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
// définir le libellé de date <see cref=\"T:Aspose.Tasks.Visualization.DateLabel\" /> pour le niveau de l'échelle de temps.
view.MiddleTimescaleTier.Count = 1;
// définir comment aligner les libellés à l'intérieur de chaque période de temps du niveau (<see cref=\"T:System.Drawing.StringAlignment\" />).
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
// définir comment aligner les étiquettes dans chaque période de temps du niveau (<see cref="T:System.Drawing.StringAlignment" />).
view.MiddleTimescaleTier.Alignment = HorizontalStringAlignment.Center;
// définir une valeur indiquant s'il faut afficher les marques de repère qui séparent les périodes de temps dans le niveau.
view.MiddleTimescaleTier.ShowTicks = true;
// définir une valeur indiquant s'il faut baser les libellés du niveau sur l'exercice fiscal.
view.MiddleTimescaleTier.UsesFiscalYear = true;

// ajouté pour une meilleure visualisation
view.TopTimescaleTier = new TimescaleTier(TimescaleUnit.Months, 1);

// personnaliser les dates du niveau intermédiaire
view.TopTimescaleTier.DateTimeConverter = date =>
    new[] { "Янв.", "Фев.", "Мар.", "Апр.", "Май", "Июнь", "Июль", "Авг.", "Сен.", "Окт.", "Ноя.", "Дек." }[date.Month - 1];

project.Set(Prj.TimescaleStart, new DateTime(2012, 7, 30));
project.Set(Prj.TimescaleFinish, new DateTime(2012, 10, 6));

// Utilisez l'option 'Timescale.DefinedInView' pour rendre les échelles de temps en utilisant les paramètres d'échelle de temps définis dans la vue (view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier).
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "CustomizeTimescaleTierLabels_out.pdf", pdfSaveOptions);
```

### Voir aussi

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


