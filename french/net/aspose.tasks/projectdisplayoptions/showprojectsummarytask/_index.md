---
title: "ProjectDisplayOptions.ShowProjectSummaryTask"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "ProjectDisplayOptions property. Obtient ou définit une valeur indiquant s'il faut afficher les informations récapitulatives d'un projet complet sur une seule ligne avec sa propre barre de tâche récapitulative en haut de la vue du diagramme de Gantt"
type: docs
weight: 70
url: /fr/net/aspose.tasks/projectdisplayoptions/showprojectsummarytask/
---
## ProjectDisplayOptions.ShowProjectSummaryTask property

Obtient ou définit une valeur indiquant s’il faut afficher les informations de synthèse d’un projet complet sur une seule ligne avec sa propre barre de tâche de synthèse en haut de la vue du diagramme de Gantt.

```csharp
public bool ShowProjectSummaryTask { get; set; }
```

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

* class [ProjectDisplayOptions](../)
* namespace [Aspose.Tasks](../../projectdisplayoptions/)
* assembly [Aspose.Tasks](../../../)


