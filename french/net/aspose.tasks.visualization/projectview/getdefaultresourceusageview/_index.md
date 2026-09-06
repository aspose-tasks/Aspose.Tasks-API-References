---
title: "ProjectView.GetDefaultResourceUsageView"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ProjectView. Inclut les colonnes de ressource uid, nom, début, fin et travail"
type: docs
weight: 50
url: /fr/net/aspose.tasks.visualization/projectview/getdefaultresourceusageview/
---
## ProjectView.GetDefaultResourceUsageView method

Inclut les colonnes Uid, nom, début, fin et ressource de travail.

```csharp
public static ProjectView GetDefaultResourceUsageView()
```

### Valeur de retour

une vue qui contient une liste de [`ResourceViewColumn`](../../resourceviewcolumn/).

## Exemples

Montre comment enregistrer un projet avec la vue d'utilisation des ressources.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultResourceUsageView()
};

project.Save(OutDir + "WorkWithProjectView_ResourceUsageView_out.pdf", options);
```

### Voir aussi

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


