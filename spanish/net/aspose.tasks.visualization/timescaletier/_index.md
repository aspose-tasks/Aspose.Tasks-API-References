---
title: "Clase TimescaleTier"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Visualization.TimescaleTier. Representa un único nivel de la escala de tiempo en un diagrama de Gantt"
type: docs
weight: 3450
url: /es/net/aspose.tasks.visualization/timescaletier/
---
## TimescaleTier class

Representa un nivel único de la escala de tiempo en un diagrama de Gantt.

```csharp
public sealed class TimescaleTier
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [TimescaleTier](timescaletier/#constructor)() | Inicializa una nueva instancia de la clase `TimescaleTier`. |
| [TimescaleTier](timescaletier/#constructor_1)(TimescaleUnit, int) | Inicializa una nueva instancia de la clase `TimescaleTier`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Alignment](../../aspose.tasks.visualization/timescaletier/alignment/) { get; set; } | Obtiene o establece cómo alinear las etiquetas dentro de cada período de tiempo del nivel ([`HorizontalStringAlignment`](../horizontalstringalignment/)). |
| [Count](../../aspose.tasks.visualization/timescaletier/count/) { get; set; } | Obtiene o establece el intervalo de unidad de tiempo en el que se muestran las etiquetas para el nivel. El valor predeterminado es 1. |
| [DateTimeConverter](../../aspose.tasks.visualization/timescaletier/datetimeconverter/) { get; set; } | Obtiene o establece una función de devolución de llamada para manejar el renderizado de marcas de fecha en este nivel. |
| [Label](../../aspose.tasks.visualization/timescaletier/label/) { get; set; } | Obtiene o establece la etiqueta de fecha [`DateLabel`](../datelabel/) para el nivel de escala de tiempo. |
| [RenderLabelOnEachPage](../../aspose.tasks.visualization/timescaletier/renderlabeloneachpage/) { get; set; } | Obtiene o establece la bandera que define si las etiquetas de fecha deben renderizarse en cada página cuando un período de tiempo abarca varias páginas. Si el valor es 'true', cuando el período de tiempo abarca varias páginas, las etiquetas de fecha para el período se renderizan en cada página. Si el valor es 'false', la etiqueta de fecha se renderiza solo una vez según el valor de la propiedad [`Alignment`](./alignment/). |
| [ShowTicks](../../aspose.tasks.visualization/timescaletier/showticks/) { get; set; } | Obtiene o establece un valor que indica si se deben mostrar marcas de graduación que separan los períodos de tiempo en el nivel. |
| [Unit](../../aspose.tasks.visualization/timescaletier/unit/) { get; set; } | Obtiene o establece la unidad de escala de tiempo [`TimescaleUnit`](../timescaleunit/) para el nivel de escala de tiempo. El valor predeterminado es [`Days`](../timescaleunit/). |
| [UsesFiscalYear](../../aspose.tasks.visualization/timescaletier/usesfiscalyear/) { get; set; } | Obtiene o establece un valor que indica si las etiquetas del nivel se basan en el año fiscal. |

## Ejemplos

Muestra cómo personalizar las etiquetas del nivel de escala de tiempo.

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");

// Agregar enlaces de tareas
project.TaskLinks.Add(project.RootTask.Children.Add("Task 1"), project.RootTask.Children.Add("Task 2"));

var view = (GanttChartView)project.DefaultView;

// ajustar los niveles de escala de tiempo

// ajustar el nivel superior
// establecer el nivel superior de escala de tiempo de la vista del diagrama de Gantt.
view.MiddleTimescaleTier = new TimescaleTier();
// establecer la unidad de escala de tiempo <see cref=\"T:Aspose.Tasks.Visualization.TimescaleUnit\" /> para el nivel de escala de tiempo.
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
// establecer el intervalo de unidad de tiempo en el que se muestran las etiquetas para el nivel.
view.MiddleTimescaleTier.Count = 1;
// establecer la etiqueta de fecha <see cref=\"T:Aspose.Tasks.Visualization.DateLabel\" /> para el nivel de escala de tiempo.
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
// establecer cómo alinear las etiquetas dentro de cada período de tiempo del nivel (<see cref=\"T:System.Drawing.StringAlignment\" />).
view.MiddleTimescaleTier.Alignment = HorizontalStringAlignment.Center;
// establecer un valor que indique si se deben mostrar marcas de verificación que separan los períodos de tiempo en el nivel.
view.MiddleTimescaleTier.ShowTicks = true;
// establecer un valor que indique si basar las etiquetas del nivel en el año fiscal.
view.MiddleTimescaleTier.UsesFiscalYear = true;

// agregado para una mejor visualización
view.TopTimescaleTier = new TimescaleTier(TimescaleUnit.Months, 1);

// personalizar las fechas del nivel intermedio
view.TopTimescaleTier.DateTimeConverter = date =>
    new[] { "Янв.", "Фев.", "Мар.", "Апр.", "Май", "Июнь", "Июль", "Авг.", "Сен.", "Окт.", "Ноя.", "Дек." }[date.Month - 1];

project.Set(Prj.TimescaleStart, new DateTime(2012, 7, 30));
project.Set(Prj.TimescaleFinish, new DateTime(2012, 10, 6));

// Utilizar la opción 'Timescale.DefinedInView' para representar escalas de tiempo usando la configuración de escalas de tiempo definida en la vista (view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier).
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "CustomizeTimescaleTierLabels_out.pdf", pdfSaveOptions);
```

### Ver también

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


