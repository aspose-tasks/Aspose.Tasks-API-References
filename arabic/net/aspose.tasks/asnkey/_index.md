---
title: "تعداد AsnKey"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Aspose.Tasks.AsnKey enum. يمثل قائمة بالحقول المدعومة للتعيين"
type: docs
weight: 40
url: /ar/net/aspose.tasks/asnkey/
---
## AsnKey enumeration

يمثل قائمة بالحقول المعينة المدعومة.

```csharp
public enum AsnKey : byte
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Guid | `0` | يمثل حقل Guid (ResourceAssignment). |
| Uid | `1` | يمثل حقل UID (ResourceAssignment). |
| Task | `2` | يمثل حقل Task (ResourceAssignment). |
| Resource | `3` | يمثل حقل Resource (ResourceAssignment). |
| PercentWorkComplete | `4` | يمثل حقل PercentWorkComplete (ResourceAssignment). |
| ActualCost | `5` | يمثل حقل ActualCost (ResourceAssignment). |
| ActualFinish | `6` | يمثل حقل ActualFinish (ResourceAssignment). |
| ActualOvertimeCost | `7` | يمثل حقل ActualOvertimeCost (ResourceAssignment). |
| ActualStart | `8` | يمثل حقل ActualStart (ResourceAssignment). |
| ActualWork | `9` | يمثل حقل ActualWork (ResourceAssignment). |
| ActualOvertimeWork | `10` | يمثل حقل ActualOvertimeWork (ResourceAssignment). |
| ACWP | `11` | يمثل حقل ACWP (ResourceAssignment). |
| Confirmed | `12` | يمثل حقل Confirmed (ResourceAssignment). |
| Cost | `13` | يمثل حقل Cost (ResourceAssignment). |
| CostRateTableType | `14` | يمثل حقل CostRateTableType (ResourceAssignment). |
| CostVariance | `15` | يمثل حقل CostVariance (ResourceAssignment). |
| CV | `16` | يمثل حقل CV (ResourceAssignment). |
| Delay | `17` | يمثل حقل Delay (ResourceAssignment). |
| Finish | `18` | يمثل حقل Finish (ResourceAssignment). |
| FinishVariance | `19` | يمثل حقل FinishVariance (ResourceAssignment). |
| Hyperlink | `20` | يمثل حقل Hyperlink (ResourceAssignment). |
| HyperlinkAddress | `21` | يمثل حقل HyperlinkAddress (ResourceAssignment). |
| HyperlinkSubAddress | `22` | يمثل الحقل HyperlinkSubAddress (ResourceAssignment). |
| WorkVariance | `23` | يمثل الحقل WorkVariance (ResourceAssignment). |
| HasFixedRateUnits | `24` | يمثل الحقل HasFixedRateUnits (ResourceAssignment). |
| FixedMaterial | `25` | يمثل الحقل FixedMaterial (ResourceAssignment). |
| LevelingDelay | `26` | يمثل الحقل LevelingDelay (ResourceAssignment). |
| LinkedFields | `27` | يمثل الحقل LinkedFields (ResourceAssignment). |
| Milestone | `28` | يمثل الحقل Milestone (ResourceAssignment). |
| Notes | `29` | يمثل الحقل Notes (ResourceAssignment). |
| NotesText | `30` | يمثل الحقل NotesText (ResourceAssignment). |
| NotesRTF | `31` | يمثل الحقل NotesRTF (ResourceAssignment). |
| Overallocated | `32` | يمثل الحقل Overallocated (ResourceAssignment). |
| OvertimeCost | `33` | يمثل الحقل OvertimeCost (ResourceAssignment). |
| OvertimeWork | `34` | يمثل الحقل OvertimeWork (ResourceAssignment). |
| PeakUnits | `35` | يمثل الحقل PeakUnits (ResourceAssignment). |
| RegularWork | `36` | يمثل الحقل RegularWork (ResourceAssignment). |
| RemainingCost | `37` | يمثل الحقل RemainingCost (ResourceAssignment). |
| RemainingOvertimeCost | `38` | يمثل الحقل RemainingOvertimeCost (ResourceAssignment). |
| RemainingOvertimeWork | `39` | يمثل الحقل RemainingOvertimeWork (ResourceAssignment). |
| RemainingWork | `40` | يمثل الحقل RemainingWork (ResourceAssignment). |
| ResponsePending | `41` | يمثل الحقل ResponsePending (ResourceAssignment). |
| Start | `42` | يمثل الحقل Start (ResourceAssignment). |
| Stop | `43` | يمثل الحقل Stop (ResourceAssignment). |
| Resume | `44` | يمثل الحقل Resume (ResourceAssignment). |
| StartVariance | `45` | يمثل الحقل StartVariance (ResourceAssignment). |
| Summary | `46` | يمثل الحقل Summary (ResourceAssignment). |
| SV | `47` | يمثل حقل SV (ResourceAssignment). |
| Units | `48` | يمثل حقل Units (ResourceAssignment). |
| UpdateNeeded | `49` | يمثل حقل UpdateNeeded (ResourceAssignment). |
| VAC | `50` | يمثل حقل VAC (ResourceAssignment). |
| Work | `51` | يمثل حقل Work (ResourceAssignment). |
| WorkContour | `52` | يمثل حقل WorkContour (ResourceAssignment). |
| BCWS | `53` | يمثل حقل BCWS (ResourceAssignment). |
| BCWP | `54` | يمثل حقل BCWP (ResourceAssignment). |
| BookingType | `55` | يمثل حقل BookingType (ResourceAssignment). |
| ActualWorkProtected | `56` | يمثل حقل ActualWorkProtected (ResourceAssignment). |
| ActualOvertimeWorkProtected | `57` | يمثل حقل ActualOvertimeWorkProtected (ResourceAssignment). |
| Created | `58` | يمثل حقل Created (ResourceAssignment). |
| AssignmentOwner | `59` | يمثل حقل AssignmentOwner (ResourceAssignment). |
| AssignmentOwnerGuid | `60` | يمثل حقل AssignmentOwnerGuid (ResourceAssignment). |
| BudgetWork | `61` | يمثل حقل BudgetWork (ResourceAssignment). |
| BudgetCost | `62` | يمثل حقل BudgetCost (ResourceAssignment). |
| RateScale | `63` | يمثل حقل RateScale (ResourceAssignment). |
| TaskUid | `64` | يمثل حقل TaskUid (ResourceAssignment). |
| ResourceUid | `65` | يمثل حقل ResourceUid (ResourceAssignment). |

## الأمثلة

يعرض كيفية قراءة/كتابة الخصائص العامة.

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

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


