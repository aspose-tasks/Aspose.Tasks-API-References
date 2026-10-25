---
title: "Classe ProjectView"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Visualization.ProjectView class. Classe de vue des projets"
type: docs
weight: 3300
url: /fr/net/aspose.tasks.visualization/projectview/
---
## ProjectView class

Classe de vue du projet

```csharp
public class ProjectView
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [ProjectView](projectview/)(IEnumerable&lt;ViewColumn&gt;) | Initialise une nouvelle instance de la classe `ProjectView`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Columns](../../aspose.tasks.visualization/projectview/columns/) { get; } | Obtient les colonnes de la vue du projet. |

## Méthodes

| Nom | Description |
| --- | --- |
| static [GetDefaultAssignmentView](../../aspose.tasks.visualization/projectview/getdefaultassignmentview/)() | Inclut les colonnes Uid, nom de tâche, nom de ressource, travail et durée d'affectation. |
| static [GetDefaultGanttChartView](../../aspose.tasks.visualization/projectview/getdefaultganttchartview/)() | Inclut les colonnes id, indicateurs, nom, durée, début et fin de tâche. |
| static [GetDefaultResourceSheetView](../../aspose.tasks.visualization/projectview/getdefaultresourcesheetview/)() | Inclut les colonnes Uid, nom de ressource, type, libellé du matériau, initiales, groupe, unités max, tarif standard, tarif des heures supplémentaires, coût par utilisation, accumulé à, calendrier de base et code ressource. |
| static [GetDefaultResourceUsageView](../../aspose.tasks.visualization/projectview/getdefaultresourceusageview/)() | Inclut les colonnes Uid, nom, début, fin et ressource de travail. |
| static [GetDefaultTaskSheetView](../../aspose.tasks.visualization/projectview/getdefaulttasksheetview/)() | Inclut les colonnes de tâche id, indicateurs, nom, durée, début, fin, prédécesseurs et noms de ressources. |

## Exemples

Montre comment enregistrer un projet avec la vue d'affectation.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultAssignmentView()
};

project.Save(OutDir + "WorkWithProjectView_AssignmentView_out.pdf", options);
```

### Voir aussi

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


