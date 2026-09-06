---
title: "ProjectView.GetDefaultAssignmentView"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ProjectView. Inclut les colonnes d'affectation Uid, tâche, nom, ressource, travail et durée"
type: docs
weight: 20
url: /fr/net/aspose.tasks.visualization/projectview/getdefaultassignmentview/
---
## ProjectView.GetDefaultAssignmentView method

Inclut les colonnes Uid, nom de tâche, nom de ressource, travail et durée d'affectation.

```csharp
public static ProjectView GetDefaultAssignmentView()
```

### Valeur de retour

une vue qui contient une liste de [`AssignmentViewColumn`](../../assignmentviewcolumn/).

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

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


