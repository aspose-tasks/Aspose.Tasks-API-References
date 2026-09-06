---
title: "Classe PageMargins"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.Visualization.PageMargins. Représente les marges de page pour l'impression"
type: docs
weight: 3230
url: /fr/net/aspose.tasks.visualization/pagemargins/
---
## PageMargins class

Représente les marges de page pour l'impression.

```csharp
public class PageMargins
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PageMargins](pagemargins/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Borders](../../aspose.tasks.visualization/pagemargins/borders/) { get; set; } | Obtient ou définit une position où imprimer les bordures. Peut être l'une des valeurs de l'énumération [`Border`](../border/). |
| [Bottom](../../aspose.tasks.visualization/pagemargins/bottom/) { get; set; } | Obtient ou définit la taille de la marge inférieure en centimètres. |
| [Left](../../aspose.tasks.visualization/pagemargins/left/) { get; set; } | Obtient ou définit la taille de la marge gauche en centimètres. |
| [Right](../../aspose.tasks.visualization/pagemargins/right/) { get; set; } | Obtient ou définit la taille de la marge droite en centimètres. |
| [Top](../../aspose.tasks.visualization/pagemargins/top/) { get; set; } | Obtient ou définit la taille de la marge supérieure en centimètres. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


