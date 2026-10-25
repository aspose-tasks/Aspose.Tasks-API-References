---
title: "PageMargins.Borders"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété PageMargins. Obtient ou définit une position où imprimer les bordures. Peut être l'une des valeurs de l'énumération Border."
type: docs
weight: 20
url: /fr/net/aspose.tasks.visualization/pagemargins/borders/
---
## PageMargins.Borders property

Obtient ou définit une position où imprimer les bordures. Peut être l'une des valeurs de l'énumération [`Border`](../../border/).

```csharp
public Border Borders { get; set; }
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

* enum [Border](../../border/)
* class [PageMargins](../)
* namespace [Aspose.Tasks.Visualization](../../pagemargins/)
* assembly [Aspose.Tasks](../../../)


