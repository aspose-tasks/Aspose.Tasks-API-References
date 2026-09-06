---
title: "Enum Border"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Visualization.Border enum. Spécifie le type de bordures"
type: docs
weight: 2970
url: /fr/net/aspose.tasks.visualization/border/
---
## Border enumeration

Spécifie le type de bordures.

```csharp
public enum Border
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| NoBorder | `0` | Aucune bordure. |
| AroundEveryPage | `1` | Autour de chaque page. |
| OutsidePages | `2` | Sur les pages extérieures. |

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


