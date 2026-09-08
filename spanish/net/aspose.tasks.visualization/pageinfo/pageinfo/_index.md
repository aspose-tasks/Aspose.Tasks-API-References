---
title: "PageInfo.PageInfo"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor PageInfo. Inicializa una nueva instancia de la clase PageInfo. Representa los datos de configuración de página que están presentes en el formato de archivo MPP y se utilizan para la impresión"
type: docs
weight: 10
url: /es/net/aspose.tasks.visualization/pageinfo/pageinfo/
---
## PageInfo constructor

Inicializa una nueva instancia de la clase [`PageInfo`](../). Representa los datos de configuración de página que están presentes en el formato de archivo MPP y se utilizan para la impresión.

```csharp
public PageInfo()
```

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

* class [PageInfo](../)
* namespace [Aspose.Tasks.Visualization](../../pageinfo/)
* assembly [Aspose.Tasks](../../../)


