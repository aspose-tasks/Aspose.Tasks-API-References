---
title: "Enum DateLabel"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.Visualization.DateLabel enum. Specifica il formato di visualizzazione per le etichette di data e ora in una scala temporale"
type: docs
weight: 2980
url: /it/net/aspose.tasks.visualization/datelabel/
---
## DateLabel enumeration

Specifica il formato di visualizzazione per le etichette di data e ora in una scala temporale.

```csharp
public enum DateLabel
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `35` | Nessuna data viene visualizzata. |
| DayDdd | `19` | Esempi: Mon, Tue. |
| DayDddDd | `105` | Esempi: Mon 30, Tue 1 |
| DayDddMDd | `112` | Esempi: Mon S 30, Tue O 1 |
| DayDddMmDd | `108` | Esempi: Mon 9/30, Tue 10/1 |
| DayDddMmDdYy | `52` | Esempi: Mon 9/30/02, Tue 10/1/02 |
| DayDddMmmDd | `23` | Esempi: Mon Sep 30, Tue Oct 1 |
| DayDddMmmDdYyy | `22` | Esempi: Mon Sep 30 '02, Tue Oct 1 '02 |
| DayDddMmmmDd | `111` | Esempi: Mon September 30, Tue October 1 |
| DayDddd | `18` | Esempi: Tuesday, Wednesday. |
| DayDdi | `119` | Esempi: Mo, Tu |
| DayDdiDd | `106` | Esempi: Mo 30, Tu 1 |
| DayDdiMDd | `113` | Esempi: Mo S 30, Tu O 1 |
| DayDdiMmDd | `109` | Esempi: Mo 9/30, Tu 10/1 |
| DayDi | `20` | Esempi: M, T |
| DayDiDdSpace | `107` | Esempi: M 30, T 1 |
| DayDiMDd | `114` | Esempi: M S 30, T O 1 |
| DayDiMmDd | `110` | Esempi: M 9/30, T 10/1 |
| DayDiDdNoSpace | `121` | Esempi: M30, T1 |
| DayMDd | `115` | Esempi: S 30, O 1 |
| DayMmDd | `27` | Esempi: 9/30, 10/1 |
| DayMmDdYy | `26` | Esempi: 9/30/02, 10/1/02 |
| DayMmmDd | `25` | Esempi sono Sep 30, Oct 1 |
| DayMmmDdYyy | `24` | Esempi sono Sep 30 '02, Oct 10 '02 |
| DayFromEndDayDd | `41` | Esempi sono Day 2, Day 1, Day -1, Day -2 dalla fine del progetto. |
| DayFromEndDd | `54` | Esempi sono 2, 1, -1, -2 |
| DayFromEndDdd | `53` | Esempi sono D2, D1, D-1, D-2 |
| DayFromStartDayDd | `40` | Esempi sono Day -2, Day -1, Day 1, Day 2 dall'inizio del progetto. |
| DayFromStartDd | `56` | Esempi sono -2, -1, 1, 2 |
| DayFromStartDdd | `55` | Esempi sono D-2, D-1, D1, D2 |
| DayOfMonthDd | `21` | Esempi sono 30, 1 |
| DayOfYearDd | `118` | Esempi sono 77, 78 |
| DayOfYearDdYyy | `116` | Esempi sono 77 '10, 78 '10 |
| DayOfYearDdYyyy | `117` | Esempi sono 77 2010, 78 2010 |
| DayDdMmYyyy | `256` | L'esempio è 19/07/2016. |
| HalfYearH | `128` | Esempi sono 1, 2. Richiede che l'unità di tempo sia TimescaleHalfYears. |
| HalfYearHh | `127` | Esempi sono H1, H2 |
| HalfYearHhYyy | `126` | Esempi sono H1 '10, H2 '10 |
| HalfYearHhhHalf | `123` | Esempi sono 1st Half, 2d Half |
| HalfYearHHyy | `129` | Esempi sono 1H10, 2H10 |
| HalfYearHlfH | `125` | Esempi sono Half 1, Half 2 |
| HalfYearHlfHYyyy | `124` | Esempi sono Half 1, 2010; Half 2, 2010 |
| HalfYearFromEndH | `135` | Esempi sono 2, 1, -1, -2. Metà anni dalla data di fine del progetto. |
| HalfYearFromEndHalfH | `133` | Esempi sono Half 2, Half 1, Half -1, Half -2 |
| HalfYearFromEndHh | `134` | Esempi sono H2, H1, H-1, H-2 |
| HalfYearFromStartH | `132` | Esempi sono -2, -1, 1, 2. Metà anni dalla data di inizio del progetto. |
| HalfYearFromStartHalfH | `130` | Esempi sono Half -2, Half -1, Half 1, Half 2 |
| HalfYearFromStartHh | `131` | Esempi sono H-2, H-1, H1, H2 |
| HourDddMmmDdHhAm | `28` | Esempi sono mer mar 18, 8 AM; mer mar 18, 9 AM. Richiede che l'unità di tempo sia TimescaleHours. |
| HourHh | `32` | Esempi sono 8, 9, 10, 11 |
| HourHhMmAm | `30` | Esempi sono 8:00 AM, 9:00 AM |
| HourHhAm | `31` | Esempi sono 8AM, 9AM |
| HourMmDdHhAm | `120` | Esempi sono 3/18 8 AM, 3/18 9 AM |
| HourMmmDdHhAm | `29` | Esempi sono mar 18, 8 AM; mar 18, 9 AM |
| HourFromEndHh | `77` | Esempi sono 3, 2, 1, -1, -2 ore dal termine del progetto. |
| HourFromEndHhh | `76` | Esempi sono H3, H2, H1, H-1, H-2 |
| HourFromEndHourHh | `39` | Esempi sono Ora 3, Ora 2, Ora 1, Ora -1, Ora -2 |
| HourFromStartHh | `79` | Esempi sono -2, -1, 1, 2, 3 ore dall'inizio del progetto. |
| HourFromStartHhh | `78` | Esempi sono H-2, H-1, H1, H2, H3 |
| HourFromStartHourHh | `38` | Esempi sono Ora -2, Ora -1, Ora 1, Ora 2, Ora 3 |
| MinuteHhMmAm | `33` | Esempi sono 8:00 AM, 8:01 AM, 8:02 AM. Richiede che l'unità di tempo sia TimescaleMinutes. |
| MinuteMm | `34` | Esempi sono 0, 1, 2, ..., 59 minuti |
| MinuteFromEndMinuteMm | `37` | Esempi sono Minuto 181, Minuto 180, ..., Minuto 1, Minuto -1 dal termine del progetto. |
| MinuteFromEndMm | `81` | Esempi sono 181, 180, ..., 1, -1 |
| MinuteFromEndMmm | `80` | Esempi sono M181, M180, ..., M1, M-1 |
| MinuteFromStartMinuteMm | `36` | Esempi sono Minuto -2, Minuto -1, Minuto 1, ... Minuto 180 dall'inizio del progetto. |
| MinuteFromStartMm | `83` | Esempi sono -2, -1, 1, ..., 180 |
| MinuteFromStartMmm | `82` | Esempi sono M-2, M-1, M1, ..., M180 |
| MonthM | `11` | Esempi sono M, A, M, J, J. Richiede che l'unità di tempo sia TimescaleMonths. |
| MonthMm | `57` | Esempi sono 11, 12, 1, 2 |
| MonthMmYy | `86` | Esempi sono 3/10, 4/10, 5/10 |
| MonthMmYyy | `85` | Esempi sono 3 '10, 4 '10, 5 '10 |
| MonthMmm | `10` | Esempi sono Mar, Apr, May |
| MonthMmmYyy | `8` | Esempi sono Mar '10, Apr '10, May '10 |
| MonthMmmm | `9` | Esempi sono marzo, aprile, maggio |
| MonthMmmmYyyy | `7` | Esempi sono marzo 2010, aprile 2010, maggio 2010 |
| MonthFromEndMm | `59` | Esempi sono 2, 1, -1, -2 mesi dal termine del progetto. |
| MonthFromEndMmm | `58` | Esempi sono M2, M1, M-1, M-2 |
| MonthFromEndMonthMm | `45` | Esempi sono Mese 2, Mese 1, Mese -1, Mese -2 |
| MonthFromStartMm | `61` | Esempi sono -2, -2, 1, 2 mesi dall'inizio del progetto. |
| MonthFromStartMmm | `60` | Esempi sono M-2, M-1, M1, M2 |
| MonthFromStartMonthMm | `44` | Esempi sono Mese -2, Mese -1, Mese 1, Mese 2 |
| QuarterQ | `62` | Esempi sono 3, 4, 1. Richiede che l'unità di tempo sia TimescaleQuarters. |
| QuarterQq | `6` | Esempi sono Q3, Q4, Q1 |
| QuarterQqYyy | `4` | Esempi sono Q3 '10, Q4 '10, Q1 '11 |
| QuarterQqqQuarter | `2` | Esempi sono 3° trimestre, 1° trimestre |
| QuarterQQyy | `51` | Esempi sono 3Q10, 4Q10, 1Q11 |
| QuarterQtrQ | `5` | Esempi sono Qtr3, Qtr4, Qtr1 |
| QuarterQtrQYyyy | `3` | Esempi sono Qtr3, 2010; Qtr4, 2010; Qtr1, 2011 |
| QuarterFromEndQ | `64` | Esempi sono 5, 4, 3, 2, 1, -1 trimestri dal termine del progetto. |
| QuarterFromEndQq | `63` | Esempi sono Q5, Q4, Q3, Q2, Q1, Q-1 |
| QuarterFromEndQuarterQ | `47` | Esempi sono Trimestre 5, Trimestre 4, Trimestre 3, Trimestre 2, Trimestre 1, Trimestre -1 |
| QuarterFromStartQ | `66` | Esempi sono -5, -4, -3, -2, -1, 1 trimestri dall'inizio del progetto. |
| QuarterFromStartQq | `65` | Esempi sono Q-5, Q-4, Q-3, Q-2, Q-1, Q1 |
| QuarterFromStartQuarterQ | `46` | Esempi sono Trimestre -5, Trimestre -4, Trimestre -3, Trimestre -2, Trimestre -1, Trimestre 1 |
| ThirdsOfMonthsDd | `136` | Esempi sono 1, 11, 21, 1. Richiede che l'unità di tempo sia TimescaleThirdsOfMonths. |
| ThirdsOfMonthsDdd | `137` | Esempi sono B, M, E, B |
| ThirdsOfMonthsDddd | `138` | Gli esempi sono Inizio, Metà, Fine, Inizio |
| ThirdsOfMonthsMmDd | `139` | L'esempio è 3/1. |
| ThirdsOfMonthsMmDdYy | `145` | L'esempio è 3/1/10. |
| ThirdsOfMonthsMmDdd | `140` | Gli esempi sono 3/B, 3/M, 3/E, 4/B |
| ThirdsOfMonthsMmDddYy | `146` | L'esempio è 3/B/10. |
| ThirdsOfMonthsMmmDd | `142` | Gli esempi sono mar 1, mar 11, mar 21, apr 1 |
| ThirdsOfMonthsMmmDdYy | `147` | Gli esempi sono mar 1, '10; mar 11, '10; mar 21, '10; apr 1, 10 |
| ThirdsOfMonthsMmmDdd | `143` | Gli esempi sono mar B, mar M, mar E, apr B |
| ThirdsOfMonthsMmmDddYy | `148` | Gli esempi sono mar B, '10; mar M, '10; mar E, '10; apr B '10 |
| ThirdsOfMonthsMmmmDd | `144` | Gli esempi sono marzo 1, marzo 11, marzo 21, aprile 1 |
| ThirdsOfMonthsMmmmDdYyyy | `149` | Gli esempi sono marzo 1, 2010; marzo 11, 2010; marzo 21, 2010; aprile 1, 2010 |
| ThirdsOfMonthsMmmmDddd | `141` | Gli esempi sono marzo Inizio, marzo Metà, marzo Fine, aprile Inizio |
| ThirdsOfMonthsMmmmDdddYyyy | `150` | Gli esempi sono marzo Inizio, 2010; marzo Metà, 2010; marzo Fine, 2010; aprile Inizio, 2010 |
| WeekDddDd | `88` | Gli esempi sono dom 21, dom 28, dom 4. Richiede che l'unità di tempo sia TimescaleWeeks. |
| WeekDddMDd | `97` | Gli esempi sono dom M 21, dom M 28, dom A 4 |
| WeekDddMmDd | `90` | Gli esempi sono dom 3/21, dom 3/28, dom 4/4 |
| WeekDddMmDdYy | `100` | Gli esempi sono dom 3/21/10, dom 3/28/10, dom 4/4/10 |
| WeekDddMmmDd | `93` | Gli esempi sono dom mar 21, dom mar 28, dom apr 4 |
| WeekDddMmmDdYyy | `101` | Gli esempi sono dom mar 21, '10; dom mar 28, '10; dom apr 4, '10 |
| WeekDddMmmmDd | `96` | Gli esempi sono dom mar 21, dom marzo 28, dom apr 4 |
| WeekDddMmmmDdYyy | `102` | Gli esempi sono dom marzo 21, '10; dom marzo 28, '10; dom aprile 4, '10 |
| WeekDddWw | `103` | Gli esempi sono dom 12, dom 13, dom 14 |
| WeekDdiMDd | `98` | Gli esempi sono dom M 21, dom M 28, dom A 4 |
| WeekDdiMmDd | `91` | Gli esempi sono dom 3/21. dom 3/28, dom 4/4 |
| WeekDdiMmmDd | `94` | Gli esempi sono dom mar 21, dom mar 28, dom apr 4 |
| WeekDiMDd | `99` | Gli esempi sono S M 21, S M 28, S A 4 |
| WeekDiMmDd | `92` | Gli esempi sono S 3/21, S 3/28, S 4/4 |
| WeekDiMmmDd | `95` | Gli esempi sono S Mar 21, S Mar 28, S Apr 4 |
| WeekMDd | `89` | Gli esempi sono M21, M28, A 4 |
| WeekMmDd | `17` | Gli esempi sono 3/21, 3/28, 4/4 |
| WeekMmDdYy | `16` | L'esempio è '3/21/10'. |
| WeekMmmDd | `15` | Gli esempi sono Mar 21, Mar 28, Apr 4 |
| WeekMmmDdYyy | `13` | Gli esempi sono Mar 21, '10; Mar 28, '10; Apr 4, '10 |
| WeekMmmmDd | `14` | Gli esempi sono Marzo 21, Marzo 28, Aprile 4 |
| WeekMmmmDdYyyy | `12` | Gli esempi sono Marzo 21, 2010; Marzo 28, 2010; Aprile 4, 2010 |
| WeekDayOfMonthDd | `87` | Gli esempi sono 21, 28, 4 |
| WeekFromEndWeekWw | `43` | Gli esempi sono Settimana 2, Settimana 1, Settimana -1 dalla fine del progetto. |
| WeekFromEndWw | `68` | Gli esempi sono 2, 1, -1 |
| WeekFromEndWww | `67` | Gli esempi sono W2, W1, W-1 |
| WeekFromStartWeekWw | `42` | Gli esempi sono Settimana -1, Settimana 1, Settimana 2 dall'inizio del progetto. |
| WeekFromStartWw | `70` | Gli esempi sono -1, 1, 2 |
| WeekFromStartWww | `69` | Gli esempi sono W-1, W1, W2 |
| WeekNumberDdWw | `104` | Gli esempi sono 1 12, 1 13, 1 14 (giorno 1 della settimana 12, giorno 1 della settimana 13, e così via) |
| WeekNumberWw | `50` | Gli esempi sono 12, 13, 14 |
| YearYy | `75` | Gli esempi sono 10, 11, 12. Richiede che l'unità di tempo sia TimescaleYears. |
| YearYyy | `1` | Gli esempi sono '10, '11, '12 |
| YearYyyy | `0` | Gli esempi sono 2010, 2011, 2012 |
| YearFromEndYearYy | `49` | Gli esempi sono Anno 2, Anno 1, Anno -1 dalla fine del progetto. |
| YearFromEndYy | `72` | Gli esempi sono 2, 1, -1 |
| YearFromEndYyy | `71` | Gli esempi sono Y2, Y1, Y-1 |
| YearFromStartYearYy | `48` | Gli esempi sono Anno -1, Anno 1, Anno 2 dall'inizio del progetto. |
| YearFromStartYy | `74` | Gli esempi sono -1, 1, 2 |
| YearFromStartYyy | `73` | Gli esempi sono Y-1, Y1, Y2 |

## Esempi

Mostra come personalizzare le etichette del livello della scala temporale.

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");

// Aggiungi collegamenti alle attività
project.TaskLinks.Add(project.RootTask.Children.Add("Task 1"), project.RootTask.Children.Add("Task 2"));

var view = (GanttChartView)project.DefaultView;

// regola i livelli della scala temporale

// regola il livello superiore
// imposta il livello superiore della scala temporale della vista del diagramma di Gantt.
view.MiddleTimescaleTier = new TimescaleTier();
// imposta l'unità della scala temporale <see cref=\"T:Aspose.Tasks.Visualization.TimescaleUnit\" /> per il livello della scala temporale.
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
// imposta l'intervallo dell'unità di tempo in cui mostrare le etichette per il livello.
view.MiddleTimescaleTier.Count = 1;
// imposta l'etichetta data <see cref=\"T:Aspose.Tasks.Visualization.DateLabel\" /> per il livello della scala temporale.
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
// imposta come allineare le etichette all'interno di ogni periodo di tempo del livello (<see cref=\"T:System.Drawing.StringAlignment\" />).
view.MiddleTimescaleTier.Alignment = HorizontalStringAlignment.Center;
// imposta un valore che indica se mostrare i segni di spunta che separano i periodi di tempo nel livello.
view.MiddleTimescaleTier.ShowTicks = true;
// imposta un valore che indica se basare le etichette del livello sull'anno fiscale.
view.MiddleTimescaleTier.UsesFiscalYear = true;

// aggiunto per una migliore visualizzazione
view.TopTimescaleTier = new TimescaleTier(TimescaleUnit.Months, 1);

// personalizza le date del livello intermedio
view.TopTimescaleTier.DateTimeConverter = date =>
    new[] { "Янв.", "Фев.", "Мар.", "Апр.", "Май", "Июнь", "Июль", "Авг.", "Сен.", "Окт.", "Ноя.", "Дек." }[date.Month - 1];

project.Set(Prj.TimescaleStart, new DateTime(2012, 7, 30));
project.Set(Prj.TimescaleFinish, new DateTime(2012, 10, 6));

// Usa l'opzione 'Timescale.DefinedInView' per renderizzare le scale temporali utilizzando le impostazioni della scala temporale definite nella vista (view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier).
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "CustomizeTimescaleTierLabels_out.pdf", pdfSaveOptions);
```

### Vedi anche

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


