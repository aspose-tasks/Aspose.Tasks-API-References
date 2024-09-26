---
title: SplitPart.GetHashCode
second_title: Aspose.Tasks for .NET API Reference
description: SplitPart method. Returns a hash code value for the instance of the SplitPart class
type: docs
weight: 40
url: /net/aspose.tasks/splitpart/gethashcode/
---
## SplitPart.GetHashCode method

Returns a hash code value for the instance of the [`SplitPart`](../) class.

```csharp
public override int GetHashCode()
```

### Return Value

returns a hash code value for this object.

## Examples

Shows how to get a hash code of a split part.

```csharp
var project = new Project();
project.Set(Prj.StartDate, new DateTime(2000, 3, 15, 8, 0, 0));
project.Set(Prj.FinishDate, new DateTime(2000, 3, 21, 17, 0, 0));

var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.IsManual, false);
task.Set(Tsk.Start, new DateTime(2000, 3, 15, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(3));

var assignment = project.ResourceAssignments.Add(task, project.Resources.Add("r1"));
assignment.Set(Asn.Start, new DateTime(2000, 3, 15, 8, 0, 0));
assignment.Set(Asn.Work, task.Get(Tsk.Work));
assignment.Set(Asn.Finish, new DateTime(2000, 3, 19, 17, 0, 0));

// have to generate resource assignment timephased data first
assignment.TimephasedDataFromTaskDuration(project.Get(Prj.Calendar));

// split the task.
assignment.SplitTask(new DateTime(2000, 3, 16, 8, 0, 0), new DateTime(2000, 3, 17, 17, 0, 0), project.Get(Prj.Calendar));

// the equality of split parts is checked against to start, finish, and index of split parts.
var part1 = task.SplitParts[0];
var part2 = task.SplitParts[1];

// the hash code of a split part based on start, finish, and index of a split part. 
Console.WriteLine("Split Part 1 Start {0} Finish {1} HashCode {2}", part1.Start, part1.Finish, part1.GetHashCode());
Console.WriteLine("Split Part 2 Start {0} Finish {1} HashCode {2}", part2.Start, part2.Finish, part2.GetHashCode());
```

### See Also

* class [SplitPart](../)
* namespace [Aspose.Tasks](../../splitpart/)
* assembly [Aspose.Tasks](../../../)


