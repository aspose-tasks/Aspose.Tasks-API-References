---
title: "Перечисление AsnKey"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.AsnKey. Представляет список поддерживаемых полей назначения"
type: docs
weight: 40
url: /ru/net/aspose.tasks/asnkey/
---
## AsnKey enumeration

Представляет список поддерживаемых полей назначения.

```csharp
public enum AsnKey : byte
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Guid | `0` | Представляет поле Guid (ResourceAssignment). |
| Uid | `1` | Представляет поле UID (ResourceAssignment). |
| Task | `2` | Представляет поле Task (ResourceAssignment). |
| Resource | `3` | Представляет поле Resource (ResourceAssignment). |
| PercentWorkComplete | `4` | Представляет поле PercentWorkComplete (ResourceAssignment). |
| ActualCost | `5` | Представляет поле ActualCost (ResourceAssignment). |
| ActualFinish | `6` | Представляет поле ActualFinish (ResourceAssignment). |
| ActualOvertimeCost | `7` | Представляет поле ActualOvertimeCost (ResourceAssignment). |
| ActualStart | `8` | Представляет поле ActualStart (ResourceAssignment). |
| ActualWork | `9` | Представляет поле ActualWork (ResourceAssignment). |
| ActualOvertimeWork | `10` | Представляет поле ActualOvertimeWork (ResourceAssignment). |
| ACWP | `11` | Представляет поле ACWP (ResourceAssignment). |
| Confirmed | `12` | Представляет поле Confirmed (ResourceAssignment). |
| Cost | `13` | Представляет поле Cost (ResourceAssignment). |
| CostRateTableType | `14` | Представляет поле CostRateTableType (ResourceAssignment). |
| CostVariance | `15` | Представляет поле CostVariance (ResourceAssignment). |
| CV | `16` | Представляет поле CV (ResourceAssignment). |
| Delay | `17` | Представляет поле Delay (ResourceAssignment). |
| Finish | `18` | Представляет поле Finish (ResourceAssignment). |
| FinishVariance | `19` | Представляет поле FinishVariance (ResourceAssignment). |
| Hyperlink | `20` | Представляет поле Hyperlink (ResourceAssignment). |
| HyperlinkAddress | `21` | Представляет поле HyperlinkAddress (ResourceAssignment). |
| HyperlinkSubAddress | `22` | Представляет поле HyperlinkSubAddress (ResourceAssignment). |
| WorkVariance | `23` | Представляет поле WorkVariance (ResourceAssignment). |
| HasFixedRateUnits | `24` | Представляет поле HasFixedRateUnits (ResourceAssignment). |
| FixedMaterial | `25` | Представляет поле FixedMaterial (ResourceAssignment). |
| LevelingDelay | `26` | Представляет поле LevelingDelay (ResourceAssignment). |
| LinkedFields | `27` | Представляет поле LinkedFields (ResourceAssignment). |
| Milestone | `28` | Представляет поле Milestone (ResourceAssignment). |
| Notes | `29` | Представляет поле Notes (ResourceAssignment). |
| NotesText | `30` | Представляет поле NotesText (ResourceAssignment). |
| NotesRTF | `31` | Представляет поле NotesRTF (ResourceAssignment). |
| Overallocated | `32` | Представляет поле Overallocated (ResourceAssignment). |
| OvertimeCost | `33` | Представляет поле OvertimeCost (ResourceAssignment). |
| OvertimeWork | `34` | Представляет поле OvertimeWork (ResourceAssignment). |
| PeakUnits | `35` | Представляет поле PeakUnits (ResourceAssignment). |
| RegularWork | `36` | Представляет поле RegularWork (ResourceAssignment). |
| RemainingCost | `37` | Представляет поле RemainingCost (ResourceAssignment). |
| RemainingOvertimeCost | `38` | Представляет поле RemainingOvertimeCost (ResourceAssignment). |
| RemainingOvertimeWork | `39` | Представляет поле RemainingOvertimeWork (ResourceAssignment). |
| RemainingWork | `40` | Представляет поле RemainingWork (ResourceAssignment). |
| ResponsePending | `41` | Представляет поле ResponsePending (ResourceAssignment). |
| Start | `42` | Представляет поле Start (ResourceAssignment). |
| Stop | `43` | Представляет поле Stop (ResourceAssignment). |
| Resume | `44` | Представляет поле Resume (ResourceAssignment). |
| StartVariance | `45` | Представляет поле StartVariance (ResourceAssignment). |
| Summary | `46` | Представляет поле Summary (ResourceAssignment). |
| SV | `47` | Представляет поле SV (ResourceAssignment). |
| Units | `48` | Представляет поле Units (ResourceAssignment). |
| UpdateNeeded | `49` | Представляет поле UpdateNeeded (ResourceAssignment). |
| VAC | `50` | Представляет поле VAC (ResourceAssignment). |
| Work | `51` | Представляет поле Work (ResourceAssignment). |
| WorkContour | `52` | Представляет поле WorkContour (ResourceAssignment). |
| BCWS | `53` | Представляет поле BCWS (ResourceAssignment). |
| BCWP | `54` | Представляет поле BCWP (ResourceAssignment). |
| BookingType | `55` | Представляет поле BookingType (ResourceAssignment). |
| ActualWorkProtected | `56` | Представляет поле ActualWorkProtected (ResourceAssignment). |
| ActualOvertimeWorkProtected | `57` | Представляет поле ActualOvertimeWorkProtected (ResourceAssignment). |
| Created | `58` | Представляет поле Created (ResourceAssignment). |
| AssignmentOwner | `59` | Представляет поле AssignmentOwner (ResourceAssignment). |
| AssignmentOwnerGuid | `60` | Представляет поле AssignmentOwnerGuid (ResourceAssignment). |
| BudgetWork | `61` | Представляет поле BudgetWork (ResourceAssignment). |
| BudgetCost | `62` | Представляет поле BudgetCost (ResourceAssignment). |
| RateScale | `63` | Представляет поле RateScale (ResourceAssignment). |
| TaskUid | `64` | Представляет поле TaskUid (ResourceAssignment). |
| ResourceUid | `65` | Представляет поле ResourceUid (ResourceAssignment). |

## Примеры

Показывает, как читать/записывать общие свойства.

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

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


