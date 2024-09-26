---
title: Enum AsnKey
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.AsnKey enum. Represents a list of supported assignment fields
type: docs
weight: 40
url: /net/aspose.tasks/asnkey/
---
## AsnKey enumeration

Represents a list of supported assignment fields.

```csharp
public enum AsnKey : byte
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Guid | `0` | Represents the Guid (ResourceAssignment) field. |
| Uid | `1` | Represents the UID (ResourceAssignment) field. |
| Task | `2` | Represents the Task (ResourceAssignment) field. |
| Resource | `3` | Represents the Resource (ResourceAssignment) field. |
| PercentWorkComplete | `4` | Represents the PercentWorkComplete (ResourceAssignment) field. |
| ActualCost | `5` | Represents the ActualCost (ResourceAssignment) field. |
| ActualFinish | `6` | Represents the ActualFinish (ResourceAssignment) field. |
| ActualOvertimeCost | `7` | Represents the ActualOvertimeCost (ResourceAssignment) field. |
| ActualStart | `8` | Represents the ActualStart (ResourceAssignment) field. |
| ActualWork | `9` | Represents the ActualWork (ResourceAssignment) field. |
| ActualOvertimeWork | `10` | Represents the ActualOvertimeWork (ResourceAssignment) field. |
| ACWP | `11` | Represents the ACWP (ResourceAssignment) field. |
| Confirmed | `12` | Represents the Confirmed (ResourceAssignment) field. |
| Cost | `13` | Represents the Cost (ResourceAssignment) field. |
| CostRateTableType | `14` | Represents the CostRateTableType (ResourceAssignment) field. |
| CostVariance | `15` | Represents the CostVariance (ResourceAssignment) field. |
| CV | `16` | Represents the CV (ResourceAssignment) field. |
| Delay | `17` | Represents the Delay (ResourceAssignment) field. |
| Finish | `18` | Represents the Finish (ResourceAssignment) field. |
| FinishVariance | `19` | Represents the FinishVariance (ResourceAssignment) field. |
| Hyperlink | `20` | Represents the Hyperlink (ResourceAssignment) field. |
| HyperlinkAddress | `21` | Represents the HyperlinkAddress (ResourceAssignment) field. |
| HyperlinkSubAddress | `22` | Represents the HyperlinkSubAddress (ResourceAssignment) field. |
| WorkVariance | `23` | Represents the WorkVariance (ResourceAssignment) field. |
| HasFixedRateUnits | `24` | Represents the HasFixedRateUnits (ResourceAssignment) field. |
| FixedMaterial | `25` | Represents the FixedMaterial (ResourceAssignment) field. |
| LevelingDelay | `26` | Represents the LevelingDelay (ResourceAssignment) field. |
| LinkedFields | `27` | Represents the LinkedFields (ResourceAssignment) field. |
| Milestone | `28` | Represents the Milestone (ResourceAssignment) field. |
| Notes | `29` | Represents the Notes (ResourceAssignment) field. |
| NotesText | `30` | Represents the NotesText (ResourceAssignment) field. |
| NotesRTF | `31` | Represents the NotesRTF (ResourceAssignment) field. |
| Overallocated | `32` | Represents the Overallocated (ResourceAssignment) field. |
| OvertimeCost | `33` | Represents the OvertimeCost (ResourceAssignment) field. |
| OvertimeWork | `34` | Represents the OvertimeWork (ResourceAssignment) field. |
| PeakUnits | `35` | Represents the PeakUnits (ResourceAssignment) field. |
| RegularWork | `36` | Represents the RegularWork (ResourceAssignment) field. |
| RemainingCost | `37` | Represents the RemainingCost (ResourceAssignment) field. |
| RemainingOvertimeCost | `38` | Represents the RemainingOvertimeCost (ResourceAssignment) field. |
| RemainingOvertimeWork | `39` | Represents the RemainingOvertimeWork (ResourceAssignment) field. |
| RemainingWork | `40` | Represents the RemainingWork (ResourceAssignment) field. |
| ResponsePending | `41` | Represents the ResponsePending (ResourceAssignment) field. |
| Start | `42` | Represents the Start (ResourceAssignment) field. |
| Stop | `43` | Represents the Stop (ResourceAssignment) field. |
| Resume | `44` | Represents the Resume (ResourceAssignment) field. |
| StartVariance | `45` | Represents the StartVariance (ResourceAssignment) field. |
| Summary | `46` | Represents the Summary (ResourceAssignment) field. |
| SV | `47` | Represents the SV (ResourceAssignment) field. |
| Units | `48` | Represents the Units (ResourceAssignment) field. |
| UpdateNeeded | `49` | Represents the UpdateNeeded (ResourceAssignment) field. |
| VAC | `50` | Represents the VAC (ResourceAssignment) field. |
| Work | `51` | Represents the Work (ResourceAssignment) field. |
| WorkContour | `52` | Represents the WorkContour (ResourceAssignment) field. |
| BCWS | `53` | Represents the BCWS (ResourceAssignment) field. |
| BCWP | `54` | Represents the BCWP (ResourceAssignment) field. |
| BookingType | `55` | Represents the BookingType (ResourceAssignment) field. |
| ActualWorkProtected | `56` | Represents the ActualWorkProtected (ResourceAssignment) field. |
| ActualOvertimeWorkProtected | `57` | Represents the ActualOvertimeWorkProtected (ResourceAssignment) field. |
| Created | `58` | Represents the Created (ResourceAssignment) field. |
| AssignmentOwner | `59` | Represents the AssignmentOwner (ResourceAssignment) field. |
| AssignmentOwnerGuid | `60` | Represents the AssignmentOwnerGuid (ResourceAssignment) field. |
| BudgetWork | `61` | Represents the BudgetWork (ResourceAssignment) field. |
| BudgetCost | `62` | Represents the BudgetCost (ResourceAssignment) field. |
| RateScale | `63` | Represents the RateScale (ResourceAssignment) field. |
| TaskUid | `64` | Represents the TaskUid (ResourceAssignment) field. |
| ResourceUid | `65` | Represents the ResourceUid (ResourceAssignment) field. |

## Examples

Shows how to read/write common properties.

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

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


