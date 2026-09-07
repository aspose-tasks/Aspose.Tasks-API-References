---
title: "Enum AsnKey"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.AsnKey. Mewakili daftar bidang penugasan yang didukung"
type: docs
weight: 40
url: /id/net/aspose.tasks/asnkey/
---
## AsnKey enumeration

Mewakili daftar bidang penugasan yang didukung.

```csharp
public enum AsnKey : byte
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| Guid | `0` | Mewakili bidang Guid (ResourceAssignment). |
| Uid | `1` | Mewakili bidang UID (ResourceAssignment). |
| Task | `2` | Mewakili bidang Task (ResourceAssignment). |
| Resource | `3` | Mewakili bidang Resource (ResourceAssignment). |
| PercentWorkComplete | `4` | Mewakili bidang PercentWorkComplete (ResourceAssignment). |
| ActualCost | `5` | Mewakili bidang ActualCost (ResourceAssignment). |
| ActualFinish | `6` | Mewakili bidang ActualFinish (ResourceAssignment). |
| ActualOvertimeCost | `7` | Mewakili bidang ActualOvertimeCost (ResourceAssignment). |
| ActualStart | `8` | Mewakili bidang ActualStart (ResourceAssignment). |
| ActualWork | `9` | Mewakili bidang ActualWork (ResourceAssignment). |
| ActualOvertimeWork | `10` | Mewakili bidang ActualOvertimeWork (ResourceAssignment). |
| ACWP | `11` | Mewakili bidang ACWP (ResourceAssignment). |
| Confirmed | `12` | Mewakili bidang Confirmed (ResourceAssignment). |
| Cost | `13` | Mewakili bidang Cost (ResourceAssignment). |
| CostRateTableType | `14` | Mewakili bidang CostRateTableType (ResourceAssignment). |
| CostVariance | `15` | Mewakili bidang CostVariance (ResourceAssignment). |
| CV | `16` | Mewakili bidang CV (ResourceAssignment). |
| Delay | `17` | Mewakili bidang Delay (ResourceAssignment). |
| Finish | `18` | Mewakili bidang Finish (ResourceAssignment). |
| FinishVariance | `19` | Mewakili bidang FinishVariance (ResourceAssignment). |
| Hyperlink | `20` | Mewakili bidang Hyperlink (ResourceAssignment). |
| HyperlinkAddress | `21` | Mewakili bidang HyperlinkAddress (ResourceAssignment). |
| HyperlinkSubAddress | `22` | Mewakili bidang HyperlinkSubAddress (ResourceAssignment). |
| WorkVariance | `23` | Mewakili bidang WorkVariance (ResourceAssignment). |
| HasFixedRateUnits | `24` | Mewakili bidang HasFixedRateUnits (ResourceAssignment). |
| FixedMaterial | `25` | Mewakili bidang FixedMaterial (ResourceAssignment). |
| LevelingDelay | `26` | Mewakili bidang LevelingDelay (ResourceAssignment). |
| LinkedFields | `27` | Mewakili bidang LinkedFields (ResourceAssignment). |
| Milestone | `28` | Mewakili bidang Milestone (ResourceAssignment). |
| Notes | `29` | Mewakili bidang Notes (ResourceAssignment). |
| NotesText | `30` | Mewakili bidang NotesText (ResourceAssignment). |
| NotesRTF | `31` | Mewakili bidang NotesRTF (ResourceAssignment). |
| Overallocated | `32` | Mewakili bidang Overallocated (ResourceAssignment). |
| OvertimeCost | `33` | Mewakili bidang OvertimeCost (ResourceAssignment). |
| OvertimeWork | `34` | Mewakili bidang OvertimeWork (ResourceAssignment). |
| PeakUnits | `35` | Mewakili bidang PeakUnits (ResourceAssignment). |
| RegularWork | `36` | Mewakili bidang RegularWork (ResourceAssignment). |
| RemainingCost | `37` | Mewakili bidang RemainingCost (ResourceAssignment). |
| RemainingOvertimeCost | `38` | Mewakili bidang RemainingOvertimeCost (ResourceAssignment). |
| RemainingOvertimeWork | `39` | Mewakili bidang RemainingOvertimeWork (ResourceAssignment). |
| RemainingWork | `40` | Mewakili bidang RemainingWork (ResourceAssignment). |
| ResponsePending | `41` | Mewakili bidang ResponsePending (ResourceAssignment). |
| Start | `42` | Mewakili bidang Start (ResourceAssignment). |
| Stop | `43` | Mewakili bidang Stop (ResourceAssignment). |
| Resume | `44` | Mewakili bidang Resume (ResourceAssignment). |
| StartVariance | `45` | Mewakili bidang StartVariance (ResourceAssignment). |
| Summary | `46` | Mewakili bidang Summary (ResourceAssignment). |
| SV | `47` | Mewakili bidang SV (ResourceAssignment). |
| Units | `48` | Mewakili bidang Units (ResourceAssignment). |
| UpdateNeeded | `49` | Mewakili bidang UpdateNeeded (ResourceAssignment). |
| VAC | `50` | Mewakili bidang VAC (ResourceAssignment). |
| Work | `51` | Mewakili bidang Work (ResourceAssignment). |
| WorkContour | `52` | Mewakili bidang WorkContour (ResourceAssignment). |
| BCWS | `53` | Mewakili bidang BCWS (ResourceAssignment). |
| BCWP | `54` | Mewakili bidang BCWP (ResourceAssignment). |
| BookingType | `55` | Mewakili bidang BookingType (ResourceAssignment). |
| ActualWorkProtected | `56` | Mewakili bidang ActualWorkProtected (ResourceAssignment). |
| ActualOvertimeWorkProtected | `57` | Mewakili bidang ActualOvertimeWorkProtected (ResourceAssignment). |
| Created | `58` | Mewakili bidang Created (ResourceAssignment). |
| AssignmentOwner | `59` | Mewakili bidang AssignmentOwner (ResourceAssignment). |
| AssignmentOwnerGuid | `60` | Mewakili bidang AssignmentOwnerGuid (ResourceAssignment). |
| BudgetWork | `61` | Mewakili bidang BudgetWork (ResourceAssignment). |
| BudgetCost | `62` | Mewakili bidang BudgetCost (ResourceAssignment). |
| RateScale | `63` | Mewakili bidang RateScale (ResourceAssignment). |
| TaskUid | `64` | Mewakili bidang TaskUid (ResourceAssignment). |
| ResourceUid | `65` | Mewakili bidang ResourceUid (ResourceAssignment). |

## Contoh

Menampilkan cara membaca/menulis properti umum.

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

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


