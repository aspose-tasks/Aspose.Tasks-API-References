---
title: "Clase TaskUsageView"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.TaskUsageView. Representa la vista de uso de tareas en un proyecto"
type: docs
weight: 2480
url: /es/net/aspose.tasks/taskusageview/
---
## TaskUsageView class

Representa la vista de uso de tareas en un proyecto.

```csharp
public class TaskUsageView : UsageView
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AlignDetailsData](../../aspose.tasks/usageview/aligndetailsdata/) { get; set; } | Obtiene o establece la alineación de los datos de detalles. |
| [BottomTimescaleTier](../../aspose.tasks/usageview/bottomtimescaletier/) { get; set; } | Obtiene o establece la configuración del nivel inferior de la escala de tiempo de la vista. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/) |
| [DisplayDetailsHeaderColumn](../../aspose.tasks/usageview/displaydetailsheadercolumn/) { get; set; } | Obtiene o establece un valor que indica si se debe mostrar la columna de encabezado de detalles en la vista o no. |
| [DisplayShortDetailHeaderNames](../../aspose.tasks/usageview/displayshortdetailheadernames/) { get; set; } | Obtiene o establece un valor que indica si se deben mostrar los nombres de encabezado de detalle corto o no. |
| [FieldCollection](../../aspose.tasks/taskusageview/fieldcollection/) { get; } | Obtiene el objeto [`TaskUsageViewFieldCollection`](../taskusageviewfieldcollection/) de este TaskUsageView. |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | Obtiene o establece un filtro utilizado en una vista única. |
| [Group](../../aspose.tasks/view/group/) { get; set; } | Obtiene o establece un grupo de la vista única. |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | Obtiene o establece un valor que indica si Microsoft Project resalta el filtro para una vista única. |
| [MiddleTimescaleTier](../../aspose.tasks/usageview/middletimescaletier/) { get; set; } | Obtiene o establece la configuración del nivel medio de la escala de tiempo de la vista. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/). |
| [Name](../../aspose.tasks/view/name/) { get; set; } | Obtiene o establece el nombre de un objeto View. |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | Obtiene una instancia de la clase [`PageInfo`](../view/pageinfo/). Representa los datos de configuración de página que están presentes en el formato de archivo mpp. |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | Obtiene el padre del objeto View. Solo lectura [`Project`](../project/). |
| [RepeatDetailsHeaderOnAllRows](../../aspose.tasks/usageview/repeatdetailsheaderonallrows/) { get; set; } | Obtiene o establece un valor que indica si se repite el encabezado de detalles en todas las filas de asignación o no. |
| [Screen](../../aspose.tasks/view/screen/) { get; } | Obtiene el tipo de pantalla para la vista única. Solo lectura [`ViewScreen`](../viewscreen/). |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | Obtiene o establece un valor que indica si Microsoft Project muestra el nombre de la vista única en las listas desplegables Vista u Otras Vistas en la cinta de opciones. |
| [Table](../../aspose.tasks/view/table/) { get; set; } | Obtiene o establece una tabla de la vista única. |
| [TimescaleSizePercentage](../../aspose.tasks/usageview/timescalesizepercentage/) { get; set; } |  |
| [TopTimescaleTier](../../aspose.tasks/usageview/toptimescaletier/) { get; set; } | Obtiene o establece la configuración del nivel superior de la escala de tiempo de la vista. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/). |
| [Type](../../aspose.tasks/view/type/) { get; } | Obtiene el tipo de elemento en la vista única, como tareas o recursos. Solo lectura [`ItemType`](../itemtype/). |
| [Uid](../../aspose.tasks/view/uid/) { get; } | Obtiene el identificador único de una vista. |
| [VisualObjectsPlacements](../../aspose.tasks/view/visualobjectsplacements/) { get; } | Obtiene una colección de objetos que representan la ubicación y apariencia de [`OleObject`](../oleobject/) en la vista. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [CompareTo](../../aspose.tasks/view/compareto/)(View) | Compara la instancia actual con otro objeto del mismo tipo y devuelve un entero que indica si la instancia actual precede, sigue o se encuentra en la misma posición en el orden de clasificación que el otro objeto. |
| override [Equals](../../aspose.tasks/view/equals/)(object) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| override [GetHashCode](../../aspose.tasks/view/gethashcode/)() | Devuelve un valor de código hash para la instancia de la clase [`Resource`](../resource/). |

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

Muestra cómo renderizar la vista de uso de tareas con ajustes de escala de tiempo predefinidos.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

// Defina las SaveOptions y especifique los ajustes predefinidos de TimeScale 'Days'.
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Days,

    // Establezca el formato de Presentación a TaskUsage
    PresentationFormat = PresentationFormat.TaskUsage
};

var outputProject = "TaskUsageView_result_days_out.pdf";
project.Save(OutDir + outputProject, options);

// Establezca los ajustes de Timescale a ThirdsOfMonths
options.Timescale = Timescale.ThirdsOfMonths;

outputProject = "TaskUsageView_result_thirdsOfMonths_out.pdf";
project.Save(OutDir + outputProject, options);

// Establezca los ajustes de Timescale a Months
options.Timescale = Timescale.Months;

outputProject = "TaskUsageView_result_months_out.pdf";
project.Save(OutDir + outputProject, options);
```

### Ver también

* class [UsageView](../usageview/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


