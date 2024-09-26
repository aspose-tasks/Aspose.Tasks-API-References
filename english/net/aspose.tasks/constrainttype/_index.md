---
title: Enum ConstraintType
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.ConstraintType enum. Specifies the constraint on the start or finish date of a task
type: docs
weight: 330
url: /net/aspose.tasks/constrainttype/
---
## ConstraintType enumeration

Specifies the constraint on the start or finish date of a task.

```csharp
public enum ConstraintType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Undefined | `-1` | The value was not defined in original project file. |
| AsSoonAsPossible | `0` | [`Start`](../tsk/start/) and [`Finish`](../tsk/finish/) dates of [`Task`](../task/) are scheduled ASAP with respect to parent [`Start`](../tsk/start/) and [`Finish`](../tsk/finish/) dates and considering [`TaskLinks`](../project/tasklinks/). |
| AsLateAsPossible | `1` | [`Start`](../tsk/start/) and [`Finish`](../tsk/finish/) dates of [`Task`](../task/) are scheduled ALAP with respect to parent [`Start`](../tsk/start/) and [`Finish`](../tsk/finish/) dates and considering [`TaskLinks`](../project/tasklinks/). |
| MustStartOn | `2` | Must Start On |
| MustFinishOn | `3` | Must Finish On |
| StartNoEarlierThan | `4` | Start No Earlier Than |
| StartNoLaterThan | `5` | Start No Later Than |
| FinishNoEarlierThan | `6` | Finish No Earlier Than |
| FinishNoLaterThan | `7` | Finish No Later Than |

## Remarks

While exporting into XML the Undefined values will be eliminated from resulting XML.

## Examples

Shows how to set constraint &lt;see cref="Aspose.Tasks.ConstraintType" /&gt; ConstraintType.AsSoonAsPossible constraint for a task.

```csharp
var project = new Project(DataDir + "Constraints/ConstraintAsLateAsPossible.mpp");

// Set constraint As Soon As Possible for task with Id 11
var task = project.RootTask.Children.GetById(11);
task.Set(Tsk.ConstraintType, ConstraintType.AsSoonAsPossible);

SaveOptions options = new PdfSaveOptions();
options.StartDate = project.Get(Prj.StartDate);
options.Timescale = Timescale.ThirdsOfMonths;
project.Save(OutDir + "AsSoonAsPossible_out.pdf", options);
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


