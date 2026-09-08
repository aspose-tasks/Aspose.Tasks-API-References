---
title: "Clase PageInfo"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Visualization.PageInfo. Representa los datos de configuración de página que están presentes en el formato de archivo MPP y se usan para imprimir."
type: docs
weight: 3200
url: /es/net/aspose.tasks.visualization/pageinfo/
---
## PageInfo class

Representa los datos de configuración de página que están presentes en el formato de archivo MPP y se usan para la impresión.

```csharp
public class PageInfo
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [PageInfo](pageinfo/)() | Inicializa una nueva instancia de la clase `PageInfo`. Representa los datos de configuración de página que están presentes en el formato de archivo MPP y se usan para imprimir. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Footer](../../aspose.tasks.visualization/pageinfo/footer/) { get; set; } | Obtiene o establece una instancia de la clase [`HeaderFooterInfo`](../headerfooterinfo/) que representa datos de pie de página. |
| [Header](../../aspose.tasks.visualization/pageinfo/header/) { get; set; } | Obtiene o establece la instancia de la clase [`HeaderFooterInfo`](../headerfooterinfo/) que representa datos de encabezado. |
| [Legend](../../aspose.tasks.visualization/pageinfo/legend/) { get; set; } | Obtiene o establece una instancia de la clase [`PageLegend`](../pagelegend/) que especifica las opciones de renderizado de la leyenda de página. |
| [Margins](../../aspose.tasks.visualization/pageinfo/margins/) { get; } | Obtiene una instancia de la clase [`PageMargins`](../pagemargins/) que especifica los márgenes de la página. |
| [Name](../../aspose.tasks.visualization/pageinfo/name/) { get; } | Obtiene el nombre de la vista para la cual se usan los datos de configuración. |
| [PageSettings](../../aspose.tasks.visualization/pageinfo/pagesettings/) { get; } | Obtiene una instancia de la clase [`PageSettings`](./pagesettings/) que especifica la configuración de impresión de la página. |
| [PageViewSettings](../../aspose.tasks.visualization/pageinfo/pageviewsettings/) { get; } | Obtiene una instancia de la clase [`PageViewSettings`](./pageviewsettings/) que especifica la configuración de impresión de la vista de página. |

## Ejemplos

Muestra cómo trabajar con la información de página de la vista de MS Project.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// permite modificar la vista predeterminada
var info = project.DefaultView.PageInfo;

Console.WriteLine("Modify Page Info: " + info.Name);

// permite modificar los márgenes
info.Margins.Left = 10d;
info.Margins.Top = 10d;
info.Margins.Right = 10d;
info.Margins.Bottom = 10d;

// modifiquemos la configuración de página
info.PageSettings.IsPortrait = true;
info.PageSettings.PaperSize = PrinterPaperSize.PaperA4;

// modifiquemos la configuración de vista de página
// establece un valor que indica si se imprimen notas.
info.PageViewSettings.PrintNotes = true;

var header = new HeaderFooterInfo
{
    LeftText = "Left header text",
    CenteredText = "Centered header text",
    RightText = "Right header text"
};
var legend = new PageLegend
{
    LeftText =  "Left legend text",
    CenteredText = "Centered legend text",
    RightText = "Right legend text"
};
var footer = new HeaderFooterInfo
{
    LeftText = "Left footer text",
    CenteredText = "Centered footer text",
    RightText = "Right footer text"
};

info.Header = header;
info.Legend = legend;
info.Footer = footer;

// trabajar con el proyecto...
```

### Ver también

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


