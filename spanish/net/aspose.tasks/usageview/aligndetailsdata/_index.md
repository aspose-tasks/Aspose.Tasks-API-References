---
title: "UsageView.AlignDetailsData"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "UsageView propiedad. Obtiene o establece la alineación de los datos de detalles"
type: docs
weight: 10
url: /es/net/aspose.tasks/usageview/aligndetailsdata/
---
## UsageView.AlignDetailsData property

Obtiene o establece la alineación de los datos de detalles.

```csharp
public HorizontalStringAlignment AlignDetailsData { get; set; }
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

* enum [HorizontalStringAlignment](../../../aspose.tasks.visualization/horizontalstringalignment/)
* class [UsageView](../)
* namespace [Aspose.Tasks](../../usageview/)
* assembly [Aspose.Tasks](../../../)


