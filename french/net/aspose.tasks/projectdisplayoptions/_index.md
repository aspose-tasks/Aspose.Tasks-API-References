---
title: "Classe ProjectDisplayOptions"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.ProjectDisplayOptions. Représente les options d’affichage pour une instance de projet"
type: docs
weight: 1450
url: /fr/net/aspose.tasks/projectdisplayoptions/
---
## ProjectDisplayOptions class

Représente les options d'affichage d'une instance de projet.

```csharp
public class ProjectDisplayOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [ProjectDisplayOptions](projectdisplayoptions/)() | Initialise une nouvelle instance de la classe `ProjectDisplayOptions`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [AddSpaceBeforeLabel](../../aspose.tasks/projectdisplayoptions/addspacebeforelabel/) { get; set; } | Obtient ou définit une valeur indiquant s’il faut ajouter un espace avant la valeur numérique et l’abréviation de temps (1 wk au lieu de 1wk). |
| [DayLabel](../../aspose.tasks/projectdisplayoptions/daylabel/) { get; set; } | Obtient ou définit la façon dont l’étiquette du jour s’affiche. |
| [HourLabel](../../aspose.tasks/projectdisplayoptions/hourlabel/) { get; set; } | Obtient ou définit la façon dont l’étiquette de l’heure s’affiche. |
| [MinuteLabel](../../aspose.tasks/projectdisplayoptions/minutelabel/) { get; set; } | Obtient ou définit la façon dont l’étiquette de la minute s’affiche. |
| [MonthLabel](../../aspose.tasks/projectdisplayoptions/monthlabel/) { get; set; } | Obtient ou définit la façon dont l’étiquette du mois s’affiche. |
| [ShowProjectSummaryTask](../../aspose.tasks/projectdisplayoptions/showprojectsummarytask/) { get; set; } | Obtient ou définit une valeur indiquant s’il faut afficher les informations de synthèse d’un projet complet sur une seule ligne avec sa propre barre de tâche de synthèse en haut de la vue du diagramme de Gantt. |
| [ShowTaskScheduleSuggestions](../../aspose.tasks/projectdisplayoptions/showtaskschedulesuggestions/) { get; set; } | Obtient ou définit une valeur indiquant s’il faut afficher des suggestions lorsque Project identifie un conflit d’ordonnancement possible avec une tâche planifiée manuellement. Cette option est disponible pour la version Project 2010 et ultérieure. |
| [ShowTaskScheduleWarnings](../../aspose.tasks/projectdisplayoptions/showtaskschedulewarnings/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut afficher des avertissements lorsque Project identifie un conflit d'échéancier possible avec une tâche planifiée manuellement. Cette option est disponible pour la version Project 2010 et suivantes. |
| [UnderlineHyperlinks](../../aspose.tasks/projectdisplayoptions/underlinehyperlinks/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut souligner les hyperliens. |
| [WeekLabel](../../aspose.tasks/projectdisplayoptions/weeklabel/) { get; set; } | Obtient ou définit comment l'étiquette de la semaine s'affiche. |
| [YearLabel](../../aspose.tasks/projectdisplayoptions/yearlabel/) { get; set; } | Obtient ou définit comment l'étiquette de l'année s'affiche. |

## Exemples

Montre comment utiliser les options d'affichage du projet.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// Définir une valeur indiquant s'il faut afficher des avertissements lorsque Project identifie un conflit d'échéancier possible avec une tâche planifiée manuellement.
// Cette option est disponible pour la version Project 2010 et suivantes.
project.DisplayOptions.ShowTaskScheduleWarnings = false;

// une valeur indiquant s'il faut ajouter un espace avant la valeur numérique et l'abréviation de temps (1 wk au lieu de 1wk)
project.DisplayOptions.AddSpaceBeforeLabel = true;

// définit comment le libellé des minutes est affiché
project.DisplayOptions.MinuteLabel = MinuteLabelDisplay.Min;

// définir comment l'étiquette d'heure est affichée
project.DisplayOptions.HourLabel = HourLabelDisplay.Hr;

// définir comment l'étiquette du jour s'affiche
project.DisplayOptions.DayLabel = DayLabelDisplay.Dy;

// définir comment l'étiquette de la semaine s'affiche
project.DisplayOptions.WeekLabel = WeekLabelDisplay.Week;

// définir comment l'étiquette du mois est affichée
project.DisplayOptions.MonthLabel = MonthLabelDisplay.Mon;

// définir comment l'étiquette d'année est affichée
project.DisplayOptions.YearLabel = YearLabelDisplay.Year;

// définir une valeur indiquant s'il faut afficher les informations récapitulatives d'un projet complet sur une seule ligne avec sa propre barre de tâche récapitulative en haut de la vue du diagramme de Gantt.
project.DisplayOptions.ShowProjectSummaryTask = true;

// définir une valeur indiquant s'il faut afficher des suggestions lorsque Project identifie un conflit d'échéancier possible avec une tâche planifiée manuellement.
project.DisplayOptions.ShowTaskScheduleSuggestions = true;

// définir une valeur indiquant s'il faut souligner les hyperliens.
project.DisplayOptions.UnderlineHyperlinks = true;

project.Save(OutDir + "WorkWithProjectDisplayOptions.mpp", SaveFileFormat.Mpp);
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


