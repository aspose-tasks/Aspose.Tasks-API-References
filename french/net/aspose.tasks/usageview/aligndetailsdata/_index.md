---
title: "UsageView.AlignDetailsData"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "UsageView propriété. Obtient ou définit l'alignement des données détaillées"
type: docs
weight: 10
url: /fr/net/aspose.tasks/usageview/aligndetailsdata/
---
## UsageView.AlignDetailsData property

Obtient ou définit l'alignement des données détaillées.

```csharp
public HorizontalStringAlignment AlignDetailsData { get; set; }
```

## Exemples

Montre comment rendre la vue d’utilisation des tâches avec les détails.

```csharp
var project = new Project(DataDir + "TaskUsageViewWithDetails.mpp");

// obtenir la vue
UsageView view = (TaskUsageView)project.DefaultView;

// la colonne d’en-tête de détail ne sera pas affichée
view.DisplayDetailsHeaderColumn = false;
view.RepeatDetailsHeaderOnAllRows = false;
view.DisplayShortDetailHeaderNames = false;
view.AlignDetailsData = HorizontalStringAlignment.Near;
project.Save(OutDir + "task usage1_out.pdf", SaveFileFormat.Pdf);

// afficher la colonne d’en-tête de détail
view.DisplayDetailsHeaderColumn = true;

// répéter l’en-tête de détail sur toutes les lignes d’affectations
view.RepeatDetailsHeaderOnAllRows = true;
view.AlignDetailsData = HorizontalStringAlignment.Far;
project.Save(OutDir + "task usage2_out.pdf", SaveFileFormat.Pdf);
```

### Voir aussi

* enum [HorizontalStringAlignment](../../../aspose.tasks.visualization/horizontalstringalignment/)
* class [UsageView](../)
* namespace [Aspose.Tasks](../../usageview/)
* assembly [Aspose.Tasks](../../../)


