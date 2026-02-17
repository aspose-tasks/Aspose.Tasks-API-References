---
title: Project.ResourceGroups
second_title: Aspose.Tasks for .NET API Reference
description: Project property. Gets all of the resourcebased group definitions. ResourceGroups is a collection of Group objects
type: docs
weight: 770
url: /net/aspose.tasks/project/resourcegroups/
---
## Project.ResourceGroups property

Gets all of the resource-based group definitions. ResourceGroups is a collection of [`Group`](../../group/) objects.

```csharp
public GroupCollection ResourceGroups { get; }
```

## Examples

Shows how to read resource groups.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

Console.WriteLine("Resource Groups Count: " + project.ResourceGroups.Count);
var resGroup = project.TaskGroups.ToList()[1];
Console.WriteLine("Resource Group Name: " + resGroup.Name);
Console.WriteLine("Resource Group Criteria count: " + resGroup.GroupCriteria.Count);
Console.WriteLine("\n************* Retrieving Resource Group's Criterion information *************");
var resCriterion = resGroup.GroupCriteria.ToList()[0];
Console.WriteLine("Resource Criterion Field: " + resCriterion.Field);
Console.WriteLine("Resource Criterion GroupOn: " + resCriterion.GroupOn);
Console.WriteLine("Resource Criterion Cell Color: " + resCriterion.CellColor);
Console.WriteLine("Resource Criterion Pattern: " + resCriterion.Pattern);

Console.WriteLine("\n*********** Retrieving Resource Criterion's Font Information ***********");
Console.WriteLine("Resource Font Name: " + resCriterion.Font.FontFamily);
Console.WriteLine("Resource Font Size: " + resCriterion.Font.Size);
Console.WriteLine("Resource Font Style: " + resCriterion.Font.Style);
Console.WriteLine("Resource Ascending/Descending: " + resCriterion.Ascending);
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


