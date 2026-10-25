---
title: "ProjectView.GetDefaultResourceUsageView"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ProjectView. Incluye columnas de recurso Uid, nombre, inicio, fin y trabajo"
type: docs
weight: 50
url: /es/net/aspose.tasks.visualization/projectview/getdefaultresourceusageview/
---
## ProjectView.GetDefaultResourceUsageView method

Incluye Uid, name, start, finish y columnas de recurso de trabajo.

```csharp
public static ProjectView GetDefaultResourceUsageView()
```

### Valor devuelto

una vista que contiene una lista de [`ResourceViewColumn`](../../resourceviewcolumn/).

## Ejemplos

Muestra cómo guardar un proyecto con la vista de uso de recursos.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultResourceUsageView()
};

project.Save(OutDir + "WorkWithProjectView_ResourceUsageView_out.pdf", options);
```

### Ver también

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


