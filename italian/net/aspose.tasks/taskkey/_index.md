---
title: TaskKey
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: Rappresenta un elenco di campi attività supportati.
type: docs
weight: 2100
url: /it/net/aspose.tasks/taskkey/
---
## TaskKey enumeration

Rappresenta un elenco di campi attività supportati.

```csharp
public enum TaskKey
```

### I valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Uid | `0` | Rappresenta ilUid Campo (attività). |
| Id | `1` | Rappresenta il campo ID (attività). |
| Name | `2` | Rappresenta il campo Nome (attività). |
| Type | `3` | Rappresenta il campo Tipo (attività). |
| IsNull | `4` | Rappresenta il campo IsNull (attività). |
| Created | `5` | Rappresenta il campo Creato (attività). |
| Contact | `6` | Rappresenta il campo Contatto (attività). |
| WBS | `7` | Rappresenta il campo WBS (attività). |
| WBSLevel | `8` | Rappresenta il campo WBSLevel (attività). |
| OutlineNumber | `9` | Rappresenta il campo OutlineNumber (attività). |
| OutlineLevel | `10` | Rappresenta il campo OutlineLevel (attività). |
| Priority | `11` | Rappresenta il campo Priorità (attività). |
| Start | `12` | Rappresenta il campo Inizio (attività). |
| Finish | `13` | Rappresenta il campo Fine (attività). |
| Duration | `14` | Rappresenta il campo Durata (attività). |
| DurationVariance | `15` | Rappresenta il campo DurationVariance (attività). |
| DurationFormat | `16` | Rappresenta il campo DurationFormat (attività). |
| Work | `17` | Rappresenta il campo Lavoro (attività). |
| Stop | `18` | Rappresenta il campo Stop (attività). |
| Resume | `19` | Rappresenta il campo Riprendi (attività). |
| IsResumeValid | `20` | Rappresenta il campo IsResumeValid (attività). |
| IsEffortDriven | `21` | Rappresenta il campo IsEffortDriven (attività). |
| IsRecurring | `22` | Rappresenta il campo IsRecurring (attività). |
| IsOverallocated | `23` | Rappresenta il campo IsOverallocated (attività). |
| HasOverallocatedResource | `24` | Rappresenta il campo HasOverallocatedResource (attività). |
| IsEstimated | `25` | Rappresenta il campo IsEstimated (attività). |
| IsMilestone | `26` | Rappresenta il campo IsMilestone (attività). |
| IsCritical | `27` | Rappresenta il campo IsCritical (attività). |
| IsSubproject | `28` | Rappresenta il campo IsSubproject (attività). |
| IsSubprojectReadOnly | `29` | Rappresenta il campo IsSubprojectReadOnly (attività). |
| IsMarked | `30` | Rappresenta il campo IsMarked (attività). |
| IgnoreWarnings | `31` | Rappresenta il campo IgnoraAvvisi (attività). |
| SubprojectName | `32` | Rappresenta il campo Nome sottoprogetto (attività). |
| IsExternalTask | `33` | Rappresenta il campo IsExternalTask (attività). |
| IsSummary | `34` | Rappresenta il campo IsSummary (attività). |
| ExternalTaskProject | `35` | Rappresenta il campo ExternalTaskProject (attività). |
| ExternalId | `36` | Rappresenta il campo ExternalId (attività). |
| ExternalKey | `37` | Rappresenta il campo ExternalKey (attività). |
| EarlyStart | `38` | Rappresenta il campo EarlyStart (attività). |
| EarlyFinish | `39` | Rappresenta il campo EarlyFinish (attività). |
| LateStart | `40` | Rappresenta il campo LateStart (attività). |
| LateFinish | `41` | Rappresenta il campo LateFinish (attività). |
| StartVariance | `42` | Rappresenta il campo StartVariance (attività). |
| FinishVariance | `43` | Rappresenta il campo FinishVariance (attività). |
| WorkVariance | `44` | Rappresenta il campo WorkVariance (attività). |
| CostVariance | `45` | Rappresenta il campo CostVariance (attività). |
| FreeSlack | `46` | Rappresenta il campo FreeSlack (attività). |
| TotalSlack | `47` | Rappresenta il campo TotalSlack (attività). |
| StartSlack | `48` | Rappresenta il campo StartSlack (attività). |
| FinishSlack | `49` | Rappresenta il campo FinishSlack (attività). |
| FixedCost | `50` | Rappresenta il campo Costo Fisso (attività). |
| FixedCostAccrual | `51` | Rappresenta il campo FixedCostAccrual (attività). |
| PercentComplete | `52` | Rappresenta il campo PercentComplete (attività). |
| PercentWorkComplete | `53` | Rappresenta il campo PercentWorkComplete (attività). |
| Cost | `54` | Rappresenta il campo Costo (attività). |
| OvertimeCost | `55` | Rappresenta il campo OvertimeCost (attività). |
| ActualStart | `56` | Rappresenta il campo ActualStart (attività). |
| ActualFinish | `57` | Rappresenta il campo ActualFinish (attività). |
| ActualDuration | `58` | Rappresenta il campo ActualDuration (attività). |
| ActualCost | `59` | Rappresenta il campo Costo effettivo (attività). |
| ActualOvertimeCost | `60` | Rappresenta il campo ActualOvertimeCost (attività). |
| ActualWork | `61` | Rappresenta il campo ActualWork (attività). |
| ActualOvertimeWork | `62` | Rappresenta il campo ActualOvertimeWork (attività). |
| OvertimeWork | `63` | Rappresenta il campo Lavoro straordinario (attività). |
| RegularWork | `64` | Rappresenta il campo RegularWork (attività). |
| RemainingDuration | `65` | Rappresenta il campo RemainingDuration (attività). |
| RemainingCost | `66` | Rappresenta il campo Costo residuo (attività). |
| RemainingWork | `67` | Rappresenta il campo RemainingWork (attività). |
| RemainingOvertimeWork | `68` | Rappresenta il campo RemainingOvertimeWork (attività). |
| RemainingOvertimeCost | `69` | Rappresenta il campo RemainingOvertimeCost (attività). |
| ACWP | `70` | Rappresenta il campo ACWP (attività). |
| CV | `71` | Rappresenta il campo CV (attività). |
| SV | `72` | Rappresenta il campo SV (attività). |
| ConstraintType | `73` | Rappresenta il campo ConstraintType (Task). |
| Calendar | `74` | Rappresenta il campo Calendario (attività). |
| ConstraintDate | `75` | Rappresenta il campo Data vincolo (attività). |
| Deadline | `76` | Rappresenta il campo Scadenza (attività). |
| LevelAssignments | `77` | Rappresenta il campo LevelAssignments (Task). |
| LevelingCanSplit | `78` | Rappresenta il campo LevelingCanSplit (attività). |
| LevelingDelay | `79` | Rappresenta il campo LevelingDelay (attività). |
| LevelingDelayFormat | `80` | Rappresenta il campo LevelingDelayFormat (attività). |
| PreleveledStart | `81` | Rappresenta il campo PreleveledStart (attività). |
| PreleveledFinish | `82` | Rappresenta il campo PreleveledFinish (Task). |
| Hyperlink | `83` | Rappresenta il campo Collegamento ipertestuale (attività). |
| HyperlinkAddress | `84` | Rappresenta il campo HyperlinkAddress (attività). |
| HyperlinkSubAddress | `85` | Rappresenta il campo HyperlinkSubAddress (attività). |
| IgnoreResourceCalendar | `86` | Rappresenta il campo IgnoreResourceCalendar (attività). |
| HideBar | `87` | Rappresenta il campo HideBar (attività). |
| IsRollup | `88` | Rappresenta il campo IsRollup (attività). |
| BCWS | `89` | Rappresenta il campo BCWS (attività). |
| BCWP | `90` | Rappresenta il campo BCWP (attività). |
| PhysicalPercentComplete | `91` | Rappresenta il campo PhysicalPercentComplete (attività). |
| EarnedValueMethod | `92` | Rappresenta il campo EarnedValueMethod (attività). |
| ActualWorkProtected | `93` | Rappresenta il campo ActualWorkProtected (attività). |
| ActualOvertimeWorkProtected | `94` | Rappresenta il campo ActualOvertimeWorkProtected (attività). |
| IsPublished | `95` | Rappresenta il campo IsPublished (attività). |
| IsScheduled | `96` | Rappresenta il campo IsScheduled (attività). |
| StatusManager | `97` | Rappresenta il campo StatusManager (attività). |
| CommitmentStart | `98` | Rappresenta il campo CommitmentStart (attività). |
| CommitmentFinish | `99` | Rappresenta il campo CommitmentFinish (attività). |
| CommitmentType | `100` | Rappresenta il campo CommitmentType (Task). |
| IsManual | `101` | Rappresenta il campo IsManual (attività). |
| IsExpanded | `102` | Rappresenta il campo IsExpanded (attività). |
| Guid | `103` | Rappresenta il campo Guid (attività). |
| NotesText | `104` | Rappresenta il campo NotesText (attività). |
| NotesRTF | `105` | Rappresenta il campo NotesRTF (attività). |
| ManualStart | `106` | Rappresenta il campo ManualStart (attività). |
| ManualFinish | `107` | Rappresenta il campo Fine manuale (attività). |
| ManualDuration | `108` | Rappresenta il campo ManualDuration (attività). |
| BudgetWork | `109` | Rappresenta il campo BudgetWork (attività). |
| BudgetCost | `110` | Rappresenta il campo BudgetCost (attività). |
| DisplayAsSummary | `111` | Rappresenta il campo DisplayAsSummary (attività). |
| SummaryProgress | `112` | Rappresenta il campo Riepilogo avanzamento (attività). |
| IsActive | `113` | Rappresenta il campo IsActive (attività). |
| StartText | `114` | Rappresenta il campo StartText (attività). |
| FinishText | `115` | Rappresenta il campo FinishText (attività). |
| DurationText | `116` | Rappresenta il campo DurationText (attività). |
| CalendarUid | `117` | Rappresenta il campo CalendarUid (attività). |
| ParentTaskUid | `118` | Rappresenta il campo ParentTaskUid (attività). |
| DisplayOnTimeline | `119` | Rappresenta il campo DisplayOnTimeline (attività). |
| TaskIsAssigned | `120` | Rappresenta il campo TaskIsAssigned (Task). |
| TaskOriginalStart | `121` | Rappresenta il campo di inizio (attività) originale. |
| TaskOriginalFinish | `122` | Rappresenta il campo di finitura (attività) originale. |
| IsShowBeforeProjectStartDateWarning | `123` | Rappresenta il flag che fa sì che MSP mostri l'avviso che un'attività sta iniziando prima della data di inizio del progetto. |
| Warning | `124` | Rappresenta il flag che indica che l'attività presenta discrepanze nella pianificazione. |
| ParentTaskGuid | `125` | Rappresenta il campo ParentTaskGuid (attività). |
| ActivityId | `126` | Rappresenta il campo ActivityId (applicabile solo ai progetti Primavera). |
| FreeSlackTimeSpan | `127` | Rappresenta il campo FreeSlack (attività). |
| TotalSlackTimeSpan | `128` | Rappresenta il campo TotalSlack (attività). |
| StartSlackTimeSpan | `129` | Rappresenta il campo StartSlack (attività). |
| FinishSlackTimeSpan | `130` | Rappresenta il campo FinishSlack (attività). |

### Guarda anche

* spazio dei nomi [Aspose.Tasks](../../aspose.tasks)
* assemblea [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
