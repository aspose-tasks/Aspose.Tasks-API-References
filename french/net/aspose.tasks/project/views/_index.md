---
title: "Project.Views"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété du projet. Obtient une liste d'objets View"
type: docs
weight: 1020
url: /fr/net/aspose.tasks/project/views/
---
## Project.Views property

Obtient une liste d'objets [`View`](../../view/).

```csharp
public ViewCollection Views { get; }
```

## Exemples

Montre comment définir une vue de projet par défaut.

```csharp
var project = new Project(DataDir + "Project5.mpp");

View view = null;
foreach (var v in project.Views)
{
    if (v.Name == "&Gantt Chart")
    {
        view = v;
    }
}

// définir la vue par défaut
project.DefaultView = view;

project.Save(OutDir + @"SaveGantChartView_out.mpp", new MPPSaveOptions { WriteViewData = true });
```

### Voir aussi

* class [ViewCollection](../../viewcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


