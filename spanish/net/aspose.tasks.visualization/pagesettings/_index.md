---
title: "Clase PageSettings"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Visualization.PageSettings. Representa la configuración de impresión para una página de la vista del proyecto"
type: docs
weight: 3240
url: /es/net/aspose.tasks.visualization/pagesettings/
---
## PageSettings class

Representa la configuración de impresión para una página de la vista del proyecto.

```csharp
public class PageSettings
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [PageSettings](pagesettings/)() | Inicializa una nueva instancia de la clase `PageSettings`. Representa la configuración de impresión para una página de la vista del proyecto. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AdjustToPercentOfNormalSize](../../aspose.tasks.visualization/pagesettings/adjusttopercentofnormalsize/) { get; set; } | Obtiene o establece un valor que indica si se debe ajustar la impresión al porcentaje especificado ([`PercentOfNormalSize`](./percentofnormalsize/)) del tamaño normal. |
| [FirstPageNumber](../../aspose.tasks.visualization/pagesettings/firstpagenumber/) { get; set; } | Obtiene o establece el número de la primera página para imprimir. |
| [IsPortrait](../../aspose.tasks.visualization/pagesettings/isportrait/) { get; set; } | Obtiene o establece un valor que indica si la orientación de la página es vertical; devuelve false si la orientación de la página es horizontal. |
| [PagesInHeight](../../aspose.tasks.visualization/pagesettings/pagesinheight/) { get; set; } | Obtiene o establece la cantidad de páginas en altura que se imprimirán. |
| [PagesInWidth](../../aspose.tasks.visualization/pagesettings/pagesinwidth/) { get; set; } | Obtiene o establece la cantidad de páginas en anchura que se imprimirán. |
| [PaperSize](../../aspose.tasks.visualization/pagesettings/papersize/) { get; set; } | Obtiene o establece un tamaño de papel. Puede ser uno de los valores de la enumeración [`PrinterPaperSize`](../printerpapersize/). |
| [PaperSizeId](../../aspose.tasks.visualization/pagesettings/papersizeid/) { get; set; } | Obtiene o establece un entero que representa uno de los valores de PrinterPaperSize o un identificador de tamaño de página personalizado. Este valor puede usarse para obtener PaperSize de la configuración del sistema operativo. |
| [PercentOfNormalSize](../../aspose.tasks.visualization/pagesettings/percentofnormalsize/) { get; set; } | Obtiene o establece un porcentaje del tamaño normal al que se debe ajustar la impresión. |

## Ejemplos

Muestra cómo trabajar con &lt;see cref=\"Aspose.Tasks.Visualization.PageSettings\" /&gt;.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// obtener la configuración
var settings = project.DefaultView.PageInfo.PageSettings;
// ajustemos algunas propiedades
// establece un valor que indica si la orientación de la página es vertical; devuelve false si la orientación de la página es horizontal.
settings.IsPortrait = true;
// establece la cantidad de páginas en anchura que se imprimirán.
settings.PagesInWidth = 5;
// establece la cantidad de páginas en altura que se imprimirán.
settings.PagesInHeight = 7;
// establece un porcentaje del tamaño normal al que se debe ajustar la impresión.
settings.PercentOfNormalSize = 200;
// establece un tamaño de papel. Puede ser uno de los valores de la enumeración <see cref=\"T:Aspose.Tasks.Visualization.PrinterPaperSize\" />.
settings.PaperSize = PrinterPaperSize.PaperB4;
// establece el número de la primera página para imprimir.
settings.FirstPageNumber = 3;

SimpleSaveOptions options = new MPPSaveOptions
{
    WriteViewData = true
};

project.Save(OutDir + "TestCanWritePageSettings.mpp", options);
```

### Ver también

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


