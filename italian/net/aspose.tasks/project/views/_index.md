---
title: "Project.Views"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà del progetto. Ottiene un elenco di oggetti View"
type: docs
weight: 1020
url: /it/net/aspose.tasks/project/views/
---
## Project.Views property

Ottiene un elenco di oggetti [`View`](../../view/).

```csharp
public ViewCollection Views { get; }
```

## Esempi

Mostra come impostare una vista predefinita del progetto.

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

// imposta vista predefinita
project.DefaultView = view;

project.Save(OutDir + @"SaveGantChartView_out.mpp", new MPPSaveOptions { WriteViewData = true });
```

### Vedi anche

* class [ViewCollection](../../viewcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


