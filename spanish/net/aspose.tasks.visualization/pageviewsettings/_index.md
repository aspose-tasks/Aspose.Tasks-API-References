---
title: "Clase PageViewSettings"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.Visualization.PageViewSettings clase. Representa la configuración de impresión para una vista del proyecto"
type: docs
weight: 3260
url: /es/net/aspose.tasks.visualization/pageviewsettings/
---
## PageViewSettings class

Representa la configuración de impresión para una vista del proyecto.

```csharp
public class PageViewSettings
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [PageViewSettings](pageviewsettings/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [FirstColumnsCount](../../aspose.tasks.visualization/pageviewsettings/firstcolumnscount/) { get; set; } | Obtiene o establece el número de primeras columnas que se imprimirán en todas las páginas. |
| [FitTimescaleToEndOfPage](../../aspose.tasks.visualization/pageviewsettings/fittimescaletoendofpage/) { get; set; } | Obtiene o establece un valor que indica si se ajusta la escala de tiempo al final de una página al imprimir. |
| [PrintAllSheetColumns](../../aspose.tasks.visualization/pageviewsettings/printallsheetcolumns/) { get; set; } | Obtiene o establece un valor que indica si se imprimen todas las columnas de hoja de una vista. |
| [PrintBlankPages](../../aspose.tasks.visualization/pageviewsettings/printblankpages/) { get; set; } | Obtiene o establece un valor que indica si se imprimen páginas en blanco de una vista. |
| [PrintFirstColumnsCountOnAllPages](../../aspose.tasks.visualization/pageviewsettings/printfirstcolumnscountonallpages/) { get; set; } | Obtiene o establece un valor que indica si se imprime un número especificado de primeras columnas en todas las páginas. |
| [PrintNotes](../../aspose.tasks.visualization/pageviewsettings/printnotes/) { get; set; } | Obtiene o establece un valor que indica si se imprimen notas. |

## Ejemplos

Muestra cómo imprimir notas de tareas, recursos y asignaciones en una página separada.

```csharp
var project = new Project(DataDir + "Input.mpp");

// establece el número de primeras columnas que se imprimirán en todas las páginas
project.DefaultView.PageInfo.PageViewSettings.FirstColumnsCount = 2;

// establece un valor que indica si se imprimen notas.
project.DefaultView.PageInfo.PageViewSettings.PrintNotes = true;

// establece un valor que indica si se ajusta la escala de tiempo al final de una página al imprimir.
project.DefaultView.PageInfo.PageViewSettings.FitTimescaleToEndOfPage = true;

// establece un valor que indica si se imprimen todas las columnas de hoja de una vista
project.DefaultView.PageInfo.PageViewSettings.PrintAllSheetColumns = true;

// establece un valor que indica si se imprimen páginas en blanco de una vista
project.DefaultView.PageInfo.PageViewSettings.PrintBlankPages = false;

// establece un valor que indica si se deben imprimir un número especificado de primeras columnas en todas las páginas
project.DefaultView.PageInfo.PageViewSettings.PrintFirstColumnsCountOnAllPages = true;

project.Save(OutDir + "ProjectWithComments_out.pdf", SaveFileFormat.Pdf);
```

### Ver también

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


