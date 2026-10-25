---
title: "Classe TaskUsageView"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.TaskUsageView. Représente la vue d'utilisation des tâches dans un projet"
type: docs
weight: 2480
url: /fr/net/aspose.tasks/taskusageview/
---
## TaskUsageView class

Représente la vue d'utilisation des tâches dans un projet.

```csharp
public class TaskUsageView : UsageView
```

## Propriétés

| Nom | Description |
| --- | --- |
| [AlignDetailsData](../../aspose.tasks/usageview/aligndetailsdata/) { get; set; } | Obtient ou définit l'alignement des données détaillées. |
| [BottomTimescaleTier](../../aspose.tasks/usageview/bottomtimescaletier/) { get; set; } | Obtient ou définit les paramètres du niveau inférieur de l'échelle de temps de la vue. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/) |
| [DisplayDetailsHeaderColumn](../../aspose.tasks/usageview/displaydetailsheadercolumn/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut afficher ou non la colonne d'en-tête des détails dans la vue. |
| [DisplayShortDetailHeaderNames](../../aspose.tasks/usageview/displayshortdetailheadernames/) { get; set; } | Obtient ou définit une valeur indiquant s’il faut afficher les noms d’en-tête de détail courts ou non. |
| [FieldCollection](../../aspose.tasks/taskusageview/fieldcollection/) { get; } | Obtient l'objet [`TaskUsageViewFieldCollection`](../taskusageviewfieldcollection/) de ce TaskUsageView. |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | Obtient ou définit un filtre utilisé dans une vue unique. |
| [Group](../../aspose.tasks/view/group/) { get; set; } | Obtient ou définit un groupe de la vue unique. |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | Obtient ou définit une valeur indiquant si Microsoft Project met en évidence le filtre pour une vue unique. |
| [MiddleTimescaleTier](../../aspose.tasks/usageview/middletimescaletier/) { get; set; } | Obtient ou définit les paramètres du niveau intermédiaire de l’échelle de temps de la vue. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/). |
| [Name](../../aspose.tasks/view/name/) { get; set; } | Obtient ou définit le nom d’un objet View. |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | Obtient une instance de la classe [`PageInfo`](../view/pageinfo/). Représente les données de configuration de page présentes dans le format de fichier mpp. |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | Obtient le parent de l’objet View. Lecture seule [`Project`](../project/). |
| [RepeatDetailsHeaderOnAllRows](../../aspose.tasks/usageview/repeatdetailsheaderonallrows/) { get; set; } | Obtient ou définit une valeur indiquant s’il faut répéter l’en-tête de détail sur toutes les lignes d’affectation ou non. |
| [Screen](../../aspose.tasks/view/screen/) { get; } | Obtient le type d’écran pour la vue unique. Lecture seule [`ViewScreen`](../viewscreen/). |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | Obtient ou définit une valeur indiquant si Microsoft Project affiche le nom de la vue unique dans les listes déroulantes Vue ou Autres Vues du Ruban. |
| [Table](../../aspose.tasks/view/table/) { get; set; } | Obtient ou définit une table de la vue unique. |
| [TimescaleSizePercentage](../../aspose.tasks/usageview/timescalesizepercentage/) { get; set; } |  |
| [TopTimescaleTier](../../aspose.tasks/usageview/toptimescaletier/) { get; set; } | Obtient ou définit les paramètres du niveau supérieur de l’échelle de temps de la vue. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/). |
| [Type](../../aspose.tasks/view/type/) { get; } | Obtient le type d’élément dans la vue unique, tel que les tâches ou les ressources. Lecture seule [`ItemType`](../itemtype/). |
| [Uid](../../aspose.tasks/view/uid/) { get; } | Obtient l’identifiant unique d’une vue. |
| [VisualObjectsPlacements](../../aspose.tasks/view/visualobjectsplacements/) { get; } | Obtient une collection d’objets représentant le placement et l’apparence de [`OleObject`](../oleobject/) dans la vue. |

## Méthodes

| Nom | Description |
| --- | --- |
| [CompareTo](../../aspose.tasks/view/compareto/)(View) | Compare l’instance actuelle avec un autre objet du même type et renvoie un entier indiquant si l’instance actuelle précède, suit ou se trouve à la même position dans l’ordre de tri que l’autre objet. |
| override [Equals](../../aspose.tasks/view/equals/)(object) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| override [GetHashCode](../../aspose.tasks/view/gethashcode/)() | Renvoie une valeur de code de hachage pour l’instance de la classe [`Resource`](../resource/). |

## Exemples

Montre comment rendre la vue d'utilisation des tâches avec les paramètres d'échelle de temps définis dans les paramètres de vue.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = project.Views.ToList()[2] as TaskUsageView;

view.TopTimescaleTier.Unit = TimescaleUnit.None;

view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
view.MiddleTimescaleTier.Label = DateLabel.WeekDddMDd;
view.MiddleTimescaleTier.Count = 1;

view.BottomTimescaleTier.Unit = TimescaleUnit.Days;
view.BottomTimescaleTier.Label = DateLabel.DayMmDd;
view.BottomTimescaleTier.Count = 1;

// Définissez les SaveOptions et spécifiez que les paramètres d'échelle de temps TaskUsageView doivent être utilisés.
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    PresentationFormat = PresentationFormat.TaskUsage
};

project.Save(OutDir + "TaskUsageView_CustomTimescale_out.pdf", options);
```

Montre comment rendre la vue d'utilisation des tâches avec des paramètres d'échelle de temps prédéfinis.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

// Définissez les SaveOptions et spécifiez les paramètres d'échelle de temps prédéfinis 'Days'.
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Days,

    // Définissez le format de présentation sur TaskUsage
    PresentationFormat = PresentationFormat.TaskUsage
};

var outputProject = "TaskUsageView_result_days_out.pdf";
project.Save(OutDir + outputProject, options);

// Définissez les paramètres d'échelle de temps sur ThirdsOfMonths
options.Timescale = Timescale.ThirdsOfMonths;

outputProject = "TaskUsageView_result_thirdsOfMonths_out.pdf";
project.Save(OutDir + outputProject, options);

// Définissez les paramètres d'échelle de temps sur Months
options.Timescale = Timescale.Months;

outputProject = "TaskUsageView_result_months_out.pdf";
project.Save(OutDir + outputProject, options);
```

### Voir aussi

* class [UsageView](../usageview/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


