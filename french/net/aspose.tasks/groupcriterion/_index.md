---
title: "Classe GroupCriterion"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.GroupCriterion class. Représente un critère dans une définition de groupe. L'objet GroupCriterion est un membre de la collection GroupCriterionCollection."
type: docs
weight: 790
url: /fr/net/aspose.tasks/groupcriterion/
---
## GroupCriterion class

Représente un critère dans une définition de groupe. L'objet GroupCriterion est un membre de la collection [`GroupCriterionCollection`](../groupcriterioncollection/).

```csharp
public class GroupCriterion
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [GroupCriterion](groupcriterion/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Ascending](../../aspose.tasks/groupcriterion/ascending/) { get; set; } | Obtient ou définit une valeur indiquant si un champ utilisé comme critère dans une définition de groupe est trié par ordre croissant. Faux si le champ est trié par ordre décroissant. |
| [CellColor](../../aspose.tasks/groupcriterion/cellcolor/) { get; set; } | Obtient ou définit la couleur d'arrière-plan de la cellule pour un champ utilisé comme critère dans une définition de groupe. |
| [Field](../../aspose.tasks/groupcriterion/field/) { get; set; } | Obtient ou définit le champ utilisé pour le regroupement. |
| [Font](../../aspose.tasks/groupcriterion/font/) { get; set; } | Obtient ou définit la police pour un critère dans une définition de groupe. |
| [FontColor](../../aspose.tasks/groupcriterion/fontcolor/) { get; set; } | Obtient ou définit la couleur de la police pour un champ utilisé comme critère dans une définition de groupe. |
| [GroupInterval](../../aspose.tasks/groupcriterion/groupinterval/) { get; set; } | Obtient ou définit l'intervalle pour un champ utilisé comme critère dans une définition de groupe. |
| [GroupOn](../../aspose.tasks/groupcriterion/groupon/) { get; set; } | Obtient ou définit le type de regroupement pour un champ utilisé comme critère dans une définition de groupe. |
| [Pattern](../../aspose.tasks/groupcriterion/pattern/) { get; set; } | Obtient ou définit le modèle de la cellule pour un champ utilisé comme critère dans une définition de groupe. |
| [StartAt](../../aspose.tasks/groupcriterion/startat/) { get; set; } | Obtient ou définit le début des intervalles pour un champ utilisé comme critère dans une définition de groupe. |

## Méthodes

| Nom | Description |
| --- | --- |
| override [Equals](../../aspose.tasks/groupcriterion/equals/)(object) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| override [GetHashCode](../../aspose.tasks/groupcriterion/gethashcode/)() | Servit de fonction de hachage pour un type particulier. |

## Exemples

Montre comment lire les propriétés d'un critère de groupe.

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

// lire le motif de fond du critère  
Console.WriteLine("Task Criterion Pattern: " + criterion.Pattern);

Console.WriteLine("\n*********** Retrieving Criterion's Font Information ***********");
Console.WriteLine("Font Name: " + criterion.Font.FontFamily);
Console.WriteLine("Font Size: " + criterion.Font.Size);
Console.WriteLine("Font Style: " + criterion.Font.Style);
Console.WriteLine("Ascending/Descending: " + criterion.Ascending);
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


