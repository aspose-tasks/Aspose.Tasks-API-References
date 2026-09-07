---
title: "Enum GanttBarShowFor"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.Visualization.GanttBarShowFor. Rappresenta le categorie di attività utilizzate durante la personalizzazione degli stili delle barre del diagramma di Gantt."
type: docs
weight: 3060
url: /it/net/aspose.tasks.visualization/ganttbarshowfor/
---
## GanttBarShowFor enumeration

Rappresenta le categorie di attività utilizzate durante la personalizzazione degli Stili di barra del diagramma di Gantt.

```csharp
public enum GanttBarShowFor
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Normal | `0` | Categoria normale. |
| Milestone | `1` | Categoria milestone. |
| Summary | `2` | Categoria riepilogo. |
| Critical | `3` | Categoria critica. |
| Noncritical | `4` | Categoria non critica. |
| Marked | `5` | Categoria contrassegnata. |
| Finished | `6` | Categoria completata. |
| InProgress | `7` | Categoria InProgress. |
| NotFinished | `8` | Categoria non completata. |
| NotStarted | `9` | Categoria non avviata. |
| StartedLate | `10` | Avviato in ritardo. |
| FinishedLate | `11` | Categoria completata in ritardo. |
| StartedEarly | `12` | Categoria avviata in anticipo. |
| FinishedEarly | `13` | Categoria completata in anticipo. |
| StartedOnTime | `14` | Categoria avviata in tempo. |
| FinishedOnTime | `15` | Categoria completata in tempo. |
| Flag1 | `16` | Categoria Flag1. |
| Flag2 | `17` | Categoria Flag2. |
| Flag3 | `18` | Categoria Flag3. |
| Flag4 | `19` | Categoria Flag4. |
| Flag5 | `20` | Categoria Flag5. |
| Flag6 | `21` | Flag6 categoria. |
| Flag7 | `22` | Flag7 categoria. |
| Flag8 | `23` | Flag8 categoria. |
| Flag9 | `24` | Flag9 categoria. |
| Flag10 | `25` | Flag10 categoria. |
| RolledUp | `26` | Rolled Up categoria. |
| ProjectSummary | `27` | Project Summary categoria. |
| Split | `28` | Split categoria. |
| ExternalTasks | `29` | External Tasks categoria. |
| Flag11 | `30` | Flag11 categoria. |
| Flag12 | `31` | Flag12 categoria. |
| Flag13 | `32` | Flag13 categoria. |
| Flag14 | `33` | Flag14 categoria. |
| Flag15 | `34` | Flag15 categoria. |
| Flag16 | `35` | Flag16 categoria. |
| Flag17 | `36` | Flag17 categoria. |
| Flag18 | `37` | Flag18 categoria. |
| Flag19 | `38` | Flag19 categoria. |
| Flag20 | `39` | Flag20 categoria. |
| GroupBySummary | `40` | Group By Summary categoria. |
| Deliverable | `41` | Deliverable categoria. |
| Dependency | `42` | Dependency categoria. |
| Active | `43` | Active categoria. |
| ManuallyScheduled | `44` | Manually Scheduled categoria. |
| Warning | `45` | Warning categoria. |
| PlaceholderStart | `46` | Segnaposto (Inizio) categoria. |
| PlaceholderFinish | `47` | Segnaposto (Fine) categoria. |
| PlaceholderDuration | `48` | Segnaposto (Durata) categoria. |
| Placeholder | `49` | Segnaposto categoria. |
| Late | `50` | In ritardo categoria. |
| NotNormal | `64` | Non Normale |
| NotMilestone | `65` | Non traguardo categoria. |
| NotSummary | `66` | Non riepilogo categoria. |
| NotCritical | `67` | Non critico categoria. |
| NotMarked | `69` | Non contrassegnato = 69 categoria. |
| NotInProgress | `71` | Non in corso = 71 categoria. |
| NotStartedLate | `74` | Non avviato in ritardo = 74 categoria. |
| NotFinishedLate | `75` | Non finito in ritardo categoria. |
| NotStartedEarly | `76` | Non avviato in anticipo categoria. |
| NotFinishedEarly | `77` | Non finito in anticipo categoria. |
| NotStartedOnTime | `78` | Non avviato in tempo categoria. |
| NotFinishedOnTime | `79` | Non finito in tempo categoria. |
| NotFlag1 | `80` | Non Flag1 categoria. |
| NotFlag2 | `81` | Non Flag2 categoria. |
| NotFlag3 | `82` | Non Flag3 categoria. |
| NotFlag4 | `83` | Non Flag4 categoria. |
| NotFlag5 | `84` | Non Flag5 categoria. |
| NotFlag6 | `85` | Non Flag6 categoria. |
| NotFlag7 | `86` | Non Flag7 categoria. |
| NotFlag8 | `87` | Non Flag8 categoria. |
| NotFlag9 | `88` | Non Flag9 categoria. |
| NotFlag10 | `89` | Non Flag10 categoria. |
| NotRolledUp | `90` | Non Rolled Up categoria. |
| NotProjectSummary | `91` | Non Project Summary categoria. |
| NotSplit | `92` | Non Split categoria. |
| NotExternalTasks | `93` | Non External Tasks categoria. |
| NotFlag11 | `94` | Non Flag11 categoria. |
| NotFlag12 | `95` | Non Flag12 categoria. |
| NotFlag13 | `96` | Non Flag13 categoria. |
| NotFlag14 | `97` | Non Flag14 categoria. |
| NotFlag15 | `98` | Non Flag15 categoria. |
| NotFlag16 | `99` | Non Flag16 categoria. |
| NotFlag17 | `100` | Non Flag17 categoria. |
| NotFlag18 | `101` | Non Flag18 categoria. |
| NotFlag19 | `102` | Non Flag19 categoria. |
| NotFlag20 | `103` | Non Flag20 categoria. |
| NotGroupBySummary | `104` | Non Group By Summary categoria. |
| NotDeliverable | `105` | Non Deliverable categoria. |
| NotDependency | `106` | Non Dependency categoria. |
| NotActive | `107` | Non Active categoria. |
| NotManuallyScheduled | `108` | Non Manually Scheduled categoria. |
| NotWarning | `109` | Non Warning categoria. |
| NotPlaceholderStart | `110` | Non Placeholder (Start) categoria. |
| NotPlaceholderFinish | `111` | Non Placeholder (Finish) categoria. |
| NotPlaceholderDuration | `112` | Non Placeholder (Duration) categoria. |
| NotPlaceholder | `113` | Nessuna categoria segnaposto. |
| NotLate | `114` | Nessuna categoria tardiva. |

## Osservazioni

Vedi la finestra di dialogo 'Bar Styles' del diagramma di Gantt, colonna 'Show For'.

## Esempi

Mostra come utilizzare le categorie ShowFor.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var view = (GanttChartView)project.DefaultView;

var barStyle = this.GetCustomBarStyle();
barStyle.ShowForTaskUid = null;

var showForCategories = new[]
{
    GanttBarShowFor.Active,
    GanttBarShowFor.NotSummary,
    GanttBarShowFor.Milestone,
    GanttBarShowFor.Finished
};

barStyle.ShowForCategories = new List<GanttBarShowFor>(showForCategories);
barStyle.Name = "My common style";
view.BarStyles.Add(barStyle);

// lavorare con il progetto...
```

### Vedi anche

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


