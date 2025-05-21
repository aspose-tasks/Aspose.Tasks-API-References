---
title: Project.TaskGroups
second_title: Aspose.Tasks for .NET API Reference
description: Project property. Gets all the taskbased group definitions. TaskGroups is a collection of Group objects
type: docs
weight: 910
url: /net/aspose.tasks/project/taskgroups/
---
## Project.TaskGroups property

Gets all the task-based group definitions. TaskGroups is a collection of [`Group`](../../group/) objects.

```csharp
public GroupCollection TaskGroups { get; }
```

## Examples

Shows how to read task groups.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

Console.WriteLine("Task Groups Count: " + project.TaskGroups.Count);
var taskGroup = project.TaskGroups.ToList()[1];
Console.WriteLine("Task Group Name: " + taskGroup.Name);
Console.WriteLine("Task Group Criteria count: " + taskGroup.GroupCriteria.Count);
Console.WriteLine("\n************* Retrieving Task Group's Criterion information *************");
var taskCriterion = taskGroup.GroupCriteria.ToList()[0];
Console.WriteLine("Task Criterion Field: " + taskCriterion.Field);
Console.WriteLine("Task Criterion GroupOn: " + taskCriterion.GroupOn);
Console.WriteLine("Task Criterion Cell Color: " + taskCriterion.CellColor);
Console.WriteLine("Task Criterion Pattern: " + taskCriterion.Pattern);

Console.WriteLine("\n*********** Retrieving Criterion's Font Information ***********");
Console.WriteLine("Font Name: " + taskCriterion.Font.FontFamily);
Console.WriteLine("Font Size: " + taskCriterion.Font.Size);
Console.WriteLine("Font Style: " + taskCriterion.Font.Style);
Console.WriteLine("Ascending/Descending: " + taskCriterion.Ascending);
```

Shows how to add groups to a project.

```csharp
var p = new Project();

{
    var group = new Group();
    group.Name = "My new task group";
    group.MaintainHierarchy = true;
    group.ShowSummary = true;

    var criterion = new GroupCriterion();
    criterion.Field = Field.TaskDuration1;
    criterion.Font = new FontDescriptor("Comic Sans MS", 13F, FontStyles.Italic);
    criterion.GroupOn = GroupOn.DurationMinutes;
    criterion.StartAt = 5;
    criterion.GroupInterval = 3D;
    criterion.Pattern = BackgroundPattern.DarkDiagonalLeft;
    group.GroupCriteria.Add(criterion);

    var criterion2 = new GroupCriterion();
    criterion2.Field = Field.TaskPercentComplete;
    criterion2.Font = new FontDescriptor("Bodoni MT", 17, FontStyles.Italic | FontStyles.Bold);
    criterion2.GroupOn = GroupOn.Pct199;
    criterion2.Pattern = BackgroundPattern.LightDither;
    criterion2.CellColor = Color.Green;
    criterion2.FontColor = Color.Red;
    group.GroupCriteria.Add(criterion2);
    group.GroupAssignments = true;
    p.TaskGroups.Add(group);
}

{
    var group = new Group();
    group.Name = "My new resource group";
    group.MaintainHierarchy = true;
    group.ShowSummary = true;

    var criterion = new GroupCriterion();
    criterion.Field = Field.ResourceDuration1;
    criterion.Font = new FontDescriptor("Comic Sans MS", 11F, FontStyles.Bold);
    criterion.GroupOn = GroupOn.DurationHours;
    criterion.StartAt = 1;
    criterion.GroupInterval = 2D;
    criterion.Pattern = BackgroundPattern.DarkDiagonalLeft;
    group.GroupCriteria.Add(criterion);

    var criterion2 = new GroupCriterion();
    criterion2.Field = Field.ResourceCost;
    criterion2.Font = new FontDescriptor("Bodoni MT", 12, FontStyles.Italic | FontStyles.Bold);
    criterion2.GroupOn = GroupOn.Interval;
    criterion2.StartAt = 1D;
    criterion2.GroupInterval = 10D;
    criterion2.Pattern = BackgroundPattern.LightDither;
    criterion2.CellColor = Color.Magenta;
    criterion2.FontColor = Color.Red;
    group.GroupCriteria.Add(criterion2);
    group.GroupAssignments = true;
    p.ResourceGroups.Add(group);
}

p.Save(OutDir + "output_CreateGroup.mpp", new MPPSaveOptions() { WriteGroups = true });
```

### See Also

* class [GroupCollection](../../groupcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


