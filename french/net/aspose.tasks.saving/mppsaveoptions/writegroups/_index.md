---
title: "MPPSaveOptions.WriteGroups"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété MPPSaveOptions. Obtient ou définit une valeur indiquant s'il faut écrire les données de groupes lors de l'enregistrement d'un projet au format MPP. Les données de groupes incluent les collections Project.TaskGroups et Project.ResourceGroups."
type: docs
weight: 60
url: /fr/net/aspose.tasks.saving/mppsaveoptions/writegroups/
---
## MPPSaveOptions.WriteGroups property

Obtient ou définit une valeur indiquant s'il faut écrire les données de groupes lors de l'enregistrement d'un projet au format MPP. Les données de groupe comprennent les collections Project.TaskGroups et Project.ResourceGroups.

```csharp
public bool WriteGroups { get; set; }
```

## Exemples

Montre comment ajouter des groupes à un projet.

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

### Voir aussi

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


