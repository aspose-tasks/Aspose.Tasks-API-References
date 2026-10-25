---
title: "ProjectDisplayOptions.HourLabel"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà ProjectDisplayOptions. Ottiene o imposta come viene visualizzata l'etichetta dell'ora"
type: docs
weight: 40
url: /it/net/aspose.tasks/projectdisplayoptions/hourlabel/
---
## ProjectDisplayOptions.HourLabel property

Ottiene o imposta come viene visualizzata l'etichetta dell'ora.

```csharp
public HourLabelDisplay HourLabel { get; set; }
```

## Esempi

Mostra come utilizzare le opzioni di visualizzazione del progetto.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// Imposta un valore che indica se mostrare avvisi quando Project identifica un possibile conflitto di pianificazione con un'attività programmata manualmente.
// Questa opzione è disponibile per la versione Project 2010 e successive.
project.DisplayOptions.ShowTaskScheduleWarnings = false;

// un valore che indica se aggiungere uno spazio prima del valore numerico e dell'abbreviazione temporale (1 wk anziché 1wk)
project.DisplayOptions.AddSpaceBeforeLabel = true;

// imposta come viene visualizzata l'etichetta dei minuti
project.DisplayOptions.MinuteLabel = MinuteLabelDisplay.Min;

// imposta come viene visualizzata l'etichetta dell'ora
project.DisplayOptions.HourLabel = HourLabelDisplay.Hr;

// imposta come viene visualizzata l'etichetta del giorno
project.DisplayOptions.DayLabel = DayLabelDisplay.Dy;

// imposta come viene visualizzata l'etichetta della settimana
project.DisplayOptions.WeekLabel = WeekLabelDisplay.Week;

// imposta come viene visualizzata l'etichetta del mese
project.DisplayOptions.MonthLabel = MonthLabelDisplay.Mon;

// imposta come viene visualizzata l'etichetta dell'anno
project.DisplayOptions.YearLabel = YearLabelDisplay.Year;

// imposta un valore che indica se visualizzare le informazioni di riepilogo di un intero progetto su una singola riga con la propria barra di attività di riepilogo nella parte superiore della visualizzazione del diagramma di Gantt.
project.DisplayOptions.ShowProjectSummaryTask = true;

// imposta un valore che indica se mostrare suggerimenti quando Project identifica un possibile conflitto di pianificazione con un'attività programmata manualmente.
project.DisplayOptions.ShowTaskScheduleSuggestions = true;

// imposta un valore che indica se sottolineare i collegamenti ipertestuali.
project.DisplayOptions.UnderlineHyperlinks = true;

project.Save(OutDir + "WorkWithProjectDisplayOptions.mpp", SaveFileFormat.Mpp);
```

### Vedi anche

* enum [HourLabelDisplay](../../hourlabeldisplay/)
* class [ProjectDisplayOptions](../)
* namespace [Aspose.Tasks](../../projectdisplayoptions/)
* assembly [Aspose.Tasks](../../../)


