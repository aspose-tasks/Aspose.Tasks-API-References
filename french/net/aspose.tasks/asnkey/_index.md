---
title: "Enum AsnKey"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.AsnKey enum. Représente une liste de champs d'affectation pris en charge"
type: docs
weight: 40
url: /fr/net/aspose.tasks/asnkey/
---
## AsnKey enumeration

Représente une liste des champs d’affectation pris en charge.

```csharp
public enum AsnKey : byte
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Guid | `0` | Représente le champ Guid (ResourceAssignment). |
| Uid | `1` | Représente le champ UID (ResourceAssignment). |
| Task | `2` | Représente le champ Task (ResourceAssignment). |
| Resource | `3` | Représente le champ Resource (ResourceAssignment). |
| PercentWorkComplete | `4` | Représente le champ PercentWorkComplete (ResourceAssignment). |
| ActualCost | `5` | Représente le champ ActualCost (ResourceAssignment). |
| ActualFinish | `6` | Représente le champ ActualFinish (ResourceAssignment). |
| ActualOvertimeCost | `7` | Représente le champ ActualOvertimeCost (ResourceAssignment). |
| ActualStart | `8` | Représente le champ ActualStart (ResourceAssignment). |
| ActualWork | `9` | Représente le champ ActualWork (ResourceAssignment). |
| ActualOvertimeWork | `10` | Représente le champ ActualOvertimeWork (ResourceAssignment). |
| ACWP | `11` | Représente le champ ACWP (ResourceAssignment). |
| Confirmed | `12` | Représente le champ Confirmed (ResourceAssignment). |
| Cost | `13` | Représente le champ Cost (ResourceAssignment). |
| CostRateTableType | `14` | Représente le champ CostRateTableType (ResourceAssignment). |
| CostVariance | `15` | Représente le champ CostVariance (ResourceAssignment). |
| CV | `16` | Représente le champ CV (ResourceAssignment). |
| Delay | `17` | Représente le champ Delay (ResourceAssignment). |
| Finish | `18` | Représente le champ Finish (ResourceAssignment). |
| FinishVariance | `19` | Représente le champ FinishVariance (ResourceAssignment). |
| Hyperlink | `20` | Représente le champ Hyperlink (ResourceAssignment). |
| HyperlinkAddress | `21` | Représente le champ HyperlinkAddress (ResourceAssignment). |
| HyperlinkSubAddress | `22` | Représente le champ HyperlinkSubAddress (ResourceAssignment). |
| WorkVariance | `23` | Représente le champ WorkVariance (ResourceAssignment). |
| HasFixedRateUnits | `24` | Représente le champ HasFixedRateUnits (ResourceAssignment). |
| FixedMaterial | `25` | Représente le champ FixedMaterial (ResourceAssignment). |
| LevelingDelay | `26` | Représente le champ LevelingDelay (ResourceAssignment). |
| LinkedFields | `27` | Représente le champ LinkedFields (ResourceAssignment). |
| Milestone | `28` | Représente le champ Milestone (ResourceAssignment). |
| Notes | `29` | Représente le champ Notes (ResourceAssignment). |
| NotesText | `30` | Représente le champ NotesText (ResourceAssignment). |
| NotesRTF | `31` | Représente le champ NotesRTF (ResourceAssignment). |
| Overallocated | `32` | Représente le champ Overallocated (ResourceAssignment). |
| OvertimeCost | `33` | Représente le champ OvertimeCost (ResourceAssignment). |
| OvertimeWork | `34` | Représente le champ OvertimeWork (ResourceAssignment). |
| PeakUnits | `35` | Représente le champ PeakUnits (ResourceAssignment). |
| RegularWork | `36` | Représente le champ RegularWork (ResourceAssignment). |
| RemainingCost | `37` | Représente le champ RemainingCost (ResourceAssignment). |
| RemainingOvertimeCost | `38` | Représente le champ RemainingOvertimeCost (ResourceAssignment). |
| RemainingOvertimeWork | `39` | Représente le champ RemainingOvertimeWork (ResourceAssignment). |
| RemainingWork | `40` | Représente le champ RemainingWork (ResourceAssignment). |
| ResponsePending | `41` | Représente le champ ResponsePending (ResourceAssignment). |
| Start | `42` | Représente le champ Start (ResourceAssignment). |
| Stop | `43` | Représente le champ Stop (ResourceAssignment). |
| Resume | `44` | Représente le champ Resume (ResourceAssignment). |
| StartVariance | `45` | Représente le champ StartVariance (ResourceAssignment). |
| Summary | `46` | Représente le champ Summary (ResourceAssignment). |
| SV | `47` | Représente le champ SV (ResourceAssignment). |
| Units | `48` | Représente le champ Units (ResourceAssignment). |
| UpdateNeeded | `49` | Représente le champ UpdateNeeded (ResourceAssignment). |
| VAC | `50` | Représente le champ VAC (ResourceAssignment). |
| Work | `51` | Représente le champ Work (ResourceAssignment). |
| WorkContour | `52` | Représente le champ WorkContour (ResourceAssignment). |
| BCWS | `53` | Représente le champ BCWS (ResourceAssignment). |
| BCWP | `54` | Représente le champ BCWP (ResourceAssignment). |
| BookingType | `55` | Représente le champ BookingType (ResourceAssignment). |
| ActualWorkProtected | `56` | Représente le champ ActualWorkProtected (ResourceAssignment). |
| ActualOvertimeWorkProtected | `57` | Représente le champ ActualOvertimeWorkProtected (ResourceAssignment). |
| Created | `58` | Représente le champ Created (ResourceAssignment). |
| AssignmentOwner | `59` | Représente le champ AssignmentOwner (ResourceAssignment). |
| AssignmentOwnerGuid | `60` | Représente le champ AssignmentOwnerGuid (ResourceAssignment). |
| BudgetWork | `61` | Représente le champ BudgetWork (ResourceAssignment). |
| BudgetCost | `62` | Représente le champ BudgetCost (ResourceAssignment). |
| RateScale | `63` | Représente le champ RateScale (ResourceAssignment). |
| TaskUid | `64` | Représente le champ TaskUid (ResourceAssignment). |
| ResourceUid | `65` | Représente le champ ResourceUid (ResourceAssignment). |

## Exemples

Montre comment lire/écrire les propriétés communes.

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

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


