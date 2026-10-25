---
title: "Enumeración AsnKey"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enumeración Aspose.Tasks.AsnKey. Representa una lista de campos de asignación compatibles"
type: docs
weight: 40
url: /es/net/aspose.tasks/asnkey/
---
## AsnKey enumeration

Representa una lista de campos de asignación compatibles.

```csharp
public enum AsnKey : byte
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Guid | `0` | Representa el campo Guid (ResourceAssignment). |
| Uid | `1` | Representa el campo UID (ResourceAssignment). |
| Task | `2` | Representa el campo Task (ResourceAssignment). |
| Resource | `3` | Representa el campo Resource (ResourceAssignment). |
| PercentWorkComplete | `4` | Representa el campo PercentWorkComplete (ResourceAssignment). |
| ActualCost | `5` | Representa el campo ActualCost (ResourceAssignment). |
| ActualFinish | `6` | Representa el campo ActualFinish (ResourceAssignment). |
| ActualOvertimeCost | `7` | Representa el campo ActualOvertimeCost (ResourceAssignment). |
| ActualStart | `8` | Representa el campo ActualStart (ResourceAssignment). |
| ActualWork | `9` | Representa el campo ActualWork (ResourceAssignment). |
| ActualOvertimeWork | `10` | Representa el campo ActualOvertimeWork (ResourceAssignment). |
| ACWP | `11` | Representa el campo ACWP (ResourceAssignment). |
| Confirmed | `12` | Representa el campo Confirmed (ResourceAssignment). |
| Cost | `13` | Representa el campo Cost (ResourceAssignment). |
| CostRateTableType | `14` | Representa el campo CostRateTableType (ResourceAssignment). |
| CostVariance | `15` | Representa el campo CostVariance (ResourceAssignment). |
| CV | `16` | Representa el campo CV (ResourceAssignment). |
| Delay | `17` | Representa el campo Delay (ResourceAssignment). |
| Finish | `18` | Representa el campo Finish (ResourceAssignment). |
| FinishVariance | `19` | Representa el campo FinishVariance (ResourceAssignment). |
| Hyperlink | `20` | Representa el campo Hyperlink (ResourceAssignment). |
| HyperlinkAddress | `21` | Representa el campo HyperlinkAddress (ResourceAssignment). |
| HyperlinkSubAddress | `22` | Representa el HyperlinkSubAddress (ResourceAssignment) campo. |
| WorkVariance | `23` | Representa el WorkVariance (ResourceAssignment) campo. |
| HasFixedRateUnits | `24` | Representa el HasFixedRateUnits (ResourceAssignment) campo. |
| FixedMaterial | `25` | Representa el FixedMaterial (ResourceAssignment) campo. |
| LevelingDelay | `26` | Representa el LevelingDelay (ResourceAssignment) campo. |
| LinkedFields | `27` | Representa el LinkedFields (ResourceAssignment) campo. |
| Milestone | `28` | Representa el Milestone (ResourceAssignment) campo. |
| Notes | `29` | Representa el Notes (ResourceAssignment) campo. |
| NotesText | `30` | Representa el NotesText (ResourceAssignment) campo. |
| NotesRTF | `31` | Representa el NotesRTF (ResourceAssignment) campo. |
| Overallocated | `32` | Representa el Overallocated (ResourceAssignment) campo. |
| OvertimeCost | `33` | Representa el OvertimeCost (ResourceAssignment) campo. |
| OvertimeWork | `34` | Representa el OvertimeWork (ResourceAssignment) campo. |
| PeakUnits | `35` | Representa el PeakUnits (ResourceAssignment) campo. |
| RegularWork | `36` | Representa el RegularWork (ResourceAssignment) campo. |
| RemainingCost | `37` | Representa el RemainingCost (ResourceAssignment) campo. |
| RemainingOvertimeCost | `38` | Representa el RemainingOvertimeCost (ResourceAssignment) campo. |
| RemainingOvertimeWork | `39` | Representa el RemainingOvertimeWork (ResourceAssignment) campo. |
| RemainingWork | `40` | Representa el RemainingWork (ResourceAssignment) campo. |
| ResponsePending | `41` | Representa el ResponsePending (ResourceAssignment) campo. |
| Start | `42` | Representa el Start (ResourceAssignment) campo. |
| Stop | `43` | Representa el Stop (ResourceAssignment) campo. |
| Resume | `44` | Representa el Resume (ResourceAssignment) campo. |
| StartVariance | `45` | Representa el StartVariance (ResourceAssignment) campo. |
| Summary | `46` | Representa el Summary (ResourceAssignment) campo. |
| SV | `47` | Representa el campo SV (ResourceAssignment). |
| Units | `48` | Representa el campo Units (ResourceAssignment). |
| UpdateNeeded | `49` | Representa el campo UpdateNeeded (ResourceAssignment). |
| VAC | `50` | Representa el campo VAC (ResourceAssignment). |
| Work | `51` | Representa el campo Work (ResourceAssignment). |
| WorkContour | `52` | Representa el campo WorkContour (ResourceAssignment). |
| BCWS | `53` | Representa el campo BCWS (ResourceAssignment). |
| BCWP | `54` | Representa el campo BCWP (ResourceAssignment). |
| BookingType | `55` | Representa el campo BookingType (ResourceAssignment). |
| ActualWorkProtected | `56` | Representa el campo ActualWorkProtected (ResourceAssignment). |
| ActualOvertimeWorkProtected | `57` | Representa el campo ActualOvertimeWorkProtected (ResourceAssignment). |
| Created | `58` | Representa el campo Created (ResourceAssignment). |
| AssignmentOwner | `59` | Representa el campo AssignmentOwner (ResourceAssignment). |
| AssignmentOwnerGuid | `60` | Representa el campo AssignmentOwnerGuid (ResourceAssignment). |
| BudgetWork | `61` | Representa el campo BudgetWork (ResourceAssignment). |
| BudgetCost | `62` | Representa el campo BudgetCost (ResourceAssignment). |
| RateScale | `63` | Representa el campo RateScale (ResourceAssignment). |
| TaskUid | `64` | Representa el campo TaskUid (ResourceAssignment). |
| ResourceUid | `65` | Representa el campo ResourceUid (ResourceAssignment). |

## Ejemplos

Muestra cómo leer/escribir propiedades comunes.

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

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


