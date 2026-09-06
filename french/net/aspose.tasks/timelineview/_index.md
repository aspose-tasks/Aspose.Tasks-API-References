---
title: "Classe TimelineView"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.TimelineView. Représente une vue de chronologie d'un projet"
type: docs
weight: 2580
url: /fr/net/aspose.tasks/timelineview/
---
## TimelineView class

Représente une vue de chronologie d'un projet.

```csharp
public class TimelineView : View
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [TimelineView](timelineview/)() | Initialise une nouvelle instance de la classe `TimelineView`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [DateFormat](../../aspose.tasks/timelineview/dateformat/) { get; set; } | Obtient ou définit une valeur indiquant comment formater les dates dans la vue Timeline. |
| [DisplayOverlapped](../../aspose.tasks/timelineview/displayoverlapped/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut afficher les tâches qui se chevauchent sur plusieurs lignes. |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | Obtient ou définit un filtre utilisé dans une vue unique. |
| [Group](../../aspose.tasks/view/group/) { get; set; } | Obtient ou définit un groupe de la vue unique. |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | Obtient ou définit une valeur indiquant si Microsoft Project met en évidence le filtre pour une vue unique. |
| [Name](../../aspose.tasks/view/name/) { get; set; } | Obtient ou définit le nom d’un objet View. |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | Obtient une instance de la classe [`PageInfo`](../view/pageinfo/). Représente les données de configuration de page présentes dans le format de fichier mpp. |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | Obtient le parent de l’objet View. Lecture seule [`Project`](../project/). |
| [Screen](../../aspose.tasks/view/screen/) { get; } | Obtient le type d’écran pour la vue unique. Lecture seule [`ViewScreen`](../viewscreen/). |
| [ShowDates](../../aspose.tasks/timelineview/showdates/) { get; } | Obtient une valeur indiquant s'il faut afficher les dates. |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | Obtient ou définit une valeur indiquant si Microsoft Project affiche le nom de la vue unique dans les listes déroulantes Vue ou Autres Vues du Ruban. |
| [ShowPanZoom](../../aspose.tasks/timelineview/showpanzoom/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut afficher le contrôle de panoramique et de zoom. |
| [ShowTimescale](../../aspose.tasks/timelineview/showtimescale/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut afficher l'échelle de temps. |
| [ShowToday](../../aspose.tasks/timelineview/showtoday/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut afficher une ligne représentant aujourd'hui. |
| [Table](../../aspose.tasks/view/table/) { get; set; } | Obtient ou définit une table de la vue unique. |
| [TextLinesCount](../../aspose.tasks/timelineview/textlinescount/) { get; set; } | Obtient ou définit une valeur indiquant combien de lignes sont utilisées pour afficher les tâches dans une chronologie. |
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

Montre comment travailler avec &lt;see cref=\"Aspose.Tasks.TimelineView\" /&gt;.

```csharp
var project = new Project();

// initialiser une vue de chronologie
var view = new TimelineView();

// définir une valeur indiquant comment formater les dates dans la vue Timeline.
view.DateFormat = DateFormat.DateDddDd;
// définir une valeur indiquant s'il faut afficher les tâches qui se chevauchent sur plusieurs lignes.
view.DisplayOverlapped = true;
// définir une valeur indiquant s'il faut afficher le contrôle de panoramique et de zoom.
view.ShowPanZoom = true;
// définir une valeur indiquant s'il faut afficher l'échelle de temps.
view.ShowTimescale = true;
// définir une valeur indiquant s'il faut afficher une ligne représentant aujourd'hui.
view.ShowToday = true;
// définir une valeur indiquant combien de lignes sont utilisées pour afficher les tâches dans une chronologie.
view.TextLinesCount = 2;

// obtient une valeur indiquant s'il faut afficher les tâches qui se chevauchent sur plusieurs lignes.
Console.WriteLine("Show Dates: " + view.ShowDates);

// ajouter la vue au projet
project.Views.Add(view);

// ajouter des données de test au projet
var task1 = project.RootTask.Children.Add("Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 4, 29, 8, 0, 0));
task1.Set(Tsk.Duration, task1.ParentProject.GetDuration(24, TimeUnitType.Hour));
var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Start, new DateTime(2020, 4, 29, 8, 0, 0));
task2.Set(Tsk.Duration, task1.ParentProject.GetDuration(40, TimeUnitType.Hour));

project.Save(OutDir + "SetTimeScaleCount_out.pdf", SaveFileFormat.Pdf);
```

### Voir aussi

* class [View](../view/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


