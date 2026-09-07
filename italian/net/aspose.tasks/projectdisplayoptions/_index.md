---
title: "Classe ProjectDisplayOptions"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.ProjectDisplayOptions. Rappresenta le opzioni di visualizzazione per un'istanza di progetto."
type: docs
weight: 1450
url: /it/net/aspose.tasks/projectdisplayoptions/
---
## ProjectDisplayOptions class

Rappresenta le opzioni di visualizzazione per un'istanza di progetto.

```csharp
public class ProjectDisplayOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [ProjectDisplayOptions](projectdisplayoptions/)() | Inizializza una nuova istanza della classe `ProjectDisplayOptions`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AddSpaceBeforeLabel](../../aspose.tasks/projectdisplayoptions/addspacebeforelabel/) { get; set; } | Ottiene o imposta un valore che indica se aggiungere uno spazio prima del valore numerico e dell'abbreviazione temporale (1 wk rispetto a 1wk). |
| [DayLabel](../../aspose.tasks/projectdisplayoptions/daylabel/) { get; set; } | Ottiene o imposta come viene visualizzata l'etichetta del giorno. |
| [HourLabel](../../aspose.tasks/projectdisplayoptions/hourlabel/) { get; set; } | Ottiene o imposta come viene visualizzata l'etichetta dell'ora. |
| [MinuteLabel](../../aspose.tasks/projectdisplayoptions/minutelabel/) { get; set; } | Ottiene o imposta come viene visualizzata l'etichetta del minuto. |
| [MonthLabel](../../aspose.tasks/projectdisplayoptions/monthlabel/) { get; set; } | Ottiene o imposta come viene visualizzata l'etichetta del mese. |
| [ShowProjectSummaryTask](../../aspose.tasks/projectdisplayoptions/showprojectsummarytask/) { get; set; } | Ottiene o imposta un valore che indica se visualizzare le informazioni di riepilogo di un intero progetto su una singola riga con la propria barra di attività di riepilogo nella parte superiore della vista Gantt Chart. |
| [ShowTaskScheduleSuggestions](../../aspose.tasks/projectdisplayoptions/showtaskschedulesuggestions/) { get; set; } | Ottiene o imposta un valore che indica se mostrare suggerimenti quando Project identifica un possibile conflitto di pianificazione con un'attività programmata manualmente. Questa opzione è disponibile per la versione Project 2010 e successive. |
| [ShowTaskScheduleWarnings](../../aspose.tasks/projectdisplayoptions/showtaskschedulewarnings/) { get; set; } | Ottiene o imposta un valore che indica se mostrare avvisi quando Project identifica un possibile conflitto di pianificazione con un'attività programmata manualmente. Questa opzione è disponibile per la versione Project 2010 e successive. |
| [UnderlineHyperlinks](../../aspose.tasks/projectdisplayoptions/underlinehyperlinks/) { get; set; } | Ottiene o imposta un valore che indica se sottolineare i collegamenti ipertestuali. |
| [WeekLabel](../../aspose.tasks/projectdisplayoptions/weeklabel/) { get; set; } | Ottiene o imposta come viene visualizzata l'etichetta della settimana. |
| [YearLabel](../../aspose.tasks/projectdisplayoptions/yearlabel/) { get; set; } | Ottiene o imposta come viene visualizzata l'etichetta dell'anno. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


