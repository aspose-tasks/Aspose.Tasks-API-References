---
title: "Enum AsnKey"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.AsnKey enum. Rappresenta un elenco di campi di assegnazione supportati"
type: docs
weight: 40
url: /it/net/aspose.tasks/asnkey/
---
## AsnKey enumeration

Rappresenta un elenco di campi di assegnazione supportati.

```csharp
public enum AsnKey : byte
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Guid | `0` | Rappresenta il campo Guid (ResourceAssignment). |
| Uid | `1` | Rappresenta il campo UID (ResourceAssignment). |
| Task | `2` | Rappresenta il campo Task (ResourceAssignment). |
| Resource | `3` | Rappresenta il campo Resource (ResourceAssignment). |
| PercentWorkComplete | `4` | Rappresenta il campo PercentWorkComplete (ResourceAssignment). |
| ActualCost | `5` | Rappresenta il campo ActualCost (ResourceAssignment). |
| ActualFinish | `6` | Rappresenta il campo ActualFinish (ResourceAssignment). |
| ActualOvertimeCost | `7` | Rappresenta il campo ActualOvertimeCost (ResourceAssignment). |
| ActualStart | `8` | Rappresenta il campo ActualStart (ResourceAssignment). |
| ActualWork | `9` | Rappresenta il campo ActualWork (ResourceAssignment). |
| ActualOvertimeWork | `10` | Rappresenta il campo ActualOvertimeWork (ResourceAssignment). |
| ACWP | `11` | Rappresenta il campo ACWP (ResourceAssignment). |
| Confirmed | `12` | Rappresenta il campo Confirmed (ResourceAssignment). |
| Cost | `13` | Rappresenta il campo Cost (ResourceAssignment). |
| CostRateTableType | `14` | Rappresenta il campo CostRateTableType (ResourceAssignment). |
| CostVariance | `15` | Rappresenta il campo CostVariance (ResourceAssignment). |
| CV | `16` | Rappresenta il campo CV (ResourceAssignment). |
| Delay | `17` | Rappresenta il campo Delay (ResourceAssignment). |
| Finish | `18` | Rappresenta il campo Finish (ResourceAssignment). |
| FinishVariance | `19` | Rappresenta il campo FinishVariance (ResourceAssignment). |
| Hyperlink | `20` | Rappresenta il campo Hyperlink (ResourceAssignment). |
| HyperlinkAddress | `21` | Rappresenta il campo HyperlinkAddress (ResourceAssignment). |
| HyperlinkSubAddress | `22` | Rappresenta il campo HyperlinkSubAddress (ResourceAssignment). |
| WorkVariance | `23` | Rappresenta il campo WorkVariance (ResourceAssignment). |
| HasFixedRateUnits | `24` | Rappresenta il campo HasFixedRateUnits (ResourceAssignment). |
| FixedMaterial | `25` | Rappresenta il campo FixedMaterial (ResourceAssignment). |
| LevelingDelay | `26` | Rappresenta il campo LevelingDelay (ResourceAssignment). |
| LinkedFields | `27` | Rappresenta il campo LinkedFields (ResourceAssignment). |
| Milestone | `28` | Rappresenta il campo Milestone (ResourceAssignment). |
| Notes | `29` | Rappresenta il campo Notes (ResourceAssignment). |
| NotesText | `30` | Rappresenta il campo NotesText (ResourceAssignment). |
| NotesRTF | `31` | Rappresenta il campo NotesRTF (ResourceAssignment). |
| Overallocated | `32` | Rappresenta il campo Overallocated (ResourceAssignment). |
| OvertimeCost | `33` | Rappresenta il campo OvertimeCost (ResourceAssignment). |
| OvertimeWork | `34` | Rappresenta il campo OvertimeWork (ResourceAssignment). |
| PeakUnits | `35` | Rappresenta il campo PeakUnits (ResourceAssignment). |
| RegularWork | `36` | Rappresenta il campo RegularWork (ResourceAssignment). |
| RemainingCost | `37` | Rappresenta il campo RemainingCost (ResourceAssignment). |
| RemainingOvertimeCost | `38` | Rappresenta il campo RemainingOvertimeCost (ResourceAssignment). |
| RemainingOvertimeWork | `39` | Rappresenta il campo RemainingOvertimeWork (ResourceAssignment). |
| RemainingWork | `40` | Rappresenta il campo RemainingWork (ResourceAssignment). |
| ResponsePending | `41` | Rappresenta il campo ResponsePending (ResourceAssignment). |
| Start | `42` | Rappresenta il campo Start (ResourceAssignment). |
| Stop | `43` | Rappresenta il campo Stop (ResourceAssignment). |
| Resume | `44` | Rappresenta il campo Resume (ResourceAssignment). |
| StartVariance | `45` | Rappresenta il campo StartVariance (ResourceAssignment). |
| Summary | `46` | Rappresenta il campo Summary (ResourceAssignment). |
| SV | `47` | Rappresenta il campo SV (ResourceAssignment). |
| Units | `48` | Rappresenta il campo Units (ResourceAssignment). |
| UpdateNeeded | `49` | Rappresenta il campo UpdateNeeded (ResourceAssignment). |
| VAC | `50` | Rappresenta il campo VAC (ResourceAssignment). |
| Work | `51` | Rappresenta il campo Work (ResourceAssignment). |
| WorkContour | `52` | Rappresenta il campo WorkContour (ResourceAssignment). |
| BCWS | `53` | Rappresenta il campo BCWS (ResourceAssignment). |
| BCWP | `54` | Rappresenta il campo BCWP (ResourceAssignment). |
| BookingType | `55` | Rappresenta il campo BookingType (ResourceAssignment). |
| ActualWorkProtected | `56` | Rappresenta il campo ActualWorkProtected (ResourceAssignment). |
| ActualOvertimeWorkProtected | `57` | Rappresenta il campo ActualOvertimeWorkProtected (ResourceAssignment). |
| Created | `58` | Rappresenta il campo Created (ResourceAssignment). |
| AssignmentOwner | `59` | Rappresenta il campo AssignmentOwner (ResourceAssignment). |
| AssignmentOwnerGuid | `60` | Rappresenta il campo AssignmentOwnerGuid (ResourceAssignment). |
| BudgetWork | `61` | Rappresenta il campo BudgetWork (ResourceAssignment). |
| BudgetCost | `62` | Rappresenta il campo BudgetCost (ResourceAssignment). |
| RateScale | `63` | Rappresenta il campo RateScale (ResourceAssignment). |
| TaskUid | `64` | Rappresenta il campo TaskUid (ResourceAssignment). |
| ResourceUid | `65` | Rappresenta il campo ResourceUid (ResourceAssignment). |

## Esempi

Mostra come leggere/scrivere le proprietà comuni.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Start, new DateTime(2020, 4, 9, 8, 0, 0));
assignment.Set(Asn.Work, project.GetWork(1));
assignment.Set(Asn.Finish, new DateTime(2020, 4, 9, 17, 0, 0));
assignment.Set(Asn.Units, 1);
assignment.Set(Asn.PeakUnits, 1);

Console.WriteLine("Start: " + assignment.Get(Asn.Start));
Console.WriteLine("Work: " + assignment.Get(Asn.Work));
Console.WriteLine("Finish: " + assignment.Get(Asn.Finish));
Console.WriteLine("Units: " + assignment.Get(Asn.Units));
Console.WriteLine("Peak Units: " + assignment.Get(Asn.PeakUnits));
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


