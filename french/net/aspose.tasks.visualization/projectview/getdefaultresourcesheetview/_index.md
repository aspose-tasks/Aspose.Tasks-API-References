---
title: "ProjectView.GetDefaultResourceSheetView"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ProjectView. Inclut les colonnes de ressource Uid, nom, type, matériau, libellé, initiales, groupe, unités max, tarif standard, tarif heures supplémentaires, coût par utilisation, accumulé, calendrier de base et code"
type: docs
weight: 40
url: /fr/net/aspose.tasks.visualization/projectview/getdefaultresourcesheetview/
---
## ProjectView.GetDefaultResourceSheetView method

Inclut les colonnes Uid, nom de ressource, type, libellé du matériau, initiales, groupe, unités max, tarif standard, tarif des heures supplémentaires, coût par utilisation, accumulé à, calendrier de base et code ressource.

```csharp
public static ProjectView GetDefaultResourceSheetView()
```

### Valeur de retour

une vue qui contient une liste de [`ResourceViewColumn`](../../resourceviewcolumn/).

## Exemples

Montre comment enregistrer un projet avec la vue de feuille de ressources.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultResourceSheetView()
};

project.Save(OutDir + "WorkWithProjectView_ResourceSheetView_out.pdf", options);
```

### Voir aussi

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


