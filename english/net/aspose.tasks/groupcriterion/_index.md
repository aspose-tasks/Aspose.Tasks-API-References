---
title: Class GroupCriterion
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.GroupCriterion class. Represents a criterion in a group definition. The GroupCriterion object is a member of the GroupCriterionCollection collection
type: docs
weight: 790
url: /net/aspose.tasks/groupcriterion/
---
## GroupCriterion class

Represents a criterion in a group definition. The GroupCriterion object is a member of the [`GroupCriterionCollection`](../groupcriterioncollection/) collection.

```csharp
public class GroupCriterion
```

## Constructors

| Name | Description |
| --- | --- |
| [GroupCriterion](groupcriterion/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [Ascending](../../aspose.tasks/groupcriterion/ascending/) { get; set; } | Gets or sets a value indicating whether a field used as a criterion in a group definition is sorted in ascending order. False if the field is sorted in descending order. |
| [CellColor](../../aspose.tasks/groupcriterion/cellcolor/) { get; set; } | Gets or sets the color of the cell background for a field used as a criterion in a group definition. |
| [Field](../../aspose.tasks/groupcriterion/field/) { get; set; } | Gets or sets the field being grouped by. |
| [Font](../../aspose.tasks/groupcriterion/font/) { get; set; } | Gets or sets the font for a criterion in a group definition. |
| [FontColor](../../aspose.tasks/groupcriterion/fontcolor/) { get; set; } | Gets or sets the color of the font for a field used as a criterion in a group definition. |
| [GroupInterval](../../aspose.tasks/groupcriterion/groupinterval/) { get; set; } | Gets or sets the interval for a field used as a criterion in a group definition. |
| [GroupOn](../../aspose.tasks/groupcriterion/groupon/) { get; set; } | Gets or sets the type of grouping for a field used as a criterion in a group definition. |
| [Pattern](../../aspose.tasks/groupcriterion/pattern/) { get; set; } | Gets or sets the pattern of the cell for a field used as a criterion in a group definition. |
| [StartAt](../../aspose.tasks/groupcriterion/startat/) { get; set; } | Gets or sets the start of the intervals for a field used as a criterion in a group definition. |

## Methods

| Name | Description |
| --- | --- |
| override [Equals](../../aspose.tasks/groupcriterion/equals/)(object) | Returns a value indicating whether this instance is equal to a specified object. |
| override [GetHashCode](../../aspose.tasks/groupcriterion/gethashcode/)() | Serves as a hash function for a particular type. |

## Examples

Shows how to read properties of a group criterion.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

Console.WriteLine("Task Groups Count: " + project.TaskGroups.Count);
var group = project.TaskGroups.ToList()[1];
Console.WriteLine("Task Group Name: " + group.Name);
Console.WriteLine("Task Group Criteria count: " + group.GroupCriteria.Count);

Console.WriteLine("\n************* Retrieving Task Group's Criterion information *************");
var criterion = group.GroupCriteria.ToList()[0];
Console.WriteLine("Task Criterion Field: " + criterion.Field);
Console.WriteLine("Task Criterion GroupOn: " + criterion.GroupOn);
Console.WriteLine("Task Criterion Cell Color: " + criterion.CellColor);
Console.WriteLine("Task Criterion Font Color: " + criterion.FontColor);
Console.WriteLine("Task Criterion Group Interval: " + criterion.GroupInterval);
Console.WriteLine("Task Criterion Start At: " + criterion.StartAt);

// read the background pattern of the criterion  
Console.WriteLine("Task Criterion Pattern: " + criterion.Pattern);

Console.WriteLine("\n*********** Retrieving Criterion's Font Information ***********");
Console.WriteLine("Font Name: " + criterion.Font.FontFamily);
Console.WriteLine("Font Size: " + criterion.Font.Size);
Console.WriteLine("Font Style: " + criterion.Font.Style);
Console.WriteLine("Ascending/Descending: " + criterion.Ascending);
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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


