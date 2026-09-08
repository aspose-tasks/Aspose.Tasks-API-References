---
title: "Enum DateLabel"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Visualization.DateLabel enum. Specificeert het weergaveformaat voor datum- en tijdlabels in een tijdschaal"
type: docs
weight: 2980
url: /nl/net/aspose.tasks.visualization/datelabel/
---
## DateLabel enumeration

Specificeert het weergaveformaat voor datum- en tijdlabels in een tijdschaal.

```csharp
public enum DateLabel
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| None | `35` | Er wordt geen datum weergegeven. |
| DayDdd | `19` | Voorbeelden zijn ma, di. |
| DayDddDd | `105` | Voorbeelden zijn ma 30, di 1 |
| DayDddMDd | `112` | Voorbeelden zijn ma S 30, di O 1 |
| DayDddMmDd | `108` | Voorbeelden zijn ma 9/30, di 10/1 |
| DayDddMmDdYy | `52` | Voorbeelden zijn ma 9/30/02, di 10/1/02 |
| DayDddMmmDd | `23` | Voorbeelden zijn ma sep 30, di okt 1 |
| DayDddMmmDdYyy | `22` | Voorbeelden zijn ma sep 30 '02, di okt 1 '02 |
| DayDddMmmmDd | `111` | Voorbeelden zijn ma september 30, di oktober 1 |
| DayDddd | `18` | Voorbeelden zijn dinsdag, woensdag. |
| DayDdi | `119` | Voorbeelden zijn ma, di |
| DayDdiDd | `106` | Voorbeelden zijn ma 30, di 1 |
| DayDdiMDd | `113` | Voorbeelden zijn ma S 30, di O 1 |
| DayDdiMmDd | `109` | Voorbeelden zijn ma 9/30, di 10/1 |
| DayDi | `20` | Voorbeelden zijn M, D |
| DayDiDdSpace | `107` | Voorbeelden zijn M 30, D 1 |
| DayDiMDd | `114` | Voorbeelden zijn M S 30, D O 1 |
| DayDiMmDd | `110` | Voorbeelden zijn M 9/30, D 10/1 |
| DayDiDdNoSpace | `121` | Voorbeelden zijn M30, D1 |
| DayMDd | `115` | Voorbeelden zijn S 30, O 1 |
| DayMmDd | `27` | Voorbeelden zijn 9/30, 10/1 |
| DayMmDdYy | `26` | Voorbeelden zijn 9/30/02, 10/1/02 |
| DayMmmDd | `25` | Voorbeelden zijn sep 30, okt 1 |
| DayMmmDdYyy | `24` | Voorbeelden zijn sep 30 '02, okt 10 '02 |
| DayFromEndDayDd | `41` | Voorbeelden zijn Dag 2, Dag 1, Dag -1, Dag -2 van het project einde. |
| DayFromEndDd | `54` | Voorbeelden zijn 2, 1, -1, -2 |
| DayFromEndDdd | `53` | Voorbeelden zijn D2, D1, D-1, D-2 |
| DayFromStartDayDd | `40` | Voorbeelden zijn Dag -2, Dag -1, Dag 1, Dag 2 van het project start. |
| DayFromStartDd | `56` | Voorbeelden zijn -2, -1, 1, 2 |
| DayFromStartDdd | `55` | Voorbeelden zijn D-2, D-1, D1, D2 |
| DayOfMonthDd | `21` | Voorbeelden zijn 30, 1 |
| DayOfYearDd | `118` | Voorbeelden zijn 77, 78 |
| DayOfYearDdYyy | `116` | Voorbeelden zijn 77 '10, 78 '10 |
| DayOfYearDdYyyy | `117` | Voorbeelden zijn 77 2010, 78 2010 |
| DayDdMmYyyy | `256` | Voorbeeld is 19/07/2016. |
| HalfYearH | `128` | Voorbeelden zijn 1, 2. Vereist dat de tijdseenheid TimescaleHalfYears is. |
| HalfYearHh | `127` | Voorbeelden zijn H1, H2 |
| HalfYearHhYyy | `126` | Voorbeelden zijn H1 '10, H2 '10 |
| HalfYearHhhHalf | `123` | Voorbeelden zijn 1e Half, 2e Half |
| HalfYearHHyy | `129` | Voorbeelden zijn 1H10, 2H10 |
| HalfYearHlfH | `125` | Voorbeelden zijn Half 1, Half 2 |
| HalfYearHlfHYyyy | `124` | Voorbeelden zijn Half 1, 2010; Half 2, 2010 |
| HalfYearFromEndH | `135` | Voorbeelden zijn 2, 1, -1, -2. Halfjaren vanaf de project einddatum. |
| HalfYearFromEndHalfH | `133` | Voorbeelden zijn Half 2, Half 1, Half -1, Half -2 |
| HalfYearFromEndHh | `134` | Voorbeelden zijn H2, H1, H-1, H-2 |
| HalfYearFromStartH | `132` | Voorbeelden zijn -2, -1, 1, 2. Halfjaren vanaf de project startdatum. |
| HalfYearFromStartHalfH | `130` | Voorbeelden zijn Half -2, Half -1, Half 1, Half 2 |
| HalfYearFromStartHh | `131` | Voorbeelden zijn H-2, H-1, H1, H2 |
| HourDddMmmDdHhAm | `28` | Voorbeelden zijn Wed Mar 18, 8 AM; Wed Mar 18, 9 AM. Vereist dat de tijdseenheid TimescaleHours is. |
| HourHh | `32` | Voorbeelden zijn 8, 9, 10, 11 |
| HourHhMmAm | `30` | Voorbeelden zijn 8:00 AM, 9:00 AM |
| HourHhAm | `31` | Voorbeelden zijn 8AM, 9AM |
| HourMmDdHhAm | `120` | Voorbeelden zijn 3/18 8 AM, 3/18 9 AM |
| HourMmmDdHhAm | `29` | Voorbeelden zijn Mar 18, 8 AM; Mar 18, 9 AM |
| HourFromEndHh | `77` | Voorbeelden zijn 3, 2, 1, -1, -2 uur vanaf het projecteinde. |
| HourFromEndHhh | `76` | Voorbeelden zijn H3, H2, H1, H-1, H-2 |
| HourFromEndHourHh | `39` | Voorbeelden zijn Uur 3, Uur 2, Uur 1, Uur -1, Uur -2 |
| HourFromStartHh | `79` | Voorbeelden zijn -2, -1, 1, 2, 3 uur vanaf het projectbegin. |
| HourFromStartHhh | `78` | Voorbeelden zijn H-2, H-1, H1, H2, H3 |
| HourFromStartHourHh | `38` | Voorbeelden zijn Uur -2, Uur -1, Uur 1, Uur 2, Uur 3 |
| MinuteHhMmAm | `33` | Voorbeelden zijn 8:00 AM, 8:01 AM, 8:02 AM. Vereist dat de tijdseenheid TimescaleMinutes is. |
| MinuteMm | `34` | Voorbeelden zijn 0, 1, 2, ..., 59 minuten |
| MinuteFromEndMinuteMm | `37` | Voorbeelden zijn Minuut 181, Minuut 180, ..., Minuut 1, Minuut -1 vanaf het projecteinde. |
| MinuteFromEndMm | `81` | Voorbeelden zijn 181, 180, ..., 1, -1 |
| MinuteFromEndMmm | `80` | Voorbeelden zijn M181, M180, ..., M1, M-1 |
| MinuteFromStartMinuteMm | `36` | Voorbeelden zijn Minuut -2, Minuut -1, Minuut 1, ... Minuut 180 vanaf het projectbegin. |
| MinuteFromStartMm | `83` | Voorbeelden zijn -2, -1, 1, ..., 180 |
| MinuteFromStartMmm | `82` | Voorbeelden zijn M-2, M-1, M1, ..., M180 |
| MonthM | `11` | Voorbeelden zijn M, A, M, J, J. Vereist dat de tijdseenheid TimescaleMonths is. |
| MonthMm | `57` | Voorbeelden zijn 11, 12, 1, 2 |
| MonthMmYy | `86` | Voorbeelden zijn 3/10, 4/10, 5/10 |
| MonthMmYyy | `85` | Voorbeelden zijn 3 '10, 4 '10, 5 '10 |
| MonthMmm | `10` | Voorbeelden zijn mrt, apr, mei |
| MonthMmmYyy | `8` | Voorbeelden zijn mrt '10, apr '10, mei '10 |
| MonthMmmm | `9` | Voorbeelden zijn maart, april, mei |
| MonthMmmmYyyy | `7` | Voorbeelden zijn maart 2010, april 2010, mei 2010 |
| MonthFromEndMm | `59` | Voorbeelden zijn 2, 1, -1, -2 maanden vanaf het projecteinde. |
| MonthFromEndMmm | `58` | Voorbeelden zijn M2, M1, M-1, M-2 |
| MonthFromEndMonthMm | `45` | Voorbeelden zijn maand 2, maand 1, maand -1, maand -2 |
| MonthFromStartMm | `61` | Voorbeelden zijn -2, -2, 1, 2 maanden vanaf de projectstart. |
| MonthFromStartMmm | `60` | Voorbeelden zijn M-2, M-1, M1, M2 |
| MonthFromStartMonthMm | `44` | Voorbeelden zijn maand -2, maand -1, maand 1, maand 2 |
| QuarterQ | `62` | Voorbeelden zijn 3, 4, 1. Vereist dat de tijdseenheid TimescaleQuarters is. |
| QuarterQq | `6` | Voorbeelden zijn Q3, Q4, Q1 |
| QuarterQqYyy | `4` | Voorbeelden zijn Q3 '10, Q4 '10, Q1 '11 |
| QuarterQqqQuarter | `2` | Voorbeelden zijn 3e kwartaal, 1e kwartaal |
| QuarterQQyy | `51` | Voorbeelden zijn 3Q10, 4Q10, 1Q11 |
| QuarterQtrQ | `5` | Voorbeelden zijn Qtr3, Qtr4, Qtr1 |
| QuarterQtrQYyyy | `3` | Voorbeelden zijn Qtr3, 2010; Qtr4, 2010; Qtr1, 2011 |
| QuarterFromEndQ | `64` | Voorbeelden zijn 5, 4, 3, 2, 1, -1 kwartalen vanaf het projecteinde. |
| QuarterFromEndQq | `63` | Voorbeelden zijn Q5, Q4, Q3, Q2, Q1, Q-1 |
| QuarterFromEndQuarterQ | `47` | Voorbeelden zijn kwartaal 5, kwartaal 4, kwartaal 3, kwartaal 2, kwartaal 1, kwartaal -1 |
| QuarterFromStartQ | `66` | Voorbeelden zijn -5, -4, -3, -2, -1, 1 kwartalen vanaf de projectstart. |
| QuarterFromStartQq | `65` | Voorbeelden zijn Q-5, Q-4, Q-3, Q-2, Q-1, Q1 |
| QuarterFromStartQuarterQ | `46` | Voorbeelden zijn kwartaal -5, kwartaal -4, kwartaal -3, kwartaal -2, kwartaal -1, kwartaal 1 |
| ThirdsOfMonthsDd | `136` | Voorbeelden zijn 1, 11, 21, 1. Vereist dat de tijdseenheid TimescaleThirdsOfMonths is. |
| ThirdsOfMonthsDdd | `137` | Voorbeelden zijn B, M, E, B |
| ThirdsOfMonthsDddd | `138` | Voorbeelden zijn Begin, Midden, Einde, Begin |
| ThirdsOfMonthsMmDd | `139` | Voorbeeld is 3/1. |
| ThirdsOfMonthsMmDdYy | `145` | Voorbeeld is 3/1/10. |
| ThirdsOfMonthsMmDdd | `140` | Voorbeelden zijn 3/B, 3/M, 3/E, 4/B |
| ThirdsOfMonthsMmDddYy | `146` | Voorbeeld is 3/B/10. |
| ThirdsOfMonthsMmmDd | `142` | Voorbeelden zijn mrt 1, mrt 11, mrt 21, apr 1 |
| ThirdsOfMonthsMmmDdYy | `147` | Voorbeelden zijn mrt 1, '10; mrt 11, '10; mrt 21, '10; apr 1, 10 |
| ThirdsOfMonthsMmmDdd | `143` | Voorbeelden zijn mrt B, mrt M, mrt E, apr B |
| ThirdsOfMonthsMmmDddYy | `148` | Voorbeelden zijn mrt B, '10; mrt M, '10; mrt E, '10; apr B '10 |
| ThirdsOfMonthsMmmmDd | `144` | Voorbeelden zijn maart 1, maart 11, maart 21, april 1 |
| ThirdsOfMonthsMmmmDdYyyy | `149` | Voorbeelden zijn maart 1, 2010; maart 11, 2010; maart 21, 2010; april 1, 2010 |
| ThirdsOfMonthsMmmmDddd | `141` | Voorbeelden zijn maart Begin, maart Midden, maart Einde, april Begin |
| ThirdsOfMonthsMmmmDdddYyyy | `150` | Voorbeelden zijn maart Begin, 2010; maart Midden, 2010; maart Einde, 2010; april Begin, 2010 |
| WeekDddDd | `88` | Voorbeelden zijn Zo 21, Zo 28, Zo 4. Vereist dat de tijdseenheid TimescaleWeeks is. |
| WeekDddMDd | `97` | Voorbeelden zijn Zo M 21, Zo M 28, Zo A 4 |
| WeekDddMmDd | `90` | Voorbeelden zijn Zo 3/21, Zo 3/28, Zo 4/4 |
| WeekDddMmDdYy | `100` | Voorbeelden zijn Zo 3/21/10, Zo 3/28/10, Zo 4/4/10 |
| WeekDddMmmDd | `93` | Voorbeelden zijn Zo mrt 21, Zo mrt 28, Zo apr 4 |
| WeekDddMmmDdYyy | `101` | Voorbeelden zijn Zo mrt 21, '10; Zo mrt 28, '10; Zo apr 4, '10 |
| WeekDddMmmmDd | `96` | Voorbeelden zijn Zo mrt 21, Zo maart 28, Zo apr 4 |
| WeekDddMmmmDdYyy | `102` | Voorbeelden zijn Zo maart 21, '10; Zo maart 28, '10; Zo april 4, '10 |
| WeekDddWw | `103` | Voorbeelden zijn Zo 12, Zo 13, Zo 14 |
| WeekDdiMDd | `98` | Voorbeelden zijn Zo M 21, Zo M 28, Zo A 4 |
| WeekDdiMmDd | `91` | Voorbeelden zijn Zo 3/21. Zo 3/28, Zo 4/4 |
| WeekDdiMmmDd | `94` | Voorbeelden zijn Zo mrt 21, Zo mrt 28, Zo apr 4 |
| WeekDiMDd | `99` | Voorbeelden zijn S M 21, S M 28, S A 4 |
| WeekDiMmDd | `92` | Voorbeelden zijn S 3/21, S 3/28, S 4/4 |
| WeekDiMmmDd | `95` | Voorbeelden zijn S mrt 21, S mrt 28, S apr 4 |
| WeekMDd | `89` | Voorbeelden zijn M21, M28, A 4 |
| WeekMmDd | `17` | Voorbeelden zijn 3/21, 3/28, 4/4 |
| WeekMmDdYy | `16` | Voorbeeld is '3/21/10'. |
| WeekMmmDd | `15` | Voorbeelden zijn mrt 21, mrt 28, apr 4 |
| WeekMmmDdYyy | `13` | Voorbeelden zijn mrt 21, '10; mrt 28, '10; apr 4, '10 |
| WeekMmmmDd | `14` | Voorbeelden zijn maart 21, maart 28, april 4 |
| WeekMmmmDdYyyy | `12` | Voorbeelden zijn maart 21, 2010; maart 28, 2010; april 4, 2010 |
| WeekDayOfMonthDd | `87` | Voorbeelden zijn 21, 28, 4 |
| WeekFromEndWeekWw | `43` | Voorbeelden zijn Week 2, Week 1, Week -1 vanaf het einde van het project. |
| WeekFromEndWw | `68` | Voorbeelden zijn 2, 1, -1 |
| WeekFromEndWww | `67` | Voorbeelden zijn W2, W1, W-1 |
| WeekFromStartWeekWw | `42` | Voorbeelden zijn Week -1, Week 1, Week 2 vanaf het begin van het project. |
| WeekFromStartWw | `70` | Voorbeelden zijn -1, 1, 2 |
| WeekFromStartWww | `69` | Voorbeelden zijn W-1, W1, W2 |
| WeekNumberDdWw | `104` | Voorbeelden zijn 1 12, 1 13, 1 14 (dag 1 van week 12, dag 1 van week 13, enzovoort) |
| WeekNumberWw | `50` | Voorbeelden zijn 12, 13, 14 |
| YearYy | `75` | Voorbeelden zijn 10, 11, 12. Vereist dat de tijdseenheid TimescaleYears is. |
| YearYyy | `1` | Voorbeelden zijn '10, '11, '12 |
| YearYyyy | `0` | Voorbeelden zijn 2010, 2011, 2012 |
| YearFromEndYearYy | `49` | Voorbeelden zijn Jaar 2, Jaar 1, Jaar -1 vanaf het einde van het project. |
| YearFromEndYy | `72` | Voorbeelden zijn 2, 1, -1 |
| YearFromEndYyy | `71` | Voorbeelden zijn Y2, Y1, Y-1 |
| YearFromStartYearYy | `48` | Voorbeelden zijn Jaar -1, Jaar 1, Jaar 2 vanaf het begin van het project. |
| YearFromStartYy | `74` | Voorbeelden zijn -1, 1, 2 |
| YearFromStartYyy | `73` | Voorbeelden zijn Y-1, Y1, Y2 |

## Voorbeelden

Toont hoe tijdsschaallaaglabels aangepast kunnen worden.

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");

// Taakkoppelingen toevoegen
project.TaskLinks.Add(project.RootTask.Children.Add("Task 1"), project.RootTask.Children.Add("Task 2"));

var view = (GanttChartView)project.DefaultView;

// tijdsschaallaag aanpassen

// de bovenste laag afstemmen
// stel de bovenste tijdsschaallaag van de Gantt-diagramweergave in.
view.MiddleTimescaleTier = new TimescaleTier();
// stel tijdsschaaleenheid <see cref="T:Aspose.Tasks.Visualization.TimescaleUnit" /> in voor de tijdsschaallaag.
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
// stel het tijdseenheid-interval in waarin labels voor de laag worden weergegeven.
view.MiddleTimescaleTier.Count = 1;
// stel datumlabel <see cref="T:Aspose.Tasks.Visualization.DateLabel" /> in voor de tijdsschaallaag.
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
// stel in hoe labels binnen elke tijdsperiode van de laag worden uitgelijnd (<see cref="T:System.Drawing.StringAlignment" />).
view.MiddleTimescaleTier.Alignment = HorizontalStringAlignment.Center;
// stel een waarde in die aangeeft of tickmarks die tijdsperioden in de tier scheiden moeten worden weergegeven.
view.MiddleTimescaleTier.ShowTicks = true;
// stel een waarde in die aangeeft of de tier‑labels gebaseerd moeten worden op het fiscale jaar.
view.MiddleTimescaleTier.UsesFiscalYear = true;

// toegevoegd voor betere visualisatie
view.TopTimescaleTier = new TimescaleTier(TimescaleUnit.Months, 1);

// pas de datums van de middelste tier aan
view.TopTimescaleTier.DateTimeConverter = date =>
    new[] { "Янв.", "Фев.", "Мар.", "Апр.", "Май", "Июнь", "Июль", "Авг.", "Сен.", "Окт.", "Ноя.", "Дек." }[date.Month - 1];

project.Set(Prj.TimescaleStart, new DateTime(2012, 7, 30));
project.Set(Prj.TimescaleFinish, new DateTime(2012, 10, 6));

// Gebruik de optie 'Timescale.DefinedInView' om tijdschalen te renderen met tijdschaalinstellingen die in de weergave zijn gedefinieerd (view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier).
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "CustomizeTimescaleTierLabels_out.pdf", pdfSaveOptions);
```

### Zie ook

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


