---
title: "UsageView.DisplayDetailsHeaderColumn"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad UsageView. Obtiene o establece un valor que indica si se debe mostrar la columna de encabezado de detalles en la vista o no"
type: docs
weight: 30
url: /es/net/aspose.tasks/usageview/displaydetailsheadercolumn/
---
## UsageView.DisplayDetailsHeaderColumn property

Obtiene o establece un valor que indica si se debe mostrar la columna de encabezado de detalles en la vista o no.

```csharp
public bool DisplayDetailsHeaderColumn { get; set; }
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


