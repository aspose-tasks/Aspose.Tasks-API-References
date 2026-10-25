---
title: "Class PrimaveraSaveOptions"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Saving.PrimaveraSaveOptions. Consente di specificare opzioni aggiuntive durante il salvataggio del progetto nel formato Primavera XER"
type: docs
weight: 2150
url: /it/net/aspose.tasks.saving/primaverasaveoptions/
---
## PrimaveraSaveOptions class

Consente di specificare opzioni aggiuntive durante il salvataggio del progetto nel formato Primavera XER.

```csharp
public class PrimaveraSaveOptions : SimpleSaveOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [PrimaveraSaveOptions](primaverasaveoptions/)() | Inizializza una nuova istanza della classe `PrimaveraSaveOptions`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ActivityIdIncrement](../../aspose.tasks.saving/primaverasaveoptions/activityidincrement/) { get; set; } | Ottiene o imposta l'incremento utilizzato nella ridenominazione degli ID delle attività. |
| [ActivityIdPrefix](../../aspose.tasks.saving/primaverasaveoptions/activityidprefix/) { get; set; } | Ottiene o imposta il prefisso utilizzato nella ridenominazione degli ID delle attività. |
| [ActivityIdSuffix](../../aspose.tasks.saving/primaverasaveoptions/activityidsuffix/) { get; set; } | Ottiene o imposta il suffisso utilizzato nella ridenominazione degli ID delle attività. |
| [RenumberActivityIds](../../aspose.tasks.saving/primaverasaveoptions/renumberactivityids/) { get; set; } | Ottiene o imposta un valore che indica se è necessario ridenominare gli ID delle attività. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Ottiene o imposta il formato in cui il documento verrà salvato se viene utilizzato questo oggetto di opzioni di salvataggio. |
| [SkipSummaryAssignments](../../aspose.tasks.saving/primaverasaveoptions/skipsummaryassignments/) { get; set; } | Ottiene o imposta un valore che indica se le assegnazioni di risorse alle attività riepilogo devono essere omesse durante l'esportazione. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Ottiene o imposta il comparatore per ordinare le attività nel diagramma di Gantt e nella tabella delle attività. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Ottiene o imposta la condizione utilizzata per filtrare le attività visualizzate nei diagrammi Gantt, nella tabella delle attività e nell'utilizzo delle attività. |

## Esempi

Mostra come lavorare con &lt;see cref="Aspose.Tasks.Saving.PrimaveraSaveOptions" /&gt;.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// crea le opzioni di salvataggio Primavera e personalizzale
var options = new PrimaveraSaveOptions
                  {
                      // definisci prefisso e suffisso di un'attività
                      ActivityIdPrefix = "TEST",
                      ActivityIdSuffix = 10000,

                      // controlla la ridenominazione delle attività
                      ActivityIdIncrement = 5,
                      RenumberActivityIds = true
                  };

project.Save(OutDir + "WorkWithPrimaveraSaveOptions_out.xer", options);
```

### Vedi anche

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


