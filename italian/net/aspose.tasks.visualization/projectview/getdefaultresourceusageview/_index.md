---
title: "ProjectView.GetDefaultResourceUsageView"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ProjectView. Include le colonne Uid, nome, inizio, fine e lavoro delle risorse"
type: docs
weight: 50
url: /it/net/aspose.tasks.visualization/projectview/getdefaultresourceusageview/
---
## ProjectView.GetDefaultResourceUsageView method

Include le colonne Uid, nome, inizio, fine e risorsa di lavoro.

```csharp
public static ProjectView GetDefaultResourceUsageView()
```

### Valore di ritorno

una vista che contiene un elenco di [`ResourceViewColumn`](../../resourceviewcolumn/).

## Esempi

Mostra come salvare un progetto con la vista di utilizzo delle risorse.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultResourceUsageView()
};

project.Save(OutDir + "WorkWithProjectView_ResourceUsageView_out.pdf", options);
```

### Vedi anche

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


