---
title: "UsageView.BottomTimescaleTier"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad UsageView. Obtiene o establece la configuración del nivel inferior de escala de tiempo de las vistas. TimescaleTier"
type: docs
weight: 20
url: /es/net/aspose.tasks/usageview/bottomtimescaletier/
---
## UsageView.BottomTimescaleTier property

Obtiene o establece la configuración del nivel inferior de escala de tiempo de la vista. [`TimescaleTier`](../../../aspose.tasks.visualization/timescaletier/)

```csharp
public TimescaleTier BottomTimescaleTier { get; set; }
```

## Ejemplos

Muestra cómo renderizar la vista de uso de tareas con la configuración de escala de tiempo definida en la configuración de la vista.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = project.Views.ToList()[2] as TaskUsageView;

view.TopTimescaleTier.Unit = TimescaleUnit.None;

view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
view.MiddleTimescaleTier.Label = DateLabel.WeekDddMDd;
view.MiddleTimescaleTier.Count = 1;

view.BottomTimescaleTier.Unit = TimescaleUnit.Days;
view.BottomTimescaleTier.Label = DateLabel.DayMmDd;
view.BottomTimescaleTier.Count = 1;

// Defina las SaveOptions y especifique que se deben usar los ajustes de escala de tiempo de TaskUsageView.
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    PresentationFormat = PresentationFormat.TaskUsage
};

project.Save(OutDir + "TaskUsageView_CustomTimescale_out.pdf", options);
```

### Ver también

* class [TimescaleTier](../../../aspose.tasks.visualization/timescaletier/)
* class [UsageView](../)
* namespace [Aspose.Tasks](../../usageview/)
* assembly [Aspose.Tasks](../../../)


