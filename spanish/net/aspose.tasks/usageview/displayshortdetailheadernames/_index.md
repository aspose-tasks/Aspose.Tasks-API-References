---
title: "UsageView.DisplayShortDetailHeaderNames"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "UsageView propiedad. Obtiene o establece un valor que indica si se deben mostrar nombres de encabezado de detalle corto o no"
type: docs
weight: 40
url: /es/net/aspose.tasks/usageview/displayshortdetailheadernames/
---
## UsageView.DisplayShortDetailHeaderNames property

Obtiene o establece un valor que indica si se deben mostrar los nombres de encabezado de detalle corto o no.

```csharp
public bool DisplayShortDetailHeaderNames { get; set; }
```

## Ejemplos

Muestra cómo renderizar la vista de uso de tareas con detalles.

```csharp
var project = new Project(DataDir + "TaskUsageViewWithDetails.mpp");

// obtener la vista
UsageView view = (TaskUsageView)project.DefaultView;

// la columna de encabezado de detalles no se mostrará
view.DisplayDetailsHeaderColumn = false;
view.RepeatDetailsHeaderOnAllRows = false;
view.DisplayShortDetailHeaderNames = false;
view.AlignDetailsData = HorizontalStringAlignment.Near;
project.Save(OutDir + "task usage1_out.pdf", SaveFileFormat.Pdf);

// mostrar columna de encabezado de detalles
view.DisplayDetailsHeaderColumn = true;

// repetir encabezado de detalles en todas las filas de asignaciones
view.RepeatDetailsHeaderOnAllRows = true;
view.AlignDetailsData = HorizontalStringAlignment.Far;
project.Save(OutDir + "task usage2_out.pdf", SaveFileFormat.Pdf);
```

### Ver también

* class [UsageView](../)
* namespace [Aspose.Tasks](../../usageview/)
* assembly [Aspose.Tasks](../../../)


