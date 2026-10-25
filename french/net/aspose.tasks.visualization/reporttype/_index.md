---
title: "Enum ReportType"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Enum Aspose.Tasks.Visualization.ReportType. Type du rapport graphique du projet"
type: docs
weight: 3330
url: /fr/net/aspose.tasks.visualization/reporttype/
---
## ReportType enumeration

Type du rapport graphique du projet.

```csharp
public enum ReportType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| ProjectOverview | `0` | Affiche la date de début et de fin du projet, le pourcentage de durée terminé, le pourcentage d'achèvement des tâches de niveau supérieur et des jalons à venir. |
| CostOverview | `1` | Affiche les dates de début et de fin du projet, le coût prévu actuel et restant, le % d'achèvement et les valeurs de coût pour les tâches de niveau supérieur. |
| WorkOverview | `2` | Affiche le travail de référence (baseline), réel et restant pour chaque tâche de niveau supérieur ainsi que le travail des ressources. |
| ResourceOverview | `3` | Affiche le travail baseline, réel et restant par ressource. |
| ResourceCostOverview | `4` | Affiche le coût baseline, réel et restant par ressource. |
| CriticalTasks | `5` | Affiche les tâches du projet qui sont critiques. |
| LateTasks | `6` | Affiche les tâches du projet qui sont en retard. |
| Milestones | `7` | Affiche les jalons qui sont en retard, à venir et terminés. |
| UpcomingTask | `8` | Affiche les tâches prévues pendant la semaine en cours et les tâches commençant pendant la semaine en cours. |
| CostOverruns | `9` | Affiche la variance de coût par tâche et par ressource. |
| TaskCostOverview | `10` | Affiche le coût baseline, réel et restant de toutes les tâches de niveau supérieur. |
| OverallocatedResources | `11` | Affiche le nombre d'heures de travail restantes pour les ressources sur-allouées. |
| SlippingTasks | `12` | Affiche les tâches qui doivent se terminer après leurs dates de fin de référence (la référence doit être définie). |
| BestPracticeAnalyzer | `13` | Affiche les tâches sans travail réel, les tâches non assignées, les tâches d'une durée inférieure à 8 heures et les résumés assignés aux ressources. |
| Burndown | `14` | Inclut les graphiques d'épuisement du travail et d'épuisement des tâches. Le graphique d'épuisement du travail montre la quantité de travail terminée par les personnes, la quantité prévue à terminer avant la date de fin du projet, ainsi que l'estimation de référence de la quantité de travail qui serait achevée à ce stade du projet. Le graphique d'épuisement des tâches montre le nombre de tâches terminées, le nombre restant, et l'estimation de référence du nombre de tâches qui seraient terminées à ce stade du projet. |
| CashFlow | `15` | Affiche les coûts et les coûts cumulatifs par trimestre pour toutes les tâches de niveau supérieur. |

## Exemples

Montre comment enregistrer le rapport d'avancement du projet au format PDF dans le flux spécifié.

```csharp
var project = new Project(DataDir + @"Homemoveplan.mpp");
using (var stream = new FileStream(OutDir + "Burndown_out.pdf", FileMode.Create))
{
    project.SaveReport(stream, ReportType.Burndown);
}
```

### Voir aussi

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


