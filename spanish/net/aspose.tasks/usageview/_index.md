---
title: "Clase UsageView"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.UsageView. Representa una vista de uso en un proyecto"
type: docs
weight: 2650
url: /es/net/aspose.tasks/usageview/
---
## UsageView class

Representa una vista de uso en un proyecto.

```csharp
public abstract class UsageView : View
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AlignDetailsData](../../aspose.tasks/usageview/aligndetailsdata/) { get; set; } | Obtiene o establece la alineación de los datos de detalles. |
| [BottomTimescaleTier](../../aspose.tasks/usageview/bottomtimescaletier/) { get; set; } | Obtiene o establece la configuración del nivel inferior de la escala de tiempo de la vista. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/) |
| [DisplayDetailsHeaderColumn](../../aspose.tasks/usageview/displaydetailsheadercolumn/) { get; set; } | Obtiene o establece un valor que indica si se debe mostrar la columna de encabezado de detalles en la vista o no. |
| [DisplayShortDetailHeaderNames](../../aspose.tasks/usageview/displayshortdetailheadernames/) { get; set; } | Obtiene o establece un valor que indica si se deben mostrar los nombres de encabezado de detalle corto o no. |
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

* class [View](../view/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


