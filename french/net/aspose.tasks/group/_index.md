---
title: "Classe Group"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.Group. Représente une définition de groupe. Un objet Group est un membre de la collection ResourceGroups ou de la collection TaskGroups"
type: docs
weight: 770
url: /fr/net/aspose.tasks/group/
---
## Group class

Représente une définition de groupe. Un objet Group est membre de la collection ResourceGroups ou de la collection TaskGroups.

```csharp
public class Group
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [Group](group/)() | Initialise une nouvelle instance de la classe `Group`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [GroupAssignments](../../aspose.tasks/group/groupassignments/) { get; set; } | Obtient ou définit une valeur indiquant si les affectations doivent être regroupées au lieu des tâches. |
| [GroupCriteria](../../aspose.tasks/group/groupcriteria/) { get; set; } | Obtient ou définit une collection GroupCriteria représentant les champs d'une définition de groupe. |
| [MaintainHierarchy](../../aspose.tasks/group/maintainhierarchy/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut afficher tous les niveaux des tâches de résumé pour les sous‑tâches au sein du groupe. |
| [Name](../../aspose.tasks/group/name/) { get; set; } | Obtient ou définit le nom d'un objet Group. |
| [ShowInMenu](../../aspose.tasks/group/showinmenu/) { get; set; } | Obtient ou définit une valeur indiquant si Project affiche le nom du groupe dans la liste déroulante Group du Ruban. |
| [ShowSummary](../../aspose.tasks/group/showsummary/) { get; set; } | Obtient ou définit une valeur indiquant si les lignes de résumé sont affichées pour le groupe. |
| [Uid](../../aspose.tasks/group/uid/) { get; } | Obtient un identifiant unique d'un groupe. |

## Exemples

Montre comment travailler avec les groupes.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

Console.WriteLine("Task Groups Count: " + project.TaskGroups.Count);
var group = project.TaskGroups.ToList()[1];
Console.WriteLine("Task Group Uid: " + group.Uid);
Console.WriteLine("Task Group Name: " + group.Name);
Console.WriteLine("Is Task Group Maintain Hierarchy?: " + group.MaintainHierarchy);
Console.WriteLine("Is Task Group Show In Menu?: " + group.ShowInMenu);
Console.WriteLine("Is Task Group Show Summary?: " + group.ShowSummary);
Console.WriteLine("Is Task Group should groups Assignments instead of Tasks?: " + group.GroupAssignments);
Console.WriteLine("Task Group Criteria count: " + group.GroupCriteria.Count);
Console.WriteLine("\n************* Retrieving Task Group's Criterion information *************");

foreach (var criterion in group.GroupCriteria)
{
    Console.WriteLine("Task Criterion Field: " + criterion.Field);
    Console.WriteLine("Task Criterion GroupOn: " + criterion.GroupOn);
    Console.WriteLine("Task Criterion Cell Color: " + criterion.CellColor);
    Console.WriteLine("Task Criterion Pattern: " + criterion.Pattern);

    Console.WriteLine("Font Name: " + criterion.Font.FontFamily);
    Console.WriteLine("Font Size: " + criterion.Font.Size);
    Console.WriteLine("Font Style: " + criterion.Font.Style);
    Console.WriteLine("Ascending/Descending: " + criterion.Ascending);
}
```

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


