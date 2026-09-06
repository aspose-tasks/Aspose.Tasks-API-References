---
title: "ProjectView.GetDefaultTaskSheetView"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ProjectView. Inclut les colonnes de tâche id, indicateurs, nom, durée, début, fin, prédécesseurs et noms de ressources"
type: docs
weight: 60
url: /fr/net/aspose.tasks.visualization/projectview/getdefaulttasksheetview/
---
## ProjectView.GetDefaultTaskSheetView method

Inclut les colonnes de tâche id, indicateurs, nom, durée, début, fin, prédécesseurs et noms de ressources.

```csharp
public static ProjectView GetDefaultTaskSheetView()
```

### Valeur de retour

une vue qui contient une liste de [`GanttChartColumn`](../../ganttchartcolumn/).

## Exemples

Montre comment enregistrer un projet avec la vue de feuille de tâches.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultTaskSheetView()
};

project.Save(OutDir + "WorkWithProjectView_TaskSheetView_out.pdf", options);
```

### Voir aussi

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


