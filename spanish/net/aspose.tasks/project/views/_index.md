---
title: "Project.Views"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad del proyecto. Obtiene una lista de objetos View"
type: docs
weight: 1020
url: /es/net/aspose.tasks/project/views/
---
## Project.Views property

Obtiene una lista de objetos [`View`](../../view/) .

```csharp
public ViewCollection Views { get; }
```

## Ejemplos

Muestra cómo establecer una vista predeterminada del proyecto.

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

// establecer vista predeterminada
project.DefaultView = view;

project.Save(OutDir + @"SaveGantChartView_out.mpp", new MPPSaveOptions { WriteViewData = true });
```

### Ver también

* class [ViewCollection](../../viewcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


