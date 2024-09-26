---
title: SplitPart.Equals
second_title: Aspose.Tasks for .NET API Reference
description: SplitPart method. Compares two split parts
type: docs
weight: 30
url: /net/aspose.tasks/splitpart/equals/
---
## SplitPart.Equals method

Compares two split parts.

```csharp
public override bool Equals(object obj)
```

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | Object to compare. |

### Return Value

True if the specified object is equal to the current object; otherwise, false.

## Examples

Shows how to check split parts equality.

```csharp
var project = new Project();
project.Set(Prj.StartDate, new DateTime(2000, 3, 15, 8, 0, 0));
project.Set(Prj.FinishDate, new DateTime(2000, 3, 21, 17, 0, 0));

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.IsManual, false);
task.Set(Tsk.Start, new DateTime(2000, 3, 15, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(4));

var assignment = project.ResourceAssignments.Add(task, project.Resources.Add("Resource"));
assignment.Set(Asn.Start, new DateTime(2000, 3, 15, 8, 0, 0));
assignment.Set(Asn.Work, task.Get(Tsk.Work));
assignment.Set(Asn.Finish, new DateTime(2000, 3, 19, 17, 0, 0));

// have to generate resource assignment timephased data first
assignment.TimephasedDataFromTaskDuration(project.Get(Prj.Calendar));
Console.WriteLine(assignment.Get(Asn.Finish));

// split the task.
assignment.SplitTask(new DateTime(2000, 3, 16, 8, 0, 0), new DateTime(2000, 3, 17, 17, 0, 0), project.Get(Prj.Calendar));

// the equality of split parts is checked against to start, finish, and index of split parts.
var part1 = task.SplitParts[0];
var part2 = task.SplitParts[1];
Console.WriteLine("Split Part 1 Start {0} Finish {1}", part1.Start, part1.Finish);
Console.WriteLine("Split Part 2 Start {0} Finish {1}", part2.Start, part2.Finish);
Console.WriteLine("Are split parts equal: " + part1.Equals(part2));
```

### See Also

* class [SplitPart](../)
* namespace [Aspose.Tasks](../../splitpart/)
* assembly [Aspose.Tasks](../../../)


