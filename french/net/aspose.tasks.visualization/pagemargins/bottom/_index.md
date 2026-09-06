---
title: "PageMargins.Bottom"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété PageMargins. Obtient ou définit la taille de la marge inférieure en centimètres"
type: docs
weight: 30
url: /fr/net/aspose.tasks.visualization/pagemargins/bottom/
---
## PageMargins.Bottom property

Obtient ou définit la taille de la marge inférieure en centimètres.

```csharp
public double Bottom { get; set; }
```

## Exemples

Montre comment travailler avec les marges de page.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// modifions la vue par défaut
var margins = project.DefaultView.PageInfo.Margins;

// modifions les marges
margins.Left = 10d;
margins.Top = 10d;
margins.Right = 10d;
margins.Bottom = 10d;
margins.Borders = Border.OutsidePages;

project.Save(OutDir + "WorkWithPageMargins_out.mpp", SaveFileFormat.Mpp);
```

### Voir aussi

* class [PageMargins](../)
* namespace [Aspose.Tasks.Visualization](../../pagemargins/)
* assembly [Aspose.Tasks](../../../)


